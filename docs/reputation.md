[Back: Messages](messages.md)

# Reputation System

The reputation system allows nodes to track their perception of other nodes in the system. This allows each node to determine whether it should use a given node in the system or preferentially use another node in the system. The sections below describe the reputation system from perspective of specific types of nodes in the system.

## Retrieval Clients 

There is no interaction between Retrieval Clients. As such, no reputation score is kept by Retrieval Clients of other Retrieval Clients.

### Retrieval Gateways

Retrieval Clients keep a track of the reputation of Retrieval Gateways to know which Gateways are most likely to be able to respond to their requests.

Retrieval Clients keep a track of the latency between themselves and Retrieval Gateways. Though not directly a reputation score, this measure can be used by Retrieval Clients as part of the decision process on which Retrieval Gateways to use.

**Reputation Establishment:** The initial *Client - Retrieval Gateway Establishment Challenge / Client - Retrieval Gateway Establishment Response* exchange is used to set the initial reputation value. 

**Action on Bad Reputation:** If the reputation for a Retrieval Gateway is less than or equal to zero the Retrieval Client should stop using the Retrieval Gateway. 

**Reputation Healing:** There is no automatic mechanism for a Retrieval Gateway’s bad reputation to be healed from the Retrieval Client’s perspective. A manual process could be used to reset a Retrieval Gateway’s reputation.

**Reputation Changes:**

Message | Action | Reputation Change
--------|--------|------------------
Client - Retrieval Gateway Establishment Challenge / Client - Retrieval Gateway Establishment Response | Response prior to TTL expiry | +1000
-|\sNo response prior to TTL expiry, challenge sent in response does not match challenge in request, or signature of response does not verify. | -1000
Standard Discovery Request / Standard Discovery Response | Response with one or more CID Offers prior to TTL expiry. For one or more of the CID Offers, the Retrieval Gateway indicates it has a funded payment channel with the Retrieval Provider indicated in the CID Offer. | +100
-|\sResponse with one or more CID Offers prior to TTL expiry. One or more CID Offers are from Retrieval Providers that the Retrieval Client has a non-zero reputation score with, or has never used. | +50
-|\sResponse with one or more CID Offers prior to TTL expiry. All CID Offers are from Retrieval Providers that the Retrieval Client has a bad (0) reputation score with. | +10
-|\sResponse with no CID Offers prior to TTL expiry | -10
-|\sNo response prior to TTL expiry | -100
DHT Discovery Request / DHT Discovery Response | Response with one or more CID Offers prior to TTL expiry. For one or more of the CID Offers, the Retrieval Gateway indicates it has a funded payment channel with the Retrieval Provider indicated in the CID Offer. | +100
-|\sResponse with one or more CID Offers prior to TTL expiry. | +50
-|\sResponse with no CID Offers prior to TTL expiry | -10
-|\sNo response prior to TTL expiry | -100
Micro-payment for content via Gateway | Content delivered in response to micro-payment via Gateway. Note that there are likely to be many micro-payments during content retrieval. | +1
-|\sNo content delivered in response to micro-payment via Gateway. | -100
Invalid message received |  A response message was invalid. | -100
Gateway uncontactable | A TCP connection can not be established with the the Gateway | -10

**Table 20.** Retrieval Client’s reputation score changes for Retrieval Gateways

### Retrieval Providers

Retrieval Clients keep a track of the reputation of Retrieval Provider to know which Providers are most likely to honour their CID Offers and deliver their content.

Retrieval Clients request content from Retrieval Providers based on CID Offers. They establish payment channels either directly or via Retrieval Gateways.

**Reputation Establishment:** Any Retrieval Providers that a Retrieval Client has no reputation score with are deemed to have the initial score of 1000. 

**Action on Bad Reputation:** If the reputation for a Retrieval Provider is less than or equal to zero the Retrieval Client should stop using the Retrieval Provider.

**Reputation Healing:** There is no automated way of healing a bad reputation (reputation less than zero). A manual intervention could be used if this type of reset is deemed desirable. 

**Reputation Changes:**
Message | Action | Reputation Change
--------|--------|------------------
Content retrieval with payment channel directly with Retrieval Provider | Content delivered in response to micro-payment. Note that there are likely to be many micro-payments during content retrieval. | +1
-|\sNo content delivered in response to micro-payment. | -350
Micro-payment for content via Gateway | Content delivered in response to micro-payment via Gateway. Note that there are likely to be many micro-payments during content retrieval. | +1
-|\sNo content delivered in response to micro-payment via Gateway. | -100
Get CID Group Publish DHT Acknowledgement Request / Get CID Group Publish DHT Acknowledgement Response | Response received within TTL | +50
-|\sNo response received within TTL | -50
Invalid message received | A response message was invalid. | -100
Retrieval Provider uncontactable | A TCP connection can not be established with the Retrieval Provider | -100

**Table 21.** Retrieval Client’s reputation score changes for Retrieval Providers

