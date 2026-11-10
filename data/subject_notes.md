Subject: Database Management System (DBMS) – B.Tech CSE Core
I have replaced all four Operating Systems topics with important DBMS topics, maintaining the same technical depth, structure, and academic language as your original content.
Topic 1: DBMS vs File System
A Database Management System (DBMS) is software that allows users to efficiently store, retrieve, update, and manage structured data. Unlike a traditional File System, where data is stored in separate files, a DBMS provides centralized data management with controlled access.

A File System often suffers from data redundancy, data inconsistency, limited security, and difficulty in sharing data. In contrast, a DBMS reduces data duplication through normalization, maintains data integrity using constraints, and provides security through authentication and authorization. It also supports concurrent access, backup, and recovery mechanisms.

Key Advantages of DBMS:
1. Data Independence: Changes in the database structure do not necessarily require changes in application programs.
2. Data Security: Restricts unauthorized access through user permissions.
3. Data Integrity: Maintains accuracy and consistency using constraints.
4. Concurrency Control: Allows multiple users to access data simultaneously without conflicts.
5. Backup and Recovery: Restores data after system failures.
Topic 2: Database Normalization and Normal Forms
Normalization is the process of organizing data in a relational database to minimize redundancy and prevent data anomalies. It involves dividing large tables into smaller related tables while maintaining relationships through primary and foreign keys.

Normalization helps eliminate three major anomalies:
- Insertion Anomaly: Difficulty in inserting new data without additional unrelated information.
- Update Anomaly: The same information must be updated at multiple locations.
- Deletion Anomaly: Deleting one record unintentionally removes other important information.
The major Normal Forms are:
1. First Normal Form (1NF): Every column must contain atomic (single) values, and each record must be unique.
2. Second Normal Form (2NF): The table must be in 1NF, and every non-key attribute must be fully functionally dependent on the entire candidate key.
3. Third Normal Form (3NF): The table must be in 2NF and should not contain transitive dependencies between non-key attributes.
4. Boyce-Codd Normal Form (BCNF): A stronger version of 3NF in which every determinant must be a superkey.
Normalization improves database efficiency, reduces unnecessary storage, and maintains data consistency.
Topic 3: SQL, Keys, and Constraints
Structured Query Language (SQL) is the standard language used to communicate with relational database systems. It allows users to create database structures, insert records, retrieve information, and modify or delete existing data.

SQL commands are categorized into five major groups:
1. DDL (Data Definition Language): Defines database structures using commands such as CREATE, ALTER, DROP, and TRUNCATE.
2. DML (Data Manipulation Language): Modifies records using INSERT, UPDATE, and DELETE.
3. DQL (Data Query Language): Retrieves data using the SELECT command.
4. DCL (Data Control Language): Controls access permissions using GRANT and REVOKE.
5. TCL (Transaction Control Language): Manages transactions using COMMIT, ROLLBACK, and SAVEPOINT.
Database Keys and Constraints:
- Primary Key: Uniquely identifies each record in a table and cannot contain NULL values.
- Foreign Key: Establishes relationships between tables by referencing a candidate or primary key in another table.
- Candidate Key: A minimal set of attributes capable of uniquely identifying a record.
- Super Key: Any set of attributes that uniquely identifies a record.
- Unique Constraint: Ensures that values in a column or combination of columns are unique.
- NOT NULL Constraint: Prevents a column from storing NULL values.
These concepts ensure data accuracy, maintain relationships, and enforce database integrity.
Topic 4: Database Transactions and ACID Properties
A Transaction is a logical unit of database operations that performs one complete task. For example, transferring money between two bank accounts involves deducting money from one account and adding it to another.

A transaction must follow the four ACID properties to maintain database reliability:
1. Atomicity: A transaction is treated as a single indivisible unit. Either all operations are completed successfully, or none of them are applied.
2. Consistency: Every transaction must move the database from one valid state to another while maintaining all integrity constraints.
3. Isolation: Multiple transactions executing simultaneously should not interfere with each other. Each transaction should behave as if it were executing independently.
4. Durability: Once a transaction is successfully committed, its changes remain permanently stored, even if a system crash occurs.
Important Transaction Concepts:
- COMMIT: Permanently saves the changes made by a transaction.
- ROLLBACK: Reverses changes made by an uncommitted transaction.
- Concurrency Control: Manages simultaneous transactions to prevent inconsistencies.
- Deadlock: Occurs when two or more transactions wait indefinitely for resources locked by one another.
ACID properties ensure database consistency, reliability, and safe transaction processing, especially in banking, e-commerce, and financial applications.