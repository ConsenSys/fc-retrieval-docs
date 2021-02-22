[Back: Core Architecture](corearchitecture.md)

# Offers

Retrieval Providers offer to provide content at fixed prices and QoS. These offers are used by Retrieval Gateways to prove to Retrieval Clients that a Retrieval Provider has offered to deliver content for a certain Piece CID at a certain price, and hence the Retrieval Provider should be paid. These offers are used by Retrieval Clients to determine the best offer.

The offers take two forms: CID Group Offers for offers that cover more than one CID and Single CID Offers that cover a single CID.

## CID Offer Information

CID Group Offers and Single CID Offers have the following offer information:

* Price per  byte.
* Expiry date.
* Quality of Service metric

If a Retrieval Provider wished to do dynamic pricing, they could issue multiple CID Group Offers for the same set of CIDs for different prices and different expiry dates.

The expiry date does not need to be the same as the storage date agreed in a storage contract. Having an earlier date would allow the Retrieval Provider to increase the price of retrieval.

Notes on QoS metrics:

*Latency and Effective Retrieval Speed (min(storage retrieval bps, network bps)) sound appropriate but…. How do you present meaningful numbers, given you won’t know where the Retrieval Client is in the network relative to Retrieval Provider.
* Could a metric be latency from the first micro-payment arriving at the Retrieval Provider to when the first piece is put onto the wire? This is at least under Retrieval Provider control. However, there will be variable latency between a Client and a Provider. As such, this measure is going to be impossible to prove. That is, Providers could cheat, offering unachievable QoS metrics. 

## Single CID Offer

A Single CID Offer contains the following:

* Piece CID
* CID Offer Information
* Retrieval Provider’s Signature

The signature is across the Piece CID and the CID Offer Information. 

Note that the Retrieval Provider’s Id is derivable from the signature.

## CID Group Offer

All Piece CIDs in a CID Group Offer share the same CID Offer Information. A CID Group Offer contains the following:

* Array of Piece CIDs
* CID Offer Information
* Retrieval Provider’s Signature

The Piece CIDs are arranged as leaves of a binary Merkle Tree. The tree is made to be balanced by zero filling as needed. The Piece CIDs can be deemed to already be message digested, and hence leaves do not need to be message digested. The Retrieval Provider calculates the CID Group Merkle Root. 

The signature is across the CID Offer Information and the Merkle Root.

[Next: Retrieval Gateway DHT Network](dhtnetwork.md)
