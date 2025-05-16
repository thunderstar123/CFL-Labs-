# Reinforcement Learning for Freight Vehicle Parking Allocation

## Project Overview

This project implements a Reinforcement Learning (RL) solution to optimize parking allocation for freight vehicles in urban areas. The goal is to reduce illegal parking, minimize waiting times, and maximize utilization of limited parking spots by dynamically assigning available spots based on real-time conditions.

---

## Implementation Summary

- **Environment:** Simulates fixed parking spots, dynamic vehicle arrivals (including peak/off-peak variations), parking durations, and time progression.
- **State Space:** Includes parking spot occupancy, number of waiting vehicles, and time of day.
- **Action Space:** Assign a vehicle to a specific spot or defer allocation.
- **Reward Function:** Encourages legal, efficient parking with penalties for illegal attempts, long waits, or unnecessary allocations.
- **Agent:** Deep Q-Network (DQN) implemented using PyTorch, trained over multiple episodes to learn an optimal parking allocation policy.
- **Training:** Experience replay, epsilon-greedy exploration, and target network updates stabilize learning.
- **Evaluation:** Tracks average wait time, illegal parking incidents, and utilization rates to measure performance improvements.

---

## Tools and Libraries Used

| Component       | Tool/Library          | Purpose                                     |
|-----------------|-----------------------|-------------------------------------------- |
| Simulation Env  | Gymnasium             | Custom RL environment simulation            |
| RL Framework    | PyTorch               | Deep Q-Network model and training           |
| Data Handling   | NumPy                 | Numerical computations and state management |
| Visualization   | Matplotlib            | Plotting metrics and environment state      |
| Experience Replay | Python deque        | Efficient memory for training samples       |
| Python Version  | 3.7+                  | Compatible runtime                          |



