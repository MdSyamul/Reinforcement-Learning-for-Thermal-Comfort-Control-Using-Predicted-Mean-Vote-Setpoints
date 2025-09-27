# Reinforcement Learning for Thermal Comfort Control Using Predicted Mean Vote Setpoints

This repository provides an implementation and demonstration of reinforcement learning (RL) methods for controlling indoor thermal comfort by optimizing HVAC setpoints based on predicted mean vote (PMV) indices. The project leverages predictive models and RL algorithms to dynamically adjust environmental conditions for occupant comfort and energy efficiency.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [References](#references)
- [License](#license)

---

## Overview

Thermal comfort is a critical aspect of building environmental quality, impacting both occupant satisfaction and energy consumption. The Predicted Mean Vote (PMV) is a widely used metric to quantify thermal comfort based on environmental parameters and human factors.

This repository demonstrates how reinforcement learning can be employed to:
- Predict PMV using sensor data and contextual features.
- Control HVAC setpoints in real-time to maintain target PMV values.
- Balance occupant comfort against energy usage.

## Features

- PMV prediction model using sensor and contextual data
- RL agent for HVAC control (e.g., DQN, PPO, or your choice)
- Simulation environment for thermal comfort control
- Data pre-processing and visualization tools
- Scripts for training, evaluation, and benchmarking

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

3. **Configure environment:**
   - Update configuration files as needed (see `config/` directory).
   - Prepare your dataset or simulation parameters.

## Repository Structure

```
├── data/                # Datasets and example input files
├── models/              # Pretrained models and training scripts
├── envs/                # Simulation environment for RL agent
├── rl_agents/           # RL algorithm implementations
├── utils/               # Utility scripts for preprocessing and visualization
├── config/              # Configuration files
├── results/             # Results, logs, figures
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

## Requirements

- Python 3.7+
- NumPy, pandas, scikit-learn
- TensorFlow or PyTorch (depending on RL agent)
- matplotlib, seaborn (for visualization)
- [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3) or similar RL library (optional)

See `requirements.txt` for the full list.

## Usage

1. **Prepare Data:** Place your sensor and contextual data in the `data/` directory.
2. **Train PMV Model:** Run the scripts in `models/` to train or load a PMV prediction model.
3. **Configure RL Environment:** Set your simulation parameters in `config/`.
4. **Train RL Agent:** Use scripts in `rl_agents/` to train a reinforcement learning agent for thermal comfort control.
5. **Evaluate and Visualize:** Generate results and visualizations with scripts in `utils/`.

Example command to train an RL agent:
```bash
python rl_agents/train_agent.py --config config/thermal_comfort.yaml
```

## Results

Results from training and evaluation—including PMV prediction accuracy, comfort metrics, and energy consumption—can be found in the `results/` directory. Visualization scripts are also provided to plot performance curves and comfort profiles.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
