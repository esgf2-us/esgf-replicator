# Key Design Points for ESGF-NG Replicator

1. The design should provide a way to configure new types of local storage (besides a Globus collection).
2. The design should provide a way to add support for new data replication methods (Globus Transfer, anonymous HTTPS, others).
3. The design should provide a way to add support for new authentication methods with the STAC Transaction API (Globus, EGI Check-in).

Maybe:
4. The design should provide ways to extend the flexibility of replication actions. (E.g., replicas can be stored in different places determined by metadata criteria.)
