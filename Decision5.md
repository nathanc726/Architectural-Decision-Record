<a name="br1"></a> 

**Decision 5 - Data Storage**

**Decision: SQLite for Data Storage**

Using SQLite rather than NoSQL for local data processing and storage.

**Raꢀonale**

SQLite is a Relaꢀonal Database Management System (RDBMS). All data are organized into tables with

predeﬁned schemas. It is a lightweight, eﬃcient, and self-contained database engine for data storage and

processing locally, allowing users to access and manipulate data stored locally in oﬄine mode.

NoSQL is a ﬂexible and schema-less data model which encompasses a variety of database management

systems. It is usually designed for handling unstructured and/or semi-structured data. Although NoSQL

oﬀers oﬄine data access and manipulaꢀon, it solely depends on speciﬁc databases and corresponding

conﬁguraꢀons.

**Consequences**

Although both types of database systems oﬀer data storage, manipulaꢀon, and synchronizaꢀon, all data

such as ﬁnancial transacꢀons and inventory management processed and stored in this app requires ﬁxed

data structure, consistency, and integrity. SQLite is more capable of maintaining consistency and reliability

and being free from anomalies which results in a lower risk of errors and data corrupꢀon.

Page | 9


