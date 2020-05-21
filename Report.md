## Report
Reinforcement learning algorithm

1. [Optimized Navigation notebook](https://github.com/Pytrader1x/DeepReinforcementLearning/blob/master/Optimal_DQN_Navigation.ipynb)

2. [Optimized Model](https://github.com/Pytrader1x/AI_Deep_Reinforcement/blob/master/model.py)

3. [RL Actor Agent](https://github.com/Pytrader1x/AI_Deep_Reinforcement/blob/master/agent.py)

The learning algorithm used is vanilla Deep Q Learning, DDQN was researched however the results weren't converging so focused on vanilla impletmentation. 

The input is the vector of states as show below:

![](Start_space.png)

# Install

You can clone the env by running git clone https://github.com/Pytrader1x/AI_Deep_Reinforcement

# Overview
In this env we have a robotic arm with 2 moveable joints which will be the inputs for targeting the robot agents hand to move to the target sphere

Reward: The robotic agent will received a reward of + 0.1 for each step in the training that the robots hand is in the target sphere

Goal: The goal of your agent is to maintain its position at the target location for as many time steps as possible.

Observation Space: The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints.

Action Space: Every entry in the action vector should be a number between -1 and 1.

In order to consider the environment has been solved, the agent must get an average score of +30 over 100 consecutive episodes.


## Results

![](20_armsGif.gif)

![](Result_episodic_scores.jpg)

## Optimized DQN agent
![](optimised_gif.gif)

# Future research:

- Ideas for Future Work

- Optimise hyperparameterts to get to a reward of +35 and fast convergence

- In addition we can explore deeper trials of Distributed Distributional Deterministic Policy Gradients and also potentially also trialing
PPO Proximal policy optimization for faster convergence


