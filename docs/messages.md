[Back: Retrieval Gateway Storage and Caching](rgstorageandcaching.md)

# Messages

All messages between different entities in the system are separate, even if the messages contain the same contents. The reason for this is to make upgrade easier. That is, when extra fields need to be added to a message in one context, but not another, having separate messages makes this straightforward, whereas if the same message was reused in different scenarios, adding a field in just one scenario would likely require large amounts of rework.

Currently all messages are statically priced. That is, there is no mechanism to offer message servicing at different prices, or do change the pricing dynamically.

## Common Message Fields

All messages have the following fields. Version numbers range from 0 to 216-1 and thus require two bytes.

Field | Description
------|------------
Protocol Version | Version number used to identify what fields a message contains and the context in which the message has been used. The version number is represented as two bytes.
Protocols Supported | A list of exactly two protocol version numbers supported by the sending node, represented as four bytes. If only one protocol version is supported, the same version number appears in both the first two and last two bytes.
Message Type | Number to be assigned to each message at implementation time.

**Table 2.** Common Message Fields

## Client - Retrieval Gateway Network Establishment

### Client - Retrieval Gateway Establishment Challenge 

**Description:** Used to check that the Retrieval Gateway Id / public key for a Retrieval Gateway at a certain IP address matches the information in the Retrieval Gateway Registration Built-in Actor; plus to check the latency between the Client and Gateway.

**Parties:** Sent from Client to Retrieval Gateway.

**Payments:** None

Fields | Description
-------|------------
Challenge | A 256 bit random number. If messages are to be sent, then use the following algorithm:
SEED = 256 bit random number
Challenge = Message Digest(SEED, Retrieval Gateway Id)
TTL | Unix time after which this message should be discarded. Typically set to a small number of seconds after the message is created.

**Table 3.** Client - Retrieval Gateway Establishment Challenge message specific fields

### Client - Retrieval Gateway Establishment Response

**Description:** Response to Client-Retrieval Gateway Establishment Challenge message.

**Parties:** Sent from Retrieval Gateway to Client.

**Payments:** None

Fields | Description
-------|------------
Challenge | Challenge sent by Client.
Signature | Signature across challenge, using Retrieval Gateway Root Signing Key.

**Table 4.** Client - Retrieval Gateway Establishment Response message specific fields

## CID Group Publication

### CID Group Publish

**Description:** Used to publish a set of CIDs that will be offered at a set price, expiry time and QoS. The set of CIDs can be ones that are all created at the same time or are all renewing at the same time. These CID sets are published to Retrieval Gateways that want to know about all content from a Retrieval Provider. 

**Parties:** From a Retrieval Provider to a Retrieval Gateway.

**Payments:** None.

Fields | Description
-------|------------
Nonce | Random number.
Provider Id | Identifier of Retrieval Provider
Price per Byte | Price at which the content can be returned.
Expiry date | Unix time when the offer will expire.
QoS Metric | Latency to first byte from first micro-payment.
Signature | Retrieval Provider’s signature across:
Provider Id, Price per Byte, Expiry date, QoS Metric, and the Merkle Root of the balanced, zero filled, Merkle Tree created from the array of Piece CIDs, where the Piece CIDs are the leaves of the tree.
Piece CID Array | Array of between 1 and 128 Piece CIDs.

**Table 5.** CID Group Publish message specific fields

### CID Group Publish to DHT

**Description:** The same as a CID Group Publish message, except the set of CIDs are CIDs that are numerically close to a Retrieval Gateway Id. These CID sets are published to Retrieval Gateways to populate the DHT. Having a separate message is important as CID Group Publish DHT messages are needed to acknowledge these messages, and not the CID Group Publish messages.

Fields | Description
-------|------------
Nonce | Random number.
Provider Id | Identifier of Retrieval Provider
Num Offers | Number of Single CID Offers
Array of: | 
Price per Byte | Price at which the content can be returned.
Expiry date | Unix time when the offer will expire.
QoS Metric | Latency to first byte from first micro-payment.
Signature | Retrieval Provider’s signature across:
Provider Id, Price per Byte, Expiry date, QoS Metric, and the Piece CID.
Piece CID | Piece CID.

**Table 6.** CID Group Publish to DHT message specific fields

### CID Group Publish Acknowledgement

**Description:** Used to send a signed acknowledgement of the CID Group Publish DHT message.

**Parties:** From a Retrieval Gateway to a Retrieval Provider.

**Payments:** None.

Fields | Description
-------|------------
Nonce | Nonce from CID Group Publish message
Signature | Signature across the CID Group Publish message

**Table 7.** CID Group Publish Acknowledgement message specific fields

## DHT Establishment

### List of Single CID Group Publish Request

**Description:** Used by a Retrieval Gateway at Gateway start-up to request a set of Single CID Offers from a Retrieval Provider.

**Parties:** From a Retrieval Gateway to a Retrieval Provider.

**Payments:** None.

