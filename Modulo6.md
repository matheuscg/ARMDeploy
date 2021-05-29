# Modulo 6 Cosmos DB

* Very fast sub 10ms latency guaranteed
* Multiplus types
    * Core SQL (JSON)
    * MongoDB
    * Cassandra
    * Azure Table
    * Gremlin (graph)
* Free tier (400 RU/s and 5 GB)
* World Replication

# Default Consistency

1. Strong (Replicate data across all regions)
1. Bounded Staleness (Lag replication across regions, preserve order)
1. Session (Defaut)
1. Consistent Prefix (Preserve order, but no garantee time)
1. Eventual (Replicate without preserve order)

# Cosmo DB Trigger

* Any change on the collection trigger a function
* Functions Azure CosmoDB Trigger