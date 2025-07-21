# 🚀 Deep Q-Learning Agent for Lunar Lander

This project implements a Deep Q-Network (DQN) to solve the **Lunar Lander** environment from OpenAI Gym. The agent learns to land a spacecraft safely between flags on the Moon’s surface using reinforcement learning techniques.

---

## 📌 Overview

- **Environment**: LunarLander-v2 (Box2D-based physics simulation)
- **Algorithm**: Deep Q-Learning (DQN)
- **Goal**: Land the spacecraft smoothly with minimum fuel consumption and avoid crashing.

---

## 🎯 Features

- Custom **Replay Buffer** for experience replay
- **Epsilon-Greedy** policy for exploration-exploitation tradeoff
- **Target Network** for stable learning
- Tunable **hyperparameters**
- Visualization of agent performance over training episodes

---

## 🧠 Key Concepts

| Concept            | Details                                                                 |
|--------------------|-------------------------------------------------------------------------|
| **State Space**    | 8-dimensional vector (position, velocity, angle, etc.)                  |
| **Action Space**   | 4 discrete actions (do nothing, fire left/right engines, fire main)     |
| **Reward**         | +100 to +140 for landing, -100 for crashing, -0.3 per frame (fuel burn) |
| **Libraries Used** | `NumPy`, `Matplotlib`, `OpenAI Gym`, `PyTorch`                          |

---

## 🧪 Training Setup

```bash
# Install dependencies
pip install gym[box2d] torch matplotlib
