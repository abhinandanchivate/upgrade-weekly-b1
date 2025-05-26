# Student Manual: Introduction to Databases, Data Models & Types of Databases

## 📘 Module Overview

This manual provides a comprehensive understanding of databases, their structure, types, and how they are used in real-world applications. It is designed for students, developers, and professionals new to the subject.

---

## 1️⃣ What is a Database?

### Definition:

A database is a structured collection of data that is stored electronically and managed by a Database Management System (DBMS). It enables efficient storage, retrieval, and management of data.

### Characteristics:

* **Structured:** Data is organized into tables, records, fields.
* **Persistent:** Data remains available over time.
* **Accessible:** Can be queried using specialized languages (e.g., SQL).
* **Secure:** Allows authorization and access control.
* **Concurrent Access:** Supports multiple users simultaneously.
* **Integrity Constraints:** Enforces rules to maintain data accuracy.

### Traditional File System vs Database:

| Feature            | File System | Database              |
| ------------------ | ----------- | --------------------- |
| Redundancy Control | No          | Yes                   |
| Data Integrity     | Manual      | Enforced by DBMS      |
| Querying Ability   | Limited     | Rich querying via SQL |
| Concurrency        | Poor        | Excellent             |
| Scalability        | Low         | High                  |

---

## 2️⃣ Importance of Databases

* **Efficiency:** Speeds up data access through indexing, query optimization.
* **Integrity:** Maintains consistency through constraints and transactions.
* **Security:** Manages access with user roles and permissions.
* **Backup and Recovery:** Protects data through automated processes.
* **Scalability:** Designed to grow with the application.
* **Analytics:** Powers reporting, BI tools, and decision-making systems.

---

## 3️⃣ Database Terminology

| Term           | Description                                                         |
| -------------- | ------------------------------------------------------------------- |
| DBMS           | Software to create, manage, and interact with a database            |
| Table          | Organized data structure using rows and columns                     |
| Row (Record)   | A single data entry or instance in a table                          |
| Column (Field) | A specific attribute or property of the data                        |
| Query          | A command to retrieve or manipulate data                            |
| Schema         | Blueprint or design of the database (tables, fields, relationships) |
| Primary Key    | Uniquely identifies each record in a table                          |
| Foreign Key    | Links records across tables through relationships                   |
| Index          | Data structure that improves the speed of data retrieval            |

---

## 4️⃣ What is a Data Model?

### Definition:

A data model is a conceptual model that defines how data is stored, related, and accessed within a database. It provides a structured framework that enables consistent data management and design.

### Benefits:

* Clear structure
* Easy maintenance
* Logical data access
* Better collaboration between developers and DBAs

### Key Concepts:

* **Entities:** Real-world objects (e.g., Student, Course)
* **Attributes:** Properties of entities (e.g., Student Name, ID)
* **Relationships:** Associations between entities (e.g., Enrolled In)

---

## 5️⃣ Types of Data Models

### 1. Hierarchical Model

* Organizes data in a tree-like structure (parent-child)
* Each child has one parent
* Example: Organizational chart
* Limitation: Poor flexibility

### 2. Network Model

* Graph structure with multiple relationships
* Each child can have multiple parents
* Used in early DBMS systems like IDS, IDMS

### 3. Relational Model

* Uses tables (relations)
* Based on mathematical relations
* Most widely used
* Supports SQL

### 4. Entity-Relationship (ER) Model

* Used for designing databases visually
* Entities, attributes, and relationships
* Converted into relational schema during implementation

### 5. Object-Oriented Model

* Based on objects (from OOP)
* Data stored as classes and objects
* Ideal for multimedia and complex data

### 6. Document Model (NoSQL)

* Uses documents (typically JSON/XML)
* Schema-less
* Ideal for fast development and changing requirements

---

## 6️⃣ Types of Databases

### Relational Databases (SQL)

* Structured data in rows and columns
* Schema defined in advance
* Uses SQL (Structured Query Language)
* Supports ACID properties (Atomicity, Consistency, Isolation, Durability)
* Examples: MySQL, PostgreSQL, Oracle, SQL Server

### NoSQL Databases

* Designed for semi-structured or unstructured data
* Scales horizontally
* Types:

#### a. Document-Oriented

* Stores data in JSON-like format
* Flexible schema
* Examples: MongoDB, CouchDB

#### b. Key-Value Stores

* Simplest NoSQL model
* Each item stored as a key-value pair
* Examples: Redis, DynamoDB

#### c. Column-Family Stores

* Stores data in columns, optimized for reads/writes
* Examples: Cassandra, HBase

#### d. Graph Databases

* Represents data as nodes and relationships
* Ideal for social networks, fraud detection
* Examples: Neo4j, ArangoDB

#### e. Time-Series Databases

* Optimized for time-stamped or chronological data
* Examples: InfluxDB, TimescaleDB

#### f. NewSQL

* Modern relational databases with NoSQL scalability
* Examples: Google Cloud Spanner, CockroachDB

---

## 7️⃣ SQL vs NoSQL

| Feature        | SQL (Relational)            | NoSQL (Non-relational)              |
| -------------- | --------------------------- | ----------------------------------- |
| Schema         | Fixed schema                | Flexible schema                     |
| Data Format    | Tables                      | Documents, Graphs, Key-Value, etc.  |
| Scalability    | Vertical                    | Horizontal                          |
| Transactions   | Strong (ACID)               | Often eventual consistency          |
| Query Language | SQL                         | Varies (MongoQL, CQL, Gremlin, etc) |
| Use Case       | Structured, relational data | Large-scale, semi/unstructured data |

---

## 8️⃣ Use Cases of Different Databases

| Type            | Use Case Example                      | Industry            |
| --------------- | ------------------------------------- | ------------------- |
| Relational      | Customer orders and billing systems   | Retail, Finance     |
| Document        | Dynamic product catalog               | E-commerce, CMS     |
| Key-Value       | Session management, real-time caching | Web applications    |
| Columnar        | Real-time analytics on large datasets | Telecom, IoT        |
| Graph           | Relationship and pattern detection    | Social media, Fraud |
| Time-Series     | Metrics and performance tracking      | DevOps, IoT         |
| Object-Oriented | Complex applications with OOP logic   | CAD/CAM, Multimedia |

---

## 9️⃣ Selection Criteria for Databases

* Data structure: Structured vs unstructured
* Consistency requirements: ACID vs eventual
* Query complexity: Need for joins, aggregations
* Scalability needs: Vertical vs horizontal
* Latency sensitivity: Real-time vs batch
* Storage capacity and cost

---

## 🔟 Summary & Best Practices

* Understand data structure before choosing DB type
* Normalize relational data for consistency
* Use indexing to speed up queries
* Regularly back up your databases
* Monitor performance and scale when needed
* Choose NoSQL for flexible and large-scale apps

---

## 💡 Practice Activities

1. Identify and classify databases used in top 5 websites/apps.
2. Design an ER diagram for a University Management System.
3. Write basic SQL queries to create and manipulate tables.
4. Set up MongoDB Atlas and insert sample documents.
5. Compare and contrast use cases for SQL vs NoSQL in a scenario.

---

## 📚 Recommended Tools & Resources

* **MySQL Workbench:** SQL DB visualizer and admin tool
* **MongoDB Atlas:** Cloud-based NoSQL DB
* **ERDPlus:** Online ER diagram generator
* **DB Fiddle:** SQL editor and testing tool
* **PostgreSQL:** Open-source SQL database
* **Redis CLI:** Key-Value DB access
* **InfluxDB UI:** Time-series DB interface

---
