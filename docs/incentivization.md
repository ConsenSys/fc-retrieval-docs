[Back: Reputation System](reputation.md)

# Incentivization Scheme

The incentivization scheme encourages Retrieval Gateways to store and deliver CID Offers for given Piece CIDs. The scheme also slashes Retrieval Gateways that are provably not obeying the protocol.

## Standard CID Request - Response

As described in CID Offers / Standard Approach, a small micro-payment is made by a Retrieval Client in conjunction with a Standard Discovery Request message. The Client then makes a larger payment if the Retrieval Gateway is able to return at least one CID Offer in the Standard Discovery Response message.

## DHT CID Request - Response

As described in DHT Network Approach, a small micro-payment is made by a Retrieval Client in conjunction with a DHT Discovery Request message. The number of Gateways to be checked is specified in this message. The Client then makes a larger payment if the Retrieval Gateway is able to return at least one CID Offer in the DHT Discovery Response message. The larger amount paid depends on the number of Gateways that return CID Offer information.

## DHT Gateway - Gateway Request - Response

As described in DHT Network Approach, a small micro-payment is made by the Retrieval Gateway in conjunction with a DHT Gateway-Gateway Discovery Request message. The calling Gateway then makes a larger payment if the called Retrieval Gateway is able to return at least one CID Offer in the DHT Gateway-Gateway Discovery Response message. 

## Gateway Slashing

All Retrieval Gateways deposit money as part of their on-chain registration. As described in the Retrieval Gateway Registration Abuse section, a Gateway can be slashed if it acknowledges the publication of a CID Offer to the DHT by a Retrieval Provider, but then indicates that no such CID Offer exists.


[Next: Security Considerations](securityconsiderations.md)