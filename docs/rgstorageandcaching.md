[Back: Retrieval Client Content Retrieval](rccontentretrieval.md)

# Retrieval Gateway Storage and Caching

## CID Group Offer Storage in Retrieval Gateway

When a CID Group Offer is received the Retrieval Gateway needs to update CID information in the following way:

* Retrieval Gateways would update their map of CID to Retrieval Provider(s) information, replacing existing Retrieval Provider information if:
  * The information was signed by the same Retrieval Provider.
  * The information indicates the same or a later expiration date **AND** the price is the same or lower.
  * If the new information indicates an increased price, then the Retrieval Gateway should keep both the old and the new information.
  * If the new information indicates a decreased price, but an earlier expiration date, then the Retrieval Gateway should keep both the old and the new information.

[Next: Messages](messages.md)