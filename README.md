# CPU-Scheduling-Algorithms
An implementation of various CPU scheduling algorithms in C++. The algorithms included are First Come First Serve (FCFS), Round Robin (RR), Shortest Process Next (SPN), Shortest Remaining Time (SRT), Highest Response Ratio Next (HRRN), Feedback (FB) and Aging.

## Table of Contents
- [CPU-Scheduling-Algorithms](#cpu-scheduling-algorithms)
  - [Algorithms](#algorithms)
    - [First Come First Serve (FCFS)](#first-come-first-serve-fcfs)
    - [Round Robin with varying time quantum (RR)](#round-robin-with-varying-time-quantum-rr)
    - [Shortest Process Next (SPN)](#shortest-process-next-spn)
    - [Shortest Remaining Time (SRT)](#shortest-remaining-time-srt)
    - [Highest Response Ratio Next (HRRN)](#highest-response-ratio-next-hrrn)
    - [Feedback (FB)](#feedback-fb)
    - [Feedback with varying time quantum (FBV)](#feedback-with-varying-time-quantum-fbv)
    - [Aging](#aging)

## Algorithms

FCFS (First Come First Serve)
Executes processes in the order they arrive without preemption. Simple but can cause long wait times if a big process arrives early.

RR (Round Robin)
Each process gets a fixed time slice in turn, ensuring fairness. Helps avoid starvation but might increase context switches.

SPN (Shortest Process Next)
Runs the process with the shortest burst time next. Reduces average waiting time but can starve longer processes.

SRT (Shortest Remaining Time)
Preemptive version of SPN that always runs the process with the least remaining time. Responds well to short processes arriving late.

HRRN (Highest Response Ratio Next)
Schedules processes with the highest response ratio first. Balances waiting time and burst time, reducing starvation risk.

Feedback (FB)
Uses multiple priority queues where processes move between levels based on their CPU usage. Gives short jobs priority but allows longer jobs to progress.

FBV (Feedback with Varying Time Quantum)
Like Feedback but changes time slices across queues. Helps fine-tune how long processes wait and how much CPU time they get.

Aging
Gradually increases the priority of waiting processes over time. Prevents starvation by ensuring all processes eventually run.

