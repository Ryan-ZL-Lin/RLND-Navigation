# Learning Algorithm
I'm using Deep Q-Network as the learning algorithm to train the model. It contains 3 Fully Connected Layers and two RELU Activation Layers. Besdies, the "Reply Buffer" is also used in the algorithm to ensure the learning process will take the past learning experience as reference, please see dqn_agemnt.py for further details.


# Plot of Rewards
Here is the screenshot for the plot of rewards (scores). it shows that I successfully gain +13 score within 600 consecutive episodes.

# Ideas for furure work
1. use Doulble DQN to improve the performance.
2. use Prioritized Experience Reply to improve the performance.
