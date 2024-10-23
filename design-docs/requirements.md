# Requirements for ESGF-NG Replicator

1. The Replicator must be able to create replicas of datasets in a Globus collection.
   * We invite others to add support for other storage configurations
2. The Replicator must be able to transfer dataset files from remote Globus collections (as Globus Transfer requests)
   * We invite others to add support for other data access methods
3. The Replicator must be able to subscribe to topics on the ESGF Event Stream.
4. The Replicator must be able to update one of the existing ESGF STAC Catalogues with new replica info when a local replica is created.
   * Q: What happens when there’s an update to a dataset that we previously replicated?
   * Q: What happens when there’s a retraction on a dataset that we previously replicated?
   * NOTE: Globus MVP only needs to support the West STAC Catalog. We invite others to add support for the East STAC Catalog.
5. The Replicator must provide a way for the data node operator to put bounds on how much and/or when data transfer is performed.
   * Need to get input about this. Maybe we should offer some obvious/easy ones and let others request what they need later?
