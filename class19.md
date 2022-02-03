# El Reading Notes of the 401 Variety

## Class 19 reading notes

### El Questions

#### 1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server.

- They all happen to use that fancy WRRC, isn't that neat?

#### 2. List the AWS Database offerings and talk about the pros and cons of each.

**Amazon Aurora, RDS, Redshift are relational:**

- Traditional applications, enterprise resource planning, customer relationship management ecommerce.

**Amazon DynamoDB uses key-value:**

- High-traffic web applications, ecommerce systems, gaming applications.

**Amazon ElastiCache, MemoryDB for Redis use in-memory:**

- Caching, session management, gaming leaderboards, geospatial applications.

**Amazon DocumentDB for Document:**

- Content management, catalogs, user profiles.

**Amazon Keyspaces for wide Column:**

- High-scale industrial apps for equipment maintenance, fleet management, and route optimization.

**Amazon Neptune with graph:**

- Fraud detection, social networking, recommendation engine.

**Amazon Timestream time series:**

- Internet of Things (IoT) applications, DevOps, industrial telemetry.
Amazon LedgerDB for ledger: Systems of record, supply chain, registrations, banking transactions.

#### 3. What’s the difference between a FIFO and a standard queue?.

- Standard queues provide delivery, at least once. Meaning, each message is delivered at least once, make sense?

- FIFO queues provide processing exactly once. Meaning, each message is delivered *exactly* once and will remain available until the consumer processes it and deletes it. Duplicates **are not** introduced into the queue.

#### 4. How can the server be assured a message was properly received?

- Use AWS SQS with a FIFO queue.

### Document the following Vocabulary Terms

**Serverless API**

> Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral, and fully managed by the cloud provider.

[The Source of the Knowledge](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)

**Triggers**

> The method of embedding information in the document that tells the javascript where to attach its event handlers

**Dynamo vs Mongo**

> **Mongo:** MongoDB is platform-agnostic and configured with the database to run virtually anywhere from a local machine, container, or on-premise deployment to any cloud provider. It requires users to manage all the infrastructure and configurations. MongoDB is a schema-free database.

>**Dynamo:** DynamoDB is limited to AWS and can only configure and use DynamoDB through AWS. It's a fully managed database. DynamoDB is a schema-less database but with no ability to enforce schemas.

[The Source of the Knowledge](https://www.bmc.com/blogs/mongodb-vs-dynamodb/)

**Dynamoose vs Mongoose**

> The ORM that refers to the specific database type its connected to (Dynamo and Mongo, respectively).

 <a href="#top">Take Me To The Repo!!</a>