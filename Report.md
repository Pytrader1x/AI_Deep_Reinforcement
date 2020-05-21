## Report
Reinforcement learning algorithm

1. [Optimized Navigation notebook](https://github.com/Pytrader1x/DeepReinforcementLearning/blob/master/Optimal_DQN_Navigation.ipynb)

2. [Optimized Model](https://github.com/Pytrader1x/DeepReinforcementLearning/blob/master/model.py)

3. [RL Actor Agent](https://github.com/Pytrader1x/DeepReinforcementLearning/blob/master/agent.py)

The learning algorithm used is vanilla Deep Q Learning, DDQN was researched however the results weren't converging so focused on vanilla impletmentation. 

The input is the vector of states as show below:


![](action_space.png)

Deep RL DQN network structure is as follows:

- Fully connected layer - input: 37 (state size) output: 512
- Fully connected layer - input: 512 output 512
- Fully connected layer - input: 512 output: (action size)

Parameters used in DQN algorithm:
- Batch size of 128 to leverage GPU rather than 64

- Starting epsilion: 1.0

- Maximum steps per episode: 1000

- Ending epsilion: 0.01

- Epsilion decay rate: 0.995

- Max number of episodes = 2000
## Results

![](Episode_training.png)

![](Result_episodic_scores.jpg)

## Optimized DQN agent
![](Deep_RL_dqn.gif)

# Future research:

- Ideas for Future Work

- Optimise hyperparameterts to get to a reward of +35 and fast convergence

- In addition we can explore deeper trials of Distributed Distributional Deterministic Policy Gradients and also potentially also trialing
PPO Proximal policy optimization for faster convergence


