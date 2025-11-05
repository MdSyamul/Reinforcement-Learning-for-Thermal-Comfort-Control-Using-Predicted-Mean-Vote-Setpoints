# Reinforcement Learning for Thermal Comfort Control Using Predicted Mean Vote Setpoints

This repository provides an implementation and demonstration of reinforcement learning (RL) methods for controlling indoor thermal comfort by optimizing HVAC setpoints based on predicted mean vote (PMV) indices. The project leverages predictive models and RL algorithms to dynamically adjust environmental conditions for occupant comfort and energy efficiency.

## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
- [Requirements](#requirements)
- [License](#license)

---

## Overview
Fixed AC set temperatures cannot reliably maintain comfort over a time window, as other parameters influencing comfort vary over time, e.g., mean radiant temperature, activity level, etc. The solution is to set a desired comfort level (e.g., Predicted Mean Vote of 0) and regulate the AC set temperature to track that pre-set Predicted Mean Vote (PMV). To address this, this study presents a reinforcement learning-based control policy that maintains the Predicted Mean Vote (PMV) at the desired set value by suggesting the optimum AC set temperature. A Deep Neural Network-based PMV prediction model was employed as the training environment for the reinforcement learning agent. Two RL algorithms: One-Step Greedy Policy and Supervised Behavioral Cloning were used to train the control policy, where the state space comprised relative humidity, air velocity, metabolic rate, clothing insulation, season, climate, monthly air temperature, building types, and the action space is discrete air temperature. Both RL-based control policies effectively maintained the PMV within the range of [−0.3, +0.3] of the user-specified (set) PMV by adjusting the AC set temperature according to the recommendations made by the policies. These proposed policies will eliminate the need for manual adjustments of the AC set temperature, which people often forget to do, leading to energy waste. The result is better comfort and improved energy efficiency. 

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/MdSyamul/Reinforcement-Learning-for-Thermal-Comfort-Control-Using-Predicted-Mean-Vote-Setpoints.git
   cd Reinforcement-Learning-for-Thermal-Comfort-Control-Using-Predicted-Mean-Vote-Setpoints
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Requirements

- Python 3.10

See `requirements.txt` for the full list.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
