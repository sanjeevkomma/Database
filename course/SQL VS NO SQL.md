When should we go for a NoSQL database?
It's when we need to scale, right?

The line between NoSQL and SQL is thin. You can write a NoSQL database on top of an SQL database (Uber Schemaless).

------------------------------------------------

Let's first note the high-level differences:

1. SQL provides constraint satisfaction, isolation levels, and transaction guarantees.
2. SQL tables can be joined at the database instead of the application level.
3. NoSQL databases have built-in sharding, data consensus, and fault tolerance.

------------------------------------------------

Now let's note the similarities:

1. Both SQL and NoSQL can scale. Query speed is dependent more on Isolation levels than database type.
2. Indexing is possible in both SQL and NoSQL tables.

------------------------------------------------

So what are the tradeoffs?

1. NoSQL's lack of constraint satisfaction checks gives fast reads and writes.
2. Joining two NoSQL tables is a tedious process.
3. Scaling NoSQL horizontally is easier because of the in-built coordinator, replication, and routing capabilities.
4. Processing transactions and having constraint checks is easier in SQL.

------------------------------------------------

When should you choose NoSQL over SQL?

1. You are ready to sacrifice transaction capabilities for speed (this is a sensible tradeoff at scale).
2. You sacrifice normalization and joins for speed.
3. You want your database to handle common problems like coordination, replication, routing, etc...

------------------------------------------------

Does this mean SQL can't scale? It CAN.
But what's easier to work with at scale? Usually, NoSQL.
