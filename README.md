# CPU Scheduling Algorithms Simulation

## Overview
This project implements and compares several fundamental **CPU scheduling algorithms** using Java. The goal is to simulate process scheduling behavior, measure per-process waiting times, and evaluate the average waiting time produced by each algorithm.

This project was completed for **CS419 – Project 1: Implementing CPU Scheduling Algorithms** and focuses on understanding how different scheduling strategies impact system performance.

---

## Objectives
- Explain the basic concepts of CPU scheduling
- Implement multiple scheduling algorithms:
  - First-Come First-Served (FCFS)
  - Shortest Job First (SJF, non-preemptive)
  - Round Robin (RR)
  - Shortest Remaining Time First (SRTF)
- Simulate workloads and compute:
  - Per-process waiting time
  - Average waiting time per algorithm
- Compare the performance of different scheduling strategies

---

## Implemented Algorithms

- **FCFS (First-Come First-Served)**  
  Provided as a reference implementation.

- **SJF (Shortest Job First – Non-Preemptive)**  
  Selects the process with the smallest CPU burst time among available processes.

- **RR (Round Robin)**  
  Uses time slicing to ensure fairness across processes.
  - Time quantum = **5** for `schedule1.txt`
  - Time quantum = **10** for `schedule2.txt`

- **SRTF (Shortest Remaining Time First)**  
  Preemptive version of SJF that always selects the process with the least remaining CPU time.

---

## How the Simulation Works
1. The program reads a schedule file containing:
   - Process ID
   - Arrival time
   - CPU burst time
2. The selected scheduling algorithm simulates CPU execution.
3. Waiting time is calculated for each process.
4. The average waiting time is computed for the entire schedule.
5. Results are recorded and reported in a PDF file.
