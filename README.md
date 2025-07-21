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

## 📈 Results

- The agent consistently learns to land safely after approximately **1000 episodes**.
- Final rewards converge toward **200+**, indicating effective mastery of the task.
- The spacecraft learns smooth landings with minimal fuel use and few crashes.

---

## 🧠 What I Learned

- Implemented core reinforcement learning concepts from scratch.
- Gained deep understanding of **experience replay**, **target networks**, and **exploration-exploitation strategies**.
- Tuned hyperparameters such as learning rate, epsilon decay, and discount factor to optimize performance.
- Learned to debug training instability and visualize learning curves for agent evaluation.

---

## ✅ Future Work

- Implement **Double DQN** and **Dueling DQN** for more robust training.
- Add **TensorBoard logging** for real-time performance visualization.
- Explore **prioritized experience replay** and **NoisyNet exploration**.
- Try more challenging environments like **BipedalWalker** or custom-designed physics tasks.

---

## 📜 References

- [OpenAI Gym](https://www.gymlibrary.dev/)
- [Deep Q-Learning with Experience Replay — Mnih et al., 2015](https://www.nature.com/articles/nature14236)
- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)
- [Machine Learning Specialization by Andrew Ng](https://www.coursera.org/specializations/machine-learning-introduction)

---

## 🤝 Acknowledgements

This project was completed as part of the **Machine Learning Specialization** on Coursera by **Andrew Ng**, Stanford University.

Special thanks to the OpenAI Gym team for providing the simulation environment.

## 🧪 Training Setup

```bash
# Install dependencies
pip install gym[box2d] torch matplotlib
