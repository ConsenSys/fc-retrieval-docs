[Back: Incentivization Scheme](incentivization.md)

# Security Considerations

This section provides advice on how to operate a Retrieval Gateway and Retrieval Provider securely.

## Network Start-up

The network start-up procedure should be (in order):

1. Start-up and register multiple Retrieval Gateways.
1. Start-up Retrieval Providers.
1. Have Retrieval Provider publish CID Offers to the Gateway DHT. These CID Offers should be for all existing Piece CIDs.
1. The network is live once the DHT has been populated with all Piece CID information. At this point new Retrieval Gateways, Retrieval Providers, and Retrieval Clients can be started in any order.

## Protocol Version Upgrade

Messages in this document are exchanged between Retrieval Clients and Retrieval Gateways, between Retrieval Providers and Retrieval Gateways, and between Retrieval Gateways. Each message contains a Protocol Version header and a Protocols Supported header. It seems likely the protocol version number will increase over time, as the protocol is upgraded. This section describes how protocol version upgrades may be safely accomplished.

To operate in the presence of multiple protocol versions: 

* Every message includes a Protocol Version header indicating the version of the protocol used for the current message;
* Every message includes a Protocols Supported header indicating the versions of the protocols it supports (limited to 2).
* Message senders send messages using the last known highest protocol version that both the message receiver and the message sender supports. Message senders send messages using the highest protocol version they support if they have not sent a message to the receiver before.

Receivers have four choices when receiving a message:

1. Respond using the same protocol version as the sender; or
1. Respond with a Protocol Change message if they wish to switch to a different protocol version number that the sender indicated they can accept; or
1. Respond with a Protocol Mismatch message if the two parties do not support any common protocol; or
1. Respond with an Invalid Message message if the message received did not parse in the format of the stated protocol version.

A possible methodology for upgrading the protocol version between two nodes without need for a Protocol Change message is to allow for protocol shifting. That is, a node receiving a response in a higher mutually-supported protocol version should shift to use the version indicated by its partner from that point forward. However, this will introduce protocol complexity (what should the response in v1 of the protocol be to a certain request in v0 of the protocol) and could possibly introduce security issues. The specifics of which messages will be allowed to use this protocol shifting behaviour will be determined when a second version of the protocol is being formalised. 

The existence of new protocol versions are communicated outside the bounds of this system (e.g. via software updates, social media, email and word of mouth). Node operators are encouraged to change their configurations to support new protocol versions to allow their nodes to interoperate with the rest of the network.

## Denial of Service Response

Most denial of service responses may be handled in the following manner:

* Receivers respond with an Invalid Message message if the message received did not parse in the format of the stated protocol version;
* Receivers receiving many requests for nonexistent CIDs from a sender may choose to treat those messages as invalid;
* Receivers receiving many invalid messages from the same sender may choose to stop responding to that sender;
* Receivers receiving many invalid messages from the same sender may choose to reduce its local reputation of that sender.

NB: The above mechanisms do not resolve all possible DOS attack scenarios (e.g. see Retrieval Gateway Registration Abuse, below). However, the following section discusses several attack-specific mitigation opportunities.


[Next: Attacks Analysis](attacksanalysis.md)