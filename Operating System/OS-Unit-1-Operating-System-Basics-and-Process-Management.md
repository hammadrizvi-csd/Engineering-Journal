# OS Unit 1 - Operating System Basics and Process Management

---

## 1. Operating System (OS)

An Operating System is system software that acts as an interface between computer hardware and the user.

### Objectives of OS:

* Convenience → makes computer easy to use
* Efficiency → optimal use of hardware resources

---

### OS Structure

User → Application → OS → Hardware

Examples:

* OS: Windows, Linux, macOS
* Hardware: CPU, RAM, HDD

---

## 2. Types of Operating Systems

---

### 1. Batch Operating System

* Jobs processed in batches
* No interaction with user
* CPU may remain idle

---

### 2. Multiprogramming OS

* Multiple jobs in memory
* CPU switches between jobs
* Improves CPU utilization

---

### 3. Time-Sharing OS

* Multiple users share CPU
* Uses time slices
* Fast response time

---

### 4. Real-Time OS

#### Hard RTOS

* Strict deadlines
* Example: Pacemaker

#### Soft RTOS

* Delays acceptable

---

## 3. OS Services

* Process management
* Memory management
* File management
* I/O management
* Security
* Communication

---

## 4. Program vs Process

| Program             | Process              |
| ------------------- | -------------------- |
| Passive entity      | Active entity        |
| Stored on disk      | Loaded in memory     |
| No resources needed | Requires CPU, memory |
| Example: .exe file  | Running application  |

---

## 5. Process States

* New
* Ready
* Running
* Waiting (Blocked)
* Terminated

---

### State Flow:

New → Ready → Running → Waiting → Running → Terminated

---

## 6. Process Control Block (PCB)

PCB stores all information about a process.

### Contents:

* Process ID
* Process state
* Program counter
* CPU registers
* Memory info
* I/O status

---

## 7. Threads and Multithreading

---

### Thread

* Smallest unit of execution
* Lightweight

---

### Features:

* Share same memory
* Faster communication

---

### Process vs Thread

| Process         | Thread         |
| --------------- | -------------- |
| Heavyweight     | Lightweight    |
| Separate memory | Shared memory  |
| Slow switching  | Fast switching |

---

### Types of Threads

#### User-Level Threads

* Managed by user
* Fast but blocking issue

#### Kernel-Level Threads

* Managed by OS
* Better control

---

## 8. Context Switching

Switching CPU from one process to another.

### Steps:

1. Save current process state
2. Load next process state
3. Resume execution

---

## 9. Scheduling

---

### Types of Schedulers

#### Long-Term Scheduler

* Selects jobs from disk

#### Short-Term Scheduler

* Selects process for CPU

#### Medium-Term Scheduler

* Handles swapping

---

## 10. Scheduling Criteria

* Arrival Time (AT)
* Burst Time (BT)
* Completion Time (CT)
* Turnaround Time (TAT = CT - AT)
* Waiting Time (WT = TAT - BT)

---

## 11. CPU Scheduling Algorithms

---

### 1. FCFS (First Come First Serve)

* Non-preemptive
* Executes in arrival order

#### Disadvantage:

* Convoy effect

---

### 2. SJF (Shortest Job First)

* Selects shortest job
* Optimal (minimum waiting time)

#### Disadvantage:

* Difficult to predict burst time

---

### 3. Round Robin (RR)

* Time quantum based
* Fair scheduling

#### Disadvantage:

* Context switching overhead

---

### 4. Priority Scheduling

* Based on priority

#### Problem:

* Starvation

#### Solution:

* Aging

---

## 12. Comparison of Scheduling Algorithms

| Algorithm | Type           | Use             |
| --------- | -------------- | --------------- |
| FCFS      | Non-preemptive | Batch systems   |
| SJF       | Both           | General purpose |
| RR        | Preemptive     | Time-sharing    |
| Priority  | Both           | Real-time       |

---

## 13. Dual Mode Operation

Two modes:

### User Mode

* Limited access

### Kernel Mode

* Full access

---

### Mode Bit:

* 0 → Kernel mode
* 1 → User mode

---

## 14. Process Memory Layout

Memory divided into:

* Text → program code
* Data → variables
* Heap → dynamic memory
* Stack → function calls

---

## 15. Distributed Operating System

* Multiple computers connected
* Works as single system

---

## 16. Network Operating System

* Manages network resources
* Examples: Windows Server, Linux

---

## 17. Multilevel Queue Scheduling

* Ready queue divided into multiple queues
* Each queue has different priority

### Example:

* System processes → RR
* Interactive → SJF
* Batch → FCFS

---

## Summary

* OS acts as interface between user and hardware
* Process management is core function
* Scheduling improves CPU efficiency
* Threads improve performance
* Memory and modes ensure system safety
* Distributed systems enable scalability

---