## Retrieval Gateways 

### Retrieval Clients

Retrieval Gateways keep a track of the reputation of Retrieval Clients to determine whether they should respond to requests from the Clients. In addition to the reputation system, the Retrieval Gateways keep a track of funds deposited into payment channels. With the exception of the challenge - response messages, Retrieval Gateways only respond to requests from Retrieval Clients that have a funded payment channel with the Retrieval Gateway.

Retrieval Clients use the Client - Retrieval Gateway Establishment Challenge / Client - Retrieval Gateway Establishment Response messages to ensure a Retrieval Gateway is not being spoofed, prior to depositing funds into a payment channel. 

**Reputation Establishment:** Retrieval Clients automatically have a reputation of 10. However, CID discovery requests are not acted upon until the Retrieval Client funds a payment channel. Note that the minimum amount of funds that need to be deposited to cause reputation establishment is to be determined prior to the Secondary Retrieval Market System going live. 

**Action on Bad Reputation:** If a Retrieval Client’s reputation is reduced to zero or less, the Retrieval Gateway stops accepting requests from the Client, banning the client. 

**Reputation Healing:** After a period of time, say a day, the Retrieval Gateway could reset the Retrieval Client’s reputation to 10. For subsequent times when the Client is banned, the wait period for re-enabling the Client’s usage could be exponentially backed-off.

The Retrieval Gateway should observe the blockchain. Requests from a Retrieval Client should be blocked if the payment channel with the Gateway is defunded. The Retrieval Gateway should return an Insufficient Funds message as a response to requests in this situation.

**Reputation Changes:**
Message | Action | Reputation Change
--------|--------|------------------
Client - Retrieval Gateway Establishment Challenge / Client - Retrieval Gateway Establishment Response | Receive request and respond. Note that -1 reputation in conjunction with an initial reputation of 10 means that a Retrieval Client could call this function 10 times prior to funding a payment channel before they would be banned. | -1
On-chain payment into payment channel | On-chain deposit detected. | +1000
Standard Discovery Request / Standard Discovery Response | Response with one or more CID Offers. Initial payment and final payment made. | +10
-|\sResponse with no CID Offers. Initial payment payment made. | +1
-|\sResponse with one or more CID Offers. Response message sent after one second prior to TTL expiry. Initial payment payment made. | +1
-|\sResponse with one or more CID Offers. Response message sent prior to one second prior to TTL expiry. Initial payment payment made but final payment not paid. | -100
DHT Discovery Request / DHT Discovery Response | Response with one or more CID Offers from one or more Gateways. Initial payment and final payment made. | +10
-|\sResponse with no CID Offers. Initial payment made. | +1
-|\sResponse with one or more CID Offers. Response message sent after one second prior to TTL expiry. Initial payment payment made. | +1
-|\sResponse with one or more CID Offers. Response message sent prior to one second prior to TTL expiry. Initial payment payment made but final payments not paid. | -300
Micro-payment for content via Gateway | Micro-payment paid for content via Gateway. Note that there will be many micro-payments during content retrieval. | +1
Invalid message requiring Invalid Message | Sent in response to invalid message. | -10

**Table 22.** Retrieval Gateway’s reputation score changes for Retrieval Clients

### Retrieval Gateways

Retrieval Gateway to Gateway reputation is used to determine which other Gateways a Gateway should prioritise to use when doing DHT look-ups.

**Reputation Establishment:** Retrieval Gateways that have not been contacted by a Retrieval Gateway have an initial reputation of 1000. 

**Action on Bad Reputation:** Retrieval Gateways do not use Retrieval Gateways that have a reputation of zero or less. Retrieval Gateways refuse connections from Retrieval Gateways that have a reputation of zero or less.

**Reputation Healing:** It may be desirable to “heal” bad reputations. A possible methodology for doing this would be to allow for a manual “reset” of a Gateway’s reputation.

**Reputation Changes:**

Table 23 shows the reputation scoring from the perspective of Retrieval Gateway making request. Table 24 shows the reputation scoring from the perspective of Retrieval Gateway receiving the request.

Message | Action | Reputation Change
--------|--------|------------------
DHT Gateway-Gateway Discovery Request / DHT Gateway-Gateway Discovery Response | Response with one or more CID Offers prior to TTL expiry. | +50
-|\sResponse with no CID Offers prior to TTL expiry | -10
-|\sNo response prior to TTL expiry | -100
Invalid message received | If an invalid response is received from the Gateway. | -200
Uncontactable | A TCP connection can not be established with the Retrieval Gateway | -350

**Table 23.** Retrieval Gateway’s reputation score changes for Retrieval Gateways (from the perspective of the Gateway making the request)



