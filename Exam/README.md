# 🧠 Operating Systems Practical – Process & Thread Programming (C)

## 📌 About This Project

This repository contains my practical test solutions for the module:

**IT2130 – Operating Systems and System Administration**

The project demonstrates key operating system concepts such as:

- Process creation using `fork()`
- Multi-threading using POSIX threads (`pthreads`)
- Inter-process and intra-process execution
- Parallel computation using threads

---

## 🚀 Questions Overview

### 🔹 Question 1 – Process Creation (fork)

- Takes user input (integer `n`)
- Creates a child process using `fork()`
- Child process:
  - Displays PID and PPID
  - Generates Fibonacci series up to `n`
- Parent process:
  - Waits using `wait()`
  - Prints completion message

---

### 🔹 Question 2 – Single Thread (pthreads)

- Takes user input `n`
- Creates a worker thread using `pthread_create()`
- Worker thread:
  - Prints Thread ID (`pthread_self()`)
  - Prints Process ID (`getpid()`)
  - Generates prime numbers up to `n`
- Main thread:
  - Waits using `pthread_join()`
  - Prints completion message

---

### 🔹 Question 3 – Multi-threaded Parallel Processing

- Takes:
  - Array size `n`
  - Array elements
  - Number of threads `t`
- Divides the array into `t` nearly equal parts
- Creates `t` worker threads
- Each thread:
  - Computes partial sum of its segment
  - Counts elements
  - Displays:
    - Thread ID
    - Process ID
    - Range
    - Partial sum
- Main thread:
  - Waits for all threads
  - Computes total sum and average

---

## 🛠️ Technologies Used

- Language: **C**
- OS: **Linux (Ubuntu)**
- Compiler: `gcc`
- Libraries:
  - `stdio.h`
  - `unistd.h`
  - `sys/wait.h`
  - `pthread.h`

---

## ⚙️ How to Run

### 🔹 Compile

```bash
gcc -o program_name file_name.c -pthread

---
## 👩‍💻 Author

Mathuppriya Naguleswaran  
Software Engineering Student  
SLIIT – Northern UNI
