# Learning Algorithm
I'm using Deep Q-Network as the learning algorithm to train the model. It contains 2 Fully Connected Layers (64 units) and two RELU Activation Layers. Besides, the "Reply Buffer" is also used in the algorithm to ensure the learning process will take the past learning experience as reference.

Here is an high level overview of the model architecture:  
State --> Fully Connected Layer 1 (64 units) --> Fully Connected Layer 2 (64 units) --> Action

In Deep Q-Network, there are tweo networks that are identical, one is Local Network, another one is Target Network.
Once enough sampling processes are taken and stored in the memory, the algorightm will go for learning process, in which the "Q_Target" is calculated and compared to the "Q_Expected" to come up with the loss, then the algorithm will try to minimize the loss by using "Gradient Descent" approach.


## Hyperparameters
- Buffer Size: 1e5
- Batch Size: 64
- Learning Rate: 5e-4
- GAMMA(discount factor): 0.99
- UPDATE_EVERY(how many t steps will the algorithm update the network): 4
- SEED: 0
- Epsilon Decay: 0.995



# Plot of Rewards
Here is the screenshot for the plot of rewards (scores). it shows that I successfully gain +13 score within 516 consecutive episodes.

<img width="446" alt="Reward Trend_Update" src="https://github.com/Ryan-ZL-Lin/RLND-Navigation/assets/33056320/ca788dd7-b5d0-4833-b4e4-723ead36e854">
<img width="412" alt="Reward Plot_Update" src="https://github.com/Ryan-ZL-Lin/RLND-Navigation/assets/33056320/d248075e-daa2-4aaf-8c4f-a1d5d8c2690d">


# Ideas for furure work
1. Use Doulble DQN to improve the performance.
2. Use Prioritized Experience Reply to improve the performance.