Fields | Description
-------|------------
Retrieval Gateway Id | Retrieval Gateway Id of the requesting Gateway
CID Min | Lower bound of requested Single CID Offers
CID Max | Upper bound of requested Single CID Offers
Block Hash | Block hash of the block that the transaction registering the Retrieval Gateway is in.
Transaction Receipt | Transaction Receipt containing a Retrieval GatewayRegister event.
Merkle Proof | Merkle Proof proving that the Transaction Receipt is part of the block designated by the block hash.

**Table 8.** DHT Establishment message specific fields

### List of Single CID Group Publish Response

**Description:** Sent in response to List of Single CID Group Publish Request.


**Parties:** From a Retrieval Provider to a Retrieval Gateway.

**Payments:** None.

**Message Fields:**
Array of CID Group Publish to DHT messages. The number returned could be limited to, say 100.

### List of Single CID Group Publish Response Acknowledgement

**Description:** Sent in response to List of Single CID Group Publish Response.

**Parties:** From a Retrieval Gateway to Retrieval Provider.

**Payments:** None.

**Message Fields:**
Array of CID Group Publish to DHT Acknowledgement messages. The number returned matches the number of Single CID Groups in the Response message.

## CID Offer Requests

### Standard Discovery Request

**Description:** Used to determine which Provider(s) can serve content for a Piece CID. 

**Parties:** Sent from Client to Retrieval Gateway.

**Payments:** 1 coin for the initial request. 99 coins more if one or more CID Group Offer or Single CID Offer are returned. 

Fields | Description
-------|------------
Piece CID | Piece CID being requested.
Nonce | Random value to guard against replay attacks. Note nonces need only be kept until the message TTL expires.
TTL | Unix time after which this message should be discarded. Typically set to a small number of seconds after the message is created.

**Table 9.** DHT Establishment message specific fields

### DHT Discovery Request

**Description:** Request a Retrieval Gateway use the DHT to return which Provider(s) can serve content for a Piece CID. 

**Parties:** Sent from Client to Retrieval Gateway (to initiate a DHT request).

**Payments:** Num DHT x (10 coins if no CID Group Offer or Single CID Offer is returned. 190 additional coins if one or more CID Group Offer or Single CID Offer are returned.)

Fields | Description
-------|------------
Piece CID | Piece CID being requested.
Nonce | Random value to guard against replay attacks. Note nonces need only be kept until the message TTL expires.
TTL | Unix time after which this message should be discarded. Typically set to a small number of minutes after the message is created.
Num DHT | The number of Retrieval Gateways the Gateway should contact to try to find the CID offer. The payment must match this. 
Incremental Results | Indicates whether results should be return incrementally or all in one message.

**Table 10.** DHT Discovery Request specific fields

### DHT Gateway-Gateway Discovery Request

**Description:** Request a Retrieval Gateway return information for a Piece CID based on their part of the DHT. 

**Parties:** Sent from Retrieval Gateway to Retrieval Gateway to forward a DHT request to a Gateway which should have the Piece CID.

**Payments:** 10 coins if no CID Group Offer or Single CID Offer is returned. 190 additional coins if one or more CID Group Offer or Single CID Offer are returned.

Fields | Description
-------|------------
Piece CID | From the DHT Discovery Request message.
Nonce | From the DHT Discovery Request message.
TTL | From the DHT Discovery Request message.

**Table 11.** DHT Gateway-Gateway Discovery Request message specific fields

### Standard Discovery Response

**Description:** Sent in response to the Standard Discovery Request message. Used to indicate which Provider(s) can serve content for a Piece CID. 

Fields | Description
-------|------------
Piece CID | Piece CID being requested.
Nonce | Nonce from the request
Found | Indicator that the CID was not found.
Retrieval Gateway Signature | Signature across the rest of the message. When signing, this field is set to zero.
Array of CID Group Information (only if found = true): | 
Provider Id | Identifier of Retrieval Provider
Price per Byte | Price at which the content can be returned.
Expiry date | Unix time when the offer will expire.
QoS Metric | Latency to first byte from first micro-payment.
Provider Signature | Retrieval Provider’s signature across: Provider Id, Price per Byte, Expiry date, QoS Metric, and the Merkle Root.
Merkle Proof | Intermediate nodes of the Merkle Tree required to combine with the CID to generate the Merkle Root. 
Funded Payment Channel | The Retrieval Gateway has a funded payment channel with the Retrieval Provider.

**Table 12.** Standard Discovery Response message specific fields

### DHT Gateway-Gateway Discovery Response

**Description:** Sent in response to the DHT Gateway-Gateway Discovery Request message. Used to indicate which Retrieval Provider(s) can serve content for a Piece CID. 

**Message Fields:**
Contains the same fields as the Standard Discovery Response message.

### DHT Discovery Response

**Description:** Sent in response to the DHT Discovery Request message. Used to indicate which Provider(s) can serve content for a Piece CID. 

