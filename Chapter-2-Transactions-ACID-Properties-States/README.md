# Chapter 2 - Transactions And Concurrency Control

### Transaction

A transaction is a fundamental entity which represents a set of logically inter related instructions to perform one logical unit of work.

#### READ

Accessing the database item x from disk where database stored data to memory variable also name as X

#### WRITE

Writing the data item from memory variable X

### Desirable Properties of Transactions
As smalles unit which have atomicity in DBMS View is transaction, so if we want that our data should be consistent then instead of concentrating on DB, we must concentrate on the transaction for our data to be consistent

Transactions should possess several properties often called ACID properties to provide integrity and consistency of the data in the database. The following are the ACID properties. 