Message | Action | Reputation Change
--------|--------|------------------
DHT Gateway-Gateway Discovery Request / DHT Gateway-Gateway Discovery Response | Request is for a valid Piece CID prior to the TTL expiry | +20
-|\sRequest is received after the TTL expiry | -10
-|\sRequest is for an invalid Piece CID | -10
Invalid message received | If an invalid response is received from the Gateway. | -200
Uncontactable | A TCP connection can not be established with the Retrieval Gateway | -350

**Table 24.** Retrieval Gateway’s reputation score changes for Retrieval Gateways (from the perspective of the Gateway receiving the request)

### Retrieval Providers

Gateways use this reputation system to determine whether they should host Standard CID Offers from Retrieval Providers. 

**Reputation Establishment:** The reputation starts off at +1000, when the Retrieval Provider responds to the List of Single CID Group Publish request message. 

**Action on Bad Reputation:** When the reputation is less than zero, the Retrieval Gateway should stop hosting Standard CID Offers from the Retrieval Provider. 

**Reputation Healing:** The reputation’s minimum value is -1000. The Retrieval Provider’s reputation will increase above zero if there are enough DHT CID Offer requests. In this case, the Retrieval Gateway should consider accepting Standard CID Offers from the Retrieval Provider again if this occurs.

**Reputation Changes:** The reputation then goes up if Retrieval Clients request CID Offer information and the Retrieval Provider publishes CID Offer information. Reputation goes down if Retrieval Clients are not interested in the content supplied by a Retrieval Provider. 

Message | Action | Reputation Change
--------|--------|------------------
List of Single CID Group Publish Request / List of Single CID Group Publish Response / List of Single CID Group Publish Response Acknowledgement | Response message is returned in response to request | +1000
-|\sNo response message is returned in response to request | 0
CID Group Publish | A CID Group Publish message is received | +0
CID Group Publish to DHT / CID Group Publish Acknowledgement | A CID Group Publish to DHT is received | +0
Detecting Retrieval Providers not delivering content | Payments proxying through Gateway for content | +1
-|\sPayments proxying through Gateway for content stop after first payment | -10
A Retrieval Client has requested CID Offer for Piece CID published using standard publishing | Each time a CID Offer is requested that was published by the Retrieval Provider with standard publishing | +3
-|\sEach time a CID Offer is requested that was published by the Retrieval Provider with DHT publishing, and this Gateway has the CID Offer in its cache | +3
-|\sEach time a CID Offer is requested that was published by the Retrieval Provider with DHT publishing, and the CID Offer is being fetched from a remote Gateway via DHT Discovery | +3
-|\sNo requests for Piece CIDs hosted by this Retrieval Provider in the past 5 minutes | -1

**Table 25.** Retrieval Gateway’s reputation score changes for Retrieval Providers

## Retrieval Providers

There is no interaction between Retrieval Providers. As such, there is no reputation system between Retrieval Providers.

### Retrieval Client

At present, the authors do not see a strong need for the Retrieval Providers to maintain a reputation metric for Retrieval Clients. This section describes the interactions that could be used to form a reputation if a need for such a reputation eventuates.

What if Clients attempt to cheat by failing to make payment for the last portion of a piece of content? Clients are not expected to have payment channels established with individual Retrieval Providers within the secondary retrieval market. If a Client chooses to establish a payment channel with a Retrieval Provider, they will be operating within the confines of the primary retrieval system and its reputation system. In the secondary retrieval market, payments by Clients transit either Retrieval Gateways or Payment Brokers. Therefore, the Client’s reputation may suffer at the Retrieval Gateways or Payment Brokers, not at the Retrieval Providers.

Message | Action | Reputation Change
--------|--------|------------------
Content retrieval - Client payment channel direct | Payment channel funded | +1000
-|\sMicro-payment paid for content | A range of possibilities from +0 to perhaps +1. Increasing reputation rapidly via many transactions may have unintended consequences.
-|\sStop payment part way through streaming content. | -10
Get CID Group Publish DHT Acknowledgement Request / Get CID Group Publish DHT Acknowledgement Response | Request a CID Group DHT Publication Acknowledgement | Increase reputation

**Table 26.** Possible Retrieval Provider’s reputation score changes for Retrieval Clients (not currently proposed for implementation)

### Retrieval Gateways

At present, the authors do not see a need for the Retrieval Providers to maintain a reputation metric for Retrieval Gateways. This section describes the interactions that could be used to form a reputation if a need for such a reputation eventuates.

Message | Action | Reputation Change
--------|--------|------------------
Content retrieval - payment channel via Gateway | Micro-payment paid for content | Increase reputation
-|\sStop payment part way through streaming content. | Decrease reputation
Get CID Group Publish DHT Acknowledgement Request / Get CID Group Publish DHT Acknowledgement Response | Acknowledge Response received | Increase reputation
-|\sAcknowledge Response not received | Decrease reputation substantially as this indicates the Gateway is not participating in the DHT properly.

**Table 27.** Possible Retrieval Provider’s reputation score changes for Retrieval Gateways (not currently proposed for implementation)

[Next: Incentivization Scheme](incentivization.md)
