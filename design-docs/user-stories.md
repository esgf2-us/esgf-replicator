# User Stories for the ESGF-NG Replicator

## As a data node operator, I need to deploy an ESGF Replicator for my data node.

I expect the experience to be something like the following:
1. Deploy the ESGF Replicator on a host system.
2. Register as a client of the ESGF Event Stream & configure my deployment to use credentials.
3. Register as a client of one of the ESGF STAC Catalogs (either East or West) and configure my deployment to use credentials.
4. Configure where my local storage is and give permissions to copy things there.
5. Configure a “profile” of datasets I want replicated on my data node.
   (We need to fill in details about what kinds of matching data node operators need.)
6. Configure how replication tasks should be "batched." (Possibilities: frequency of runs, batch size(s), max delay before something new gets replicated, etc???)
7. Configure limits on storage use. (Possibilities: cap on storage utilization, warning thresholds, etc???)

## As a data node operator, I need to view recent activity in my Replicator.

I expect this to be log of some form.

## As a data node operator, I need to check the current status of my Replicator.

## As a data node operator, I need to change the configuration of my Replicator.

## As a data node operator, I need to get statistics about how many datasets have been replicated by my Replicator.

I expect the stats to include things like:
* How many datasets have been replicated
* How much data has been replicated (by volume, GBs/TBs/PBs)
* Subtotals by time periods (e.g, today, this month, this year, all time)
* Maybe subtotals by profile matches? (If the configuration of things to be replicated is divided into subsets--e.g., by ESGF project--subtotals would also be given for each subset.)
