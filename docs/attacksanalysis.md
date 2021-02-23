[Back: Security Considerations](securityconsiderations.md)

# Attacks Analysis

This section lists common questions / attacks people might have in mind, and our thoughts on how these are mitigated.

## Malicious Retrieval Provider: Attempted CID Denial of Service

_Scenario_

Client C wants content associated with CID. Assume a Retrieval Gateway G has an offer from malicious Retrieval Provider mRP for the content. mRP could block this content simply because they are nefarious. Alternatively, a Government security agency could tell Retrieval Provider mRP to block content CID.

* mRP creates a CID Group Offer containing CID with a very low price and very good QoS and long expiry time. mRP publishes the CID Group Offer to Retrieval Gateway G.
* When G receives a request for CID from a client C, it returns the CID Group Offer from mRP.
* G provides C with the CID Group Offer showing that mRP can supply content for CID at a good price.
* As the price offered by mRP is less than all other offers, C attempts to retrieve content from mRP.
* G will offer to be a payment broker for mRP.
* C pays the full discovery payment to G.
* C sends the first micro-payment for content to G, expecting G to forward the payment to mRP.
* mRP never sends any content to C.
* When C receives no content it reduces the reputation score for G and adds mRP to its banned list.
* C asks other Retrieval Gateways for the content. If G had returned offers from other Retrieval Providers, it could attempt to pursue one of the other offers.

_Analysis_

For the non-state based actor scenario:

* Retrieval Providers are long lived entities that have staked money. Damaging their reputation like this will yield small amounts of money by their nefarious activities, but will prevent them from greater gains that could be achieved by obeying the protocol.
* The malicious Retrieval Provider is not successful in their attack as the Client will still be able to obtain the content via another Retrieval Provider.

For the state-based actor scenario:

* The Retrieval Provider will accept the damaged reputation because the government agency has told them to block the content. They will see this as the cost of complying with government requirements / legal take-down requests.
* The Client will detect the attempt to block the content and will have to obtain the content from another Retrieval Provider.

## Malicious Retrieval Gateway and Retrieval Provider: Fake CID Offers

_Scenario_

Client C wants content associated with CID. Assume a malicious Retrieval Gateway mG works cooperatively with malicious Retrieval Provider mRP.

* When mG receives a request from C, it asks mRP to create a Single CID Offer for the requested CID.
* mG provides C with the Single CID Offer for the CID.
* C will believe that mRP can deliver the content. 
* mG will offer to be a payment brokers for mRP.
* C pays the full discovery payment to mG.
* C sends the first micro-payment for content to mG, expecting mG to forward the payment to mRP.
* mRP never sends any content to C.
* When C receives no content it reduces the reputation score for mG and adds mRP to its banned list.
* C asks other Retrieval Gateways for the content. If mG had returned offers from other Retrieval Providers, it could attempt to pursue one of the other offers.

_Analysis_

Retrieval Gateways and Retrieval Providers are long lived entities that have staked money. Damaging their reputation like this will yield small amounts of money by their nefarious activities, but will prevent them from greater gains that could be achieved by obeying the protocol. Additionally, we expect community reporting of bad Retrieval Gateways and bad Retrieval Providers to be promulgated out-of-band (e.g. via Reddit, email, Discord, etc), thus allowing Clients to avoid bad actors using information not processed on the network itself.

## Malicious Retrieval Gateway and Client: DHT Discovery Request Abuse

_Scenario_

A malicious Retrieval Gateway mG operates a malicious Client mC. They target new Retrieval Gateways that start up and have Retrieval Gateway Ids that are adjacent to the malicious Gateway’s Id. The attack is:

* The mC requests a Piece CID via the DHT request that will be close to the malicious Retrieval Gateway’s Id and close to the new Gateway’s Retrieval Gateway Id.
* The initial micro-payment is made to the new Retrieval Gateway. 
* The new Retrieval Gateway requests the Piece CID from mG.
* The new Retrieval Gateway makes the same micro-payment to the mG.
* mG returns a Single CID Offer for the Piece CID to the new Retrieval Gateway.
* The new Retrieval Gateway returns the Single CID Offer to mC.
* mC does NOT pay the larger micropayment.
* The new Retrieval Gateway now has a problem. If they don’t make the larger micro-payment to the malicious Retrieval Gateway, they will perceive they will have reputation loss, so may make the payment anyway. 

_Analysis_

The reason why this scenario is unlikely to happen:

