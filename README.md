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

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the DRLND GitHub repository, in the `p1_navigation/` folder, and unzip (or decompress) the file. 


## Instruction
Open Navigation.ipynb and execute the cell one by one, you will go through the traning code and see the final traning outcome as a chart. The final model weights is saved in **model.pt**.

### Training Code: Navigation.ipynb
1: Setup the environment and install packages in the workspace.

2: Start the environment

3: Examine the state and action space.

4: Training Code implementation
- Initiate the agent (with Epsilon Decay parameter)  
- Initiate the environment  
- Train the agent iwith DQN  
- Plot out the average score during the training process (2000 episodes)

### AI Agent Code: dqn_agent.py
It contains the following parts
- the Class and Functions that describe how Deep Q-Network agent works with Reply Buffer
- the hyper parameters such as Buffer Size, Batch Size, Learning Rate, etc.

### Neural Network Architecture: model.py
- It uses Pythorch as the Frmework.
- Totally two Fully Connected layers and two RELU Activation Layers are used to construct the model architecture.

### Trained Model Weights
It's saved in mode.pt.