**Message Fields:**
An array of DHT Gateway-Gateway Discovery Response messages and for uncontactable Gateways:

Fields | Description
-------|------------
Retrieval Gateway Id | The Retrieval Gateway that was uncontactable.
Nonce | Nonce from the request

**Table 13.** DHT Discovery Response message specific fields

## Gathering Proofs to Prevent Sybil Attacks on DHT

### Get CID Group Publish DHT Acknowledgement Request

**Description:** Used to request the latest signed acknowledgement of a CID Group Publish DHT message for a certain Retrieval Provider - Retrieval Gateway pair. 

**Parties:** From a Client to a Provider.

**Payments:** None.

Fields | Description
-------|------------
Piece CID | Piece CID to request the acknowledgement for.
Retrieval Gateway Id | Retrieval Gateway Id to get the acknowledgement for.

**Table 14.**  Get CID Group Publish DHT Acknowledgment Request message specific fields

### Get CID Group Publish DHT Acknowledgement Response

**Description:** Used to request the latest signed acknowledgement of a CID Group Publish DHT message for a certain Retrieval Provider - Retrieval Gateway pair. 

**Parties:** From a Provider to a Client.

**Payments:** None.

Fields | Description
-------|------------
Piece CID | Piece CID to request the acknowledgement for.
Retrieval Gateway Id | Retrieval Gateway Id that the acknowledgement is for.
Found | Indication if there was such an acknowledgement.
CID Group Publish to DHT | Fields from the CID Group Publish to DHT message.
CID Group Publish to DHT Acknowledgement | Fields from the CID Group Publish to DHT Acknowledgement message.

**Table 15.** Get CID Group Publish DHT Acknowledgment Response message specific fields

## Protocol Housekeeping

Protocol housekeeping messages are anticipated to be used relatively rarely, but provide mechanisms for handling protocol upgrades, protocol mismatches and malformed messages.

### Protocol Change

**Description:** Used to request the receiver shift to a given protocol number. Well-behaved nodes will use this message solely upon receipt of a message from a sender that indicates the protocol version numbers accepted by the sender, and return a mutually-supported protocol version number from the sender’s list.

There are two usage scenarios for this message:

* A node receives a message in a new protocol version that it doesn’t support. It sees that the sender indicates that it supports an older version of the protocol that this node does support. This node sends a Protocol Change message to request the sender resend the request using the older version of the protocol.
* Two nodes have an existing relationship. The sender has upgraded to the new version of the protocol. As the receiver has not upgraded, the sender remembers the version of the protocol the receiver supports, and continues to send messages using the old version of the protocol. When the receiver upgrades and can support the new version of the protocol, they need to inform the sender. They do this by responding with a Protocol Change message, indicating that they have detected that both themselves as receiver and the sender support a new version of the protocol.

**Parties:** From any node to any other node.

**Payments:** None.

Fields | Description
-------|------------
Desired Protocol | A protocol version number, in two bytes.

**Table 16.** Protocol Change message specific fields

### Protocol Mismatch

**Description:** Used to indicate to another node that the two parties do not support any common protocol versions.

**Parties:** From any node to any other node.

**Payments:** None.

**Message Fields:**
None

### Invalid Message

**Description:** Used to indicate to another node that a message received could not be parsed using the message formats indicated by the sender’s Protocol Version field.

Note that usage of this message is enabled when Retrieval Gateways are in a “debug mode”, but might be disabled in production environment configurations. Doing this helps prevent DoS and other attacks.

**Parties:** From any node to any other node.

**Payments:** None.

**Message Fields:**
None

### Insufficient Funds

**Description:** Used by a Retrieval Provider or Retrieval Gateway to indicate to a Retrieval Gateway or Retrieval Client that the payment channel between the Provider and Gateway, Gateway and Client or Gateway and Gateway does not have sufficient funds to complete a requested operation.

**Parties:** From a Retrieval Provider to a Retrieval Gateway.

**Payments:** None.

Fields | Description
-------|------------
Payment Channel ID | A payment channel identifier

**Table 19.** Insufficient Funds message specific fields

## Admin API

Administrative functions for Retrieval Gateways and Retrieval Providers are provided via the Admin API. 

### getReputationChallenge

**Description:** Used to request the reputation of a Retrieval Client as held by a Retrieval Gateway. It allows (e.g.) a client to check the state of its own reputation.

**Parties:** From a Retrieval Client to a Retrieval Gateway

**Payments:** None.

Fields | Description
-------|------------
ClientID | A client identifier

**Table 20.** getReputationChallenge message specific fields

### getReputationResponse

**Description:** A response to a getReputationChallenge by a Retrieval Gateway to a Retrieval Client.

**Parties:** From a Retrieval Gateway to a Retrieval Client

**Payments:** None.

Fields | Description
-------|------------
Reputation | A reputation number

**Table 21.** getReputationResponse message specific fields

[Next: Reputation System](reputation.md)