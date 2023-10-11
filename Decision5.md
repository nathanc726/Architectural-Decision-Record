<a name="br1"></a> 

**Decision 5 - Data Storage**

**Decision: SQLite for Data Storage**

Using SQLite rather than NoSQL for local data processing and storage.

**Rationale**

SQLite is a Relational Database Management System (RDBMS). All data are organized into tables with predefined schemas. It is a lightweight, efficient, and self-contained database engine for data storage and processing locally, allowing users to access and manipulate data stored locally in offline mode.
NoSQL is a flexible and schema-less data model which encompasses a variety of database management systems. It is usually designed for handling unstructured and/or semi-structured data. Although NoSQL offers offline data access and manipulation, it solely depends on specific databases and corresponding configurations.

**Consequences**

Although both types of database systems offer data storage, manipulation, and synchronization, all data such as financial transactions and inventory management processed and stored in this app requires fixed data structure, consistency, and integrity. SQLite is more capable of maintaining consistency and reliability and being free from anomalies which results in a lower risk of errors and data corruption.

Page | 9


