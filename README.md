# AI_Deep_Reinforcement
Deep RL for continuous space robotic arm
![](20_armsGif.gif)

# Goal

In this project, I build a reinforcement learning (RL) agent that controls a robotic arm within Unity's Reacher environment. The goal is to get 20 different robotic arms to maintain contact with the green spheres.

A reward of +0.1 is provided for each timestep that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

[version 1] A single agent receives an average reward (over 100 episodes) of at least +30, or
[version 2] the agent is able to receive an average reward (over 100 episodes, and over all 20 agents) of at least +30.

# Summary of Environment

Set-up: Double-jointed arm which can move to target locations.
Goal: Each agent must move its hand to the goal location, and keep it there.
Agents: The environment contains 20 agents linked to a single Brain.
Agent Reward Function (independent):
+0.1 for each timestep agent's hand is in goal location.
Brains: One Brain with the following observation/action space.
Vector Observation space: 33 variables corresponding to position, rotation, velocity, and angular velocities of the two arm Rigidbodies.
Vector Action space: (Continuous) Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.
Visual Observations: None.
Reset Parameters: Two, corresponding to goal size, and goal movement speed.
Benchmark Mean Reward: 30


# Approach

Here are the high-level steps taken in building an agent that solves this environment.

Evaluate the state and action space.

Establish performance baseline using a random action policy.

Select an appropriate algorithm and begin implementing it.

Run experiments, make revisions, and retrain the agent until the performance threshold is reached.

# Solving the Environment

The task is episodic, and in order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

# Setting up the environment

The environment can be downloaded from one of the links below for all operating systems

- Linux: - [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)

- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)

- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)

- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

- For AWS: To train the agent on AWS (without enabled a virtual screen), use this link to obtain the "headless" version of the environment. The agent can not be watched without enabling a virtual screen, but can be trained. (To watch the agent, one can follow the instructions to enable a virtual screen, and then download the environment for the Linux operating system above.)
