[Back: Overview](overview.md)

# Terminology

Term | Definition
-----|-----------
CID Group Offer | Signed offer by a Retrieval Provider to deliver content based on a Piece CID for a certain price and QoS until a specified expiry date. The offer applies to all CIDs in the CID Group Offer.
Content Identifier (CID) | See https://github.com/multiformats/cid 
Content Discovery | The means by which a Retrieval Client may discover which nodes are holding data related to a given CID.
DHT Span | The region of the DHT Ring of Piece CIDs that a Gateway is responsible for or the set of Gateways that a Single CID Offer for a Piece CID should be published to, depending on your perspective.
Node Discovery | The means by which a Filecoin node finds a sufficient number of other nodes to participate in a retrieval process.
Piece CID | A CID that serves as the top-level identifier for a defined bit of content (e.g. a file)
Retrieval Client | Filecoin software acting on behalf of a user (e.g. to request the storage or retrieval of documents).
Retrieval Gateway | A (proposed) Filecoin node that brokers retrieval of user files with one or more Retrieval Providers and Storage Miners.
Retrieval Provider | A Filecoin node that either provides user files upon a retrieval request (from its local cache) or brokers retrieval via one or more Storage Miners.
Single CID Offer | Signed offer by a Retrieval Provider to deliver content based on a Piece CID for a certain price and QoS until a specified expiry date. The offer applies to a single CID.
Storage Miner | A Filecoin node that provides storage of user files for a fee and provides those files upon a retrieval request for another fee.

[Next: Core Architecture](corearchitecture.md)