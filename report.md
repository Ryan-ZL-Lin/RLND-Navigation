# Learning Algorithm
I'm using Deep Q-Network as the learning algorithm to train the model. It contains 2 Fully Connected Layers (64 units) and two RELU Activation Layers. Besdies, the "Reply Buffer" is also used in the algorithm to ensure the learning process will take the past learning experience as reference, please see dqn_agemnt.py for further details.

State --> Fully Connected Layer 1 (64 units) --> Fully Connected Layer 2 (64 units) --> Action

## Hyperparameters
- Buffer Size: 1e5
- Batch Size: 64
- Learning Rate: 5e-4
- GAMMA(discount factor): 0.99
- UPDATE_EVERY(how many t steps will the algorithm update the network): 4
- SEED: 0
- Epsilon Decay: 0.995



# Plot of Rewards
Here is the screenshot for the plot of rewards (scores). it shows that I successfully gain +13 score within 600 consecutive episodes.
<img width="466" alt="Reward Trend_New" src="https://github.com/Ryan-ZL-Lin/RLND-Navigation/assets/33056320/35abb6de-518e-4a9f-9dd4-fb5ff18e5dd9">
<img width="493" alt="Reward Plot_New" src="https://github.com/Ryan-ZL-Lin/RLND-Navigation/assets/33056320/9a01fcf3-52c5-48d7-b017-2d4288bd7c35">



# Ideas for furure work
1. use Doulble DQN to improve the performance.
2. use Prioritized Experience Reply to improve the performance.
