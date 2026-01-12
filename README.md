# 🤖🎮 Unity AI Learning to Move with PPO Reinforcement Learning

![Unity](https://img.shields.io/badge/Unity-3D-black.svg)
![ML-Agents](https://img.shields.io/badge/ML--Agents-PPO-blue.svg)
![Reinforcement Learning](https://img.shields.io/badge/Reinforcement-Learning-green.svg)

![License](https://img.shields.io/badge/license-MIT-green.svg)  
![Contributions](https://img.shields.io/badge/contributions-welcome-orange.svg)  

<p align="center">
  <img src="img/Gif-Unity_move.gif" alt="Gif - ML AI moving">
</p>

## 📝 Project Description
This project demonstrates **Reinforcement Learning** using **PPO (Proximal Policy Optimization)** in **Unity 3D** to train an AI agent to navigate and reach a target.  
The blue cube learns to move towards the yellow sphere (reward) through trial and error across multiple parallel training environments.

⚡️ Essentially, the AI learns navigation skills autonomously by being rewarded for reaching its goal!

---

## ⚙️ Features

🧠 **PPO Reinforcement Learning** - State-of-the-art algorithm for training intelligent agents.  

🎮 **Unity ML-Agents** - Unity's machine learning framework for 3D environments.  

🔄 **Parallel Training** - Multiple platforms train simultaneously to speed up learning.  

📊 **Visual Feedback** - Green platforms indicate successful goal reach within time limit, red indicates failure.  

🎯 **Simple Goal** - Blue cube agent learns to reach yellow sphere reward.

---

## 📊 Example Outputs

### Neural Network Architecture
The AI agent uses a fully connected neural network trained with PPO:

<p align="center">
  <img src="img/Capture%20d'écran%202026-01-09%20231045.png" alt="Neural Network Architecture" width="600">
</p>

### Training Process
Watch the agent learn across multiple parallel environments. The training demonstrates how multiple blue cubes simultaneously learn to reach their yellow targets:

**Perspective View:**
<p align="center">
  <img src="img/Gif-Unity_move-X9-training-perspective.gif" alt="Training - Perspective View" width="700">
</p>

**Top-Down View:**
<p align="center">
  <img src="img/Gif-Unity_move-X9-training.gif" alt="Training - Top View" width="700">
</p>

### Trained Agent Performance
After training, the agent efficiently navigates to its target:

**Top-Down View:**
<p align="center">
  <img src="img/Gif-Unity_move-X9.gif" alt="Trained Agent - Top View" width="700">
</p>

**Perspective View:**
<p align="center">
  <img src="img/Gif-Unity_move-perspective.gif" alt="Trained Agent - Perspective View" width="700">
</p>

---

## 🧠 Training Visualization

The training process demonstrates reinforcement learning in action:
- **Blue cubes** = AI agents learning to navigate  
- **Yellow spheres** = Target rewards to reach  
- **Green platforms** = Successful episodes (goal reached in time)  
- **Red platforms** = Failed episodes (timeout before reaching goal)

As training progresses, you'll observe more green platforms appearing, indicating improved performance and successful goal completions.

---

## ⚙️ How it Works

1. 🎬 **Environment Reset** → Each platform initializes with random agent and target positions.  
2. 🤖 **Observation** → The agent observes its position, target position, and distance.  
3. 🧠 **Decision** → PPO algorithm decides movement actions based on current policy.  
4. 🎯 **Action & Reward** → Agent moves and receives rewards for getting closer or reaching the goal.  
5. 🔄 **Learning** → Neural network updates based on accumulated experiences across all platforms.  
6. ✅ **Success Indicator** → Platform turns green on success, red on timeout.

The parallel training approach significantly accelerates the learning process by gathering experiences from multiple agents simultaneously.

---

## 🧰 Components

| Component | Description |
|-----------|-------------|
| 🎮 **Training Platform** | Multiple parallel environments for simultaneous learning |
| 🤖 **Agent (Blue Cube)** | AI-controlled entity learning navigation |
| 🎯 **Goal (Yellow Sphere)** | Target reward the agent must reach |
| 🧠 **PPO Algorithm** | Reinforcement learning algorithm optimizing agent behavior |
| 📊 **Visual Feedback** | Color-coded platforms showing success (green) or failure (red) |
| ⏱️ **Time Limit** | Episode duration constraint for reaching the goal |

---

## 🚀 Getting Started

### Prerequisites
- Unity 2020.3 or later
- Unity ML-Agents Toolkit
- Python 3.7+ (for ML-Agents training)

### Installation
1. Clone this repository
2. Open the project in Unity
3. Install ML-Agents package via Package Manager
4. Configure training parameters in the YAML config file
5. Run training using `mlagents-learn` command

---

## 📖 Inspiration / Sources  

This project uses Unity's ML-Agents framework for reinforcement learning:
- [Unity ML-Agents Documentation](https://github.com/Unity-Technologies/ml-agents)
- [PPO Algorithm Paper](https://arxiv.org/abs/1707.06347)

Project created by me 😎, Thibault GAREL - [Github](https://github.com/Thibault-GAREL)
