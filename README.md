# RLND-Navigation
Navigation project for Reinforcement Learning Nanodegree


## Introduction
In this project, the environment is built on top of **Unity ML-Agents**. The project goal is to implement an AI agent to learn how to navigate and collect yellow bananas in a large, square world.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to: 
0 - move Forward.
1 - move backward.
2 - turn left.
3 - turn right.

The task is episodic, and the environment is considered sovled when the trained agent can reach average +13 score wihtin 1800 consecutive episodes.


## Getting Started

### Training Code: Navigation.ipynb
1: Setup the environment and install packages in the workspace.
2: Start the environment
3: Examine the state and action space.
4: Training Code implementation
  4.1: Initiate the agent (with Epsilon Decay parameter)
  4.2: Initiate the environment
  4.3: Train the agent iwith DQN
  4.4: Plot out the average score during the training process (2000 episodes)

### AI Agent Code: dqn_agent.py
It contains the following parts
- the Class and Functions that describe how Deep Q-Network agent works with Reply Buffer
- the hyper parameters such as Buffer Size, Batch Size, Learning Rate, etc.

### Neural Network Architecture: model.py
- It uses Pythorch as the Frmework.
- Totally three Fully Connected layers and two RELU Activation Layers are used to construct the model architecture.

### Trained Model Weights
It's saved in mode.pt.

## Instruction
Open Navigation.ipynb and execute the cell one by one, you will go through the traning code and see the final traning outcome as a chart. The final model weights is saved in **model.pt**.

