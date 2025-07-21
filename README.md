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

📈 Results
The agent consistently learns to land safely after ~1000 episodes.

Reward converges towards 200+, indicating successful mastery of the environment.

<!-- optional if you have it -->

🧠 What I Learned
Implemented core reinforcement learning concepts from scratch

Understood and applied experience replay and target networks

Tuned hyperparameters and explored learning dynamics

📂 Project Structure
bash
Copy
Edit
📁 dqn-lunar-lander/
├── dqn_lunar_lander.py      # Main training script
├── replay_buffer.py         # Experience Replay Buffer class
├── model.py                 # Neural network model (Q-function)
├── utils.py                 # Helper functions
├── README.md                # Project documentation
✅ Future Work
Implement Double DQN or Dueling DQN

Integrate TensorBoard for better monitoring

Try alternative environments like CartPole or BipedalWalker

📜 References
OpenAI Gym: https://www.gymlibrary.dev/

Deep Q-Learning Paper: Mnih et al., 2015

Course: Machine Learning Specialization by Andrew Ng

🤝 Acknowledgements
This project was completed as part of the Machine Learning Specialization on Coursera by Andrew Ng, Stanford University.

yaml
Copy
Edit

---

Let me know if you'd like:

- A code scaffold that matches this README
- An additional section for "Demo Video" or Colab link
- Conversion into PDF format for portfolio inclusion

---

## 🧪 Training Setup

```bash
# Install dependencies
pip install gym[box2d] torch matplotlib
