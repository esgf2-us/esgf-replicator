# ESGF-NG Replicator
The ESGF-NG Replicator is a service designed to be used by ESGF Data Node operators with the new [ESGF-NG core architecture](https://github.com/ESGF/esgf-roadmap).
* It monitors the ESGF-wide Event Stream.
* When it sees a new ESGF dataset that matches a configured replication policy, it makes a replica of the dataset in configured local storage.
* It updates the configured ESGF STAC Catalogue with information about any replicas it creates.

The design-docs folder contains the following:
* [User Stories](https://github.com/esgf2-us/esgf-replicator/blob/main/design-docs/user-stories.md)
* [Requirements](https://github.com/esgf2-us/esgf-replicator/blob/main/design-docs/requirements.md)
* [Key Design Points, aka Technical Requirements](https://github.com/esgf2-us/esgf-replicator/blob/main/design-docs/key-design-points.md)
* [Open Questions](https://github.com/esgf2-us/esgf-replicator/blob/main/design-docs/open-questions.md)
