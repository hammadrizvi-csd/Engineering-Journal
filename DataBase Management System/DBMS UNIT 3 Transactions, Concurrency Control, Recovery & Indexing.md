# DBMS Unit 3 - Transactions, Concurrency Control, Recovery and Indexing

---

## 1. Database Transaction

A database transaction is a logical unit of work consisting of multiple operations (read/write) performed on a database.

### Key Points:

* Must be executed completely or not at all
* Maintains database consistency
* Transforms database from one state to another

---

## 2. ACID Properties

### Atomicity

* All or nothing execution
* Failure leads to rollback

### Consistency

* Database remains valid before and after transaction

### Isolation

* Transactions do not interfere with each other

### Durability

* Changes are permanently stored

---

## 3. Transaction States

1. Active – Transaction is executing
2. Partially Committed – Last operation executed
3. Committed – Transaction completed successfully
4. Failed – Transaction failed due to error
5. Terminated – Transaction ends

---

## 4. Concurrent Execution

Concurrent execution means multiple transactions are executed at the same time.

### Advantages:

* Better CPU utilization
* Faster processing
* Improved throughput

---

## 5. Problems in Concurrency

### Lost Update Problem

* One transaction overwrites another

### Dirty Read Problem

* Reading uncommitted data

### Unrepeatable Read Problem

* Same query gives different results

---

## 6. Concurrency Control

Mechanism used to manage concurrent execution and maintain consistency.

### Objectives:

* Ensure atomicity
* Maintain consistency
* Provide isolation

---

## 7. Lock-Based Protocol

### Types of Locks

#### Shared Lock

* Allows read only
* No modification allowed

#### Exclusive Lock

* Allows read and write
* No other transaction allowed

---

### Lock Protocols

#### Simple Lock Protocol

* Lock before access
* Unlock after use

#### Pre-Claiming Protocol

* All locks acquired before execution

#### Two-Phase Locking (2PL)

* Growing Phase: Locks are acquired
* Shrinking Phase: Locks are released

---

## 8. Timestamp Ordering Protocol

* Each transaction is assigned a timestamp
* Execution is based on timestamps

### Rules:

* Older transactions get priority
* Invalid operations are rejected

---

## 9. Schedule in DBMS

A schedule defines the execution order of transactions.

### Types:

#### Serial Schedule

* Transactions executed one after another

#### Non-Serial Schedule

* Transactions are interleaved

#### Serializable Schedule

* Equivalent to serial execution

---

## 10. Database Recovery

Database recovery restores database after failure.

### Causes:

* System crash
* Power failure
* Software error

---

## 11. System Log

Stores all transaction details.

### Contains:

* Start transaction
* Write operations
* Commit
* Abort

---

## 12. Recovery Techniques

### Deferred Update

* Changes applied after commit
* Uses REDO

### Immediate Update

* Changes applied before commit
* Uses UNDO and REDO

---

## 13. Checkpoint

* Saves database state
* Reduces recovery time

---

## 14. Shadow Paging

* Maintains two copies:

  * Original
  * Modified

---

## 15. Buffering

* Data temporarily stored in memory
* Written to disk later

---

## 16. Hashing

Technique used for fast data retrieval.

### Components:

* Hash Function
* Data Bucket

---

### Types of Hashing

#### Static Hashing

* Fixed buckets

#### Dynamic Hashing

* Buckets can grow or shrink

---

## 17. Collision Handling

### Chaining

* Uses linked list

### Open Addressing

#### Methods:

* Linear Probing
* Quadratic Probing
* Double Hashing

---

## 18. B-Tree

A balanced tree used in indexing.

### Features:

* Multiple children
* Balanced structure

### Advantages:

* Fast search
* Efficient insertion and deletion

---

## Summary

* Transactions ensure consistency
* ACID properties maintain reliability
* Concurrency improves performance but introduces problems
* Locking and timestamp protocols control concurrency
* Recovery techniques ensure data safety
* Hashing and B-Tree improve data access speed

---
