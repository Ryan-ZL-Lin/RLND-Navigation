# Learning Algorithm
I'm using Deep Q-Network as the learning algorithm to train the model. It contains 3 Fully Connected Layers and two RELU Activation Layers. Besdies, the "Reply Buffer" is also used in the algorithm to ensure the learning process will take the past learning experience as reference, please see dqn_agemnt.py for further details.


# Plot of Rewards
Here is the screenshot for the plot of rewards (scores). it shows that I successfully gain +13 score within 600 consecutive episodes.
![Reward Plot](https://github.com/Ryan-ZL-Lin/RLND-Navigation/assets/33056320/5695ae1e-1ddf-4e05-8a48-a64aa7e3dbff)

# Ideas for furure work
1. use Doulble DQN to improve the performance.
2. use Prioritized Experience Reply to improve the performance.
