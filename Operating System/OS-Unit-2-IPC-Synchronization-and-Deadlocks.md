# OS Unit 2 - Inter Process Communication, Synchronization and Deadlocks

---

## 1. Inter Process Communication (IPC)

IPC is a mechanism that allows processes to communicate and synchronize their actions.

---

### Need for IPC

* Information sharing (e.g., databases)
* Computation speedup (parallel execution)
* Modularity (divide system into processes)

---

### Models of IPC

#### 1. Shared Memory

* Processes share memory region
* Fast communication
* No kernel intervention

---

#### 2. Message Passing

* Processes communicate via messages
* Safer but slower

---

## 2. Critical Section Problem

A critical section is a part of code where shared resources are accessed.

---

### Requirements

1. Mutual Exclusion

* Only one process at a time

2. Progress

* Decision should not be postponed

3. Bounded Waiting

* No starvation

---

## 3. Race Condition

Occurs when multiple processes access shared data simultaneously and outcome depends on execution order.

---

## 4. Semaphores

Semaphore is a synchronization tool using integer variable.

---

### Operations:

* `wait()` → decrement
* `signal()` → increment

---

### Types:

#### Binary Semaphore (Mutex)

* Values: 0 or 1
* Used for mutual exclusion

---

#### Counting Semaphore

* Used for multiple resources

---

## 5. Producer-Consumer Problem

* Producer → adds data to buffer
* Consumer → removes data

---

### Constraints:

* No overflow
* No underflow
* Mutual exclusion

---

### Solution (Semaphores):

* mutex = 1
* empty = n
* full = 0

---

### Producer Code

```c
do {
    wait(empty);
    wait(mutex);

    // add item

    signal(mutex);
    signal(full);
} while(TRUE);
```

---

### Consumer Code

```c
do {
    wait(full);
    wait(mutex);

    // remove item

    signal(mutex);
    signal(empty);
} while(TRUE);
```

---

## 6. Readers-Writers Problem

* Readers → only read
* Writers → read + write

---

### Rules:

* Multiple readers allowed
* Only one writer allowed

---

### Solution:

* Use semaphores: mutex, write
* Track reader count

---

## 7. Dining Philosophers Problem

* 5 philosophers, 5 chopsticks
* Need 2 chopsticks to eat

---

### Problem:

* Deadlock

---

### Solutions:

* Limit philosophers
* Asymmetric solution
* Resource ordering

---

## 8. Deadlock

Deadlock occurs when processes wait indefinitely for resources.

---

### Example:

P1 holds R1, waits for R2
P2 holds R2, waits for R1

---

## 9. Necessary Conditions for Deadlock

1. Mutual Exclusion
2. Hold and Wait
3. No Preemption
4. Circular Wait

---

## 10. Resource Allocation Graph (RAG)

* Nodes → processes & resources
* Cycle → possible deadlock

---

## 11. Deadlock Handling Methods

---

### 1. Prevention

* Break one condition

---

### 2. Avoidance

* Use Banker’s Algorithm

---

### 3. Detection & Recovery

* Detect deadlock
* Recover

---

### 4. Ignore

* Assume deadlock rare

---

## 12. Banker’s Algorithm

Used to avoid deadlock.

---

### Data Structures:

* Available
* Max
* Allocation
* Need = Max - Allocation

---

### Steps:

1. Find process with Need ≤ Available
2. Execute process
3. Release resources
4. Repeat

---

### Safe State:

* System is safe if safe sequence exists

---

## 13. Deadlock Detection

* Check cycles in graph
* Use algorithm similar to Banker

---

## 14. Deadlock Recovery

---

### 1. Process Termination

* Kill processes

---

### 2. Resource Preemption

* Take resources back

---

## 15. Deadlock Prevention Techniques

---

### 1. Mutual Exclusion

* Make resources shareable

---

### 2. Hold and Wait

* Allocate all resources at once

---

### 3. No Preemption

* Force release resources

---

### 4. Circular Wait

* Assign ordering to resources

---

## 16. Monitor

* High-level synchronization tool
* Only one process executes at a time

---

## 17. Event Counter

* Synchronization without mutual exclusion
* Tracks occurrence of events

---

## Summary

* IPC enables communication
* Semaphores solve synchronization
* Classic problems: Producer-Consumer, Readers-Writers
* Deadlocks are critical issue
* Banker’s Algorithm avoids deadlocks
* Prevention, avoidance, detection are key strategies

---
