# Chapter 2 - Transactions And Concurrency Control

### Transaction

A transaction is a fundamental entity which represents a set of logically inter related instructions to perform one logical unit of work.

#### READ

Accessing the database item x from disk where database stored data to memory variable also name as X

#### WRITE

Writing the data item from memory variable X

### Desirable Properties of Transactions

As smallest unit which have atomicity in DBMS View is transaction, so if we want that our data should be consistent then instead of concentrating on DB, we must concentrate on the transaction

Transactions should possess several properties often called ACID properties to provide integrity and consistency of the data in the database. The following are the ACID properties.

- Atomicity
- Consistency
- Isolation
- Durability

#### Atomicity

A transaction is an atomic unit of processing, it should be either performed in its entirety or not performed at all.

- It is the responsibility of the **Recovery Control Manager** or **Transaction Control Manager** of DBMS to ensure atomicity

#### Consistency

A Transaction should be consistency preserving, meaning it has to be executed completely from beginning to end without interference from other transaction. It should take the database from one consistent state to the other.

#### Isolation

A Transaction should appear as though it is being executed in isolation from other transactions, even though many transactions are executing concurrently.Which means execution of a transaction must not be hampered by any other transaction being executed concurrently.

- It is the responsibility of the **Concurrency Control Manager** of the database to ensure Isolation


#### Durability
Changes applied to the database by a committed transaction must persist in the database.The changes must not be lost due to any failure like power outage or software crashes. 

It is the responsibility of the **Recovery Control Manager** of the Database Management System 