* The malicious Client needs to set-up a payment channel with the new Retrieval Gateway. There will be a cost overhead of having the transaction on the blockchain.
* For the malicious Retrieval Gateway to make much money from this, they would need to have many new Retrieval Gateways set-up with adjacent Retrieval Gateway Ids, which is unlikely. 

## Retrieval Gateway Registration Abuse or Censorship

_Scenario_

A bad actor could determine a region of the Retrieval Gateway Id number space that was sparsely populated. They could repeatedly generate Retrieval Provider Root Signing key pairs until the related Retrieval Gateway Id is in the desired region (recall the Retrieval Gateway Id is the message digest of the Retrieval Provider Root Signing Public Key). 

The malicious actor could register a multitude of Retrieval Gateways in the region. Given the requirement to publish CIDs to the DHT to 16 Retrieval Gateways, having 16 Gateways with sequential Retrieval Gateway Ids would be enough for a malicious actor to “own” the region of the Retrieval Gateway Id number range where only those Gateways would hold the CID.

Alternatively, a bad actor could see some content that they do not wish to be available via the Gateway DHT. The bad actor could generate 16 Retrieval Gateway Ids around the CID they wish to block.

The process would be:

* Retrieval Provider RP publishes a CID offer to the DHT to malicious Retrieval Gateways mG01 to mG16.
* mG01 to mG16 respond with acknowledgement messages for the Offer messages to RP.
* The user who stored the content or a user that knows the content exists could check that the CID was available via the DHT. 
* mG01 to mG16 could choose to respond indicating that no offer was available for the CID. This CID not available response is signed by the Retrieval Gateway.
* The user would request the acknowledgement of CID Offer publication to the DHT for each Retrieval Gateway (which will be mG01 to mG16) from RP using the Get CID Group Publish DHT Acknowledgement Request / Get CID Group Publish DHT Acknowledgement Response messages. 
* For each malicious Retrieval Gateway the user would submit to the Gateway Registration contract:
* The DHT Offer Acknowledgement for the CID
* The signed response indicating no offer is available for the CID.
* The Retrieval Gateways would then be slashed.

_Analysis_

Acknowledging a CID Offer added to the DHT, but then not providing the offer results in the Retrieval Gateway being slashed. Retrieval Gateways will comply with the protocol in order to not be slashed.

A set of malicious Retrieval Gateways are unlikely to know what content is related to a Piece CID. As such, they are unlikely to know ahead of time to not acknowledge a Piece CID when the offer is first published.

The malicious Retrieval Gateways could not return any signed responses to the Clients for CIDs they did not want to provide information for. Owners of the content or other interested parties could see this behaviour and set-up a Gateway with an appropriate Gateway Id to ensure this content is available.

## Combined Retrieval Gateway - Retrieval Provider blocking CIDs from other Providers

_Scenario_

A Retrieval Provider RP1 could operate a Retrieval Gateway G1 (or even a set of Gateways). They might seek to have their content retrieved ahead of their competitors. When they saw CID Offers published (either in the standard mechanism or the DHT mechanism) from other Retrieval Providers for Piece CIDs that they also host, they could:

* They could create a new CID Offer for a Piece CID they host when they see a CID Offer for the same CID from other Retrieval Providers to under-cut the other Retrieval Providers.
* They could refuse to acknowledge CID Offers from other Retrieval Providers for Piece CIDs that they also host. 
* They could acknowledge CID Offers from other Retrieval Providers, but then when requested for CID Offers for a CID, only return their own CID Offers.

_Analysis_

For the first scenario of under-cutting the opposition, this would be good for users as they will get their content for a lower price. This is perceived to be a good thing.

For the second scenario, by not acknowledging the CID Offer from the other Retrieval Providers they would prevent themselves from being slashed. A user will be able to obtain a range of CID Offers by asking multiple Retrieval Gateways controlled by different entities. For the DHT they could ask all 16 Retrieval Gateways that should have the offer for the CID.

For the third scenario, by not signing a response indicating the CID Offer is not available the Retrieval Provider is not risking being slashed. A user will be able to obtain a range of CID Offers by asking multiple Retrieval Gateways controlled by different entities. For the DHT they could ask all 16 Retrieval Gateways that should have the offer for the CID.

If a particular entity owned all Retrieval Gateways for a particular region of the Retrieval Gateway Id number range they could conceivably block Retrieval Providers from offering a certain Piece CID via the DHT. However, the blocked Retrieval Provider could create a Retrieval Gateway with a Retrieval Gateway Id close to the CID (by generating many Retrieval Provider Root Signing key pairs), thus being within the 16 Retrieval Gateway Id range, thus making their CID Offer visible to all users of the DHT. 

[Next: Appendices](appendices.md)