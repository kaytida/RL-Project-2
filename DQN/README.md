# Deep Q-Network (DQN) for Pendulum Swing-Up Problem

This repository contains an implementation of the Deep Q-Network (DQN) algorithm applied to the pendulum swing-up problem. The goal of the pendulum swing-up problem is to control a pendulum to swing from its initial downward position to the upright position (pendulum angle close to vertical) while minimizing the control effort.

## Overview

The DQN algorithm is a reinforcement learning technique used for training agents to make sequential decisions in environments with discrete action spaces. In this implementation, we use DQN to train an agent to control a pendulum to swing up to the vertical position.

## Implementation Details

- **DQNAgent**: The `DQNAgent` class contains the implementation of the DQN algorithm. It consists of methods for initializing the agent, choosing actions based on an epsilon-greedy policy, memorizing experiences, and training the agent.




- **ReplayBuffer**: The `ReplayBuffer` class implements a replay buffer for storing and sampling experiences for training the agent. It helps in reducing the correlation between consecutive experiences and stabilizing the training process.

- **Pendulum Dynamics**: The `simulate_pendulum` function simulates the dynamics of the pendulum given the current state and control input (action). It returns the next state of the pendulum based on the dynamics equations.

- **DQN**: The policy network architecture is defined in the `DQN` class. It is a neural network that takes the current state as input and outputs Q-values for each action.
- 
![q_net](https://github.com/kaytida/RL-Project-2/assets/72248519/6ec113a7-bfa2-4a66-b8eb-9d8425f904c7)

## Animation of the Pendulum Swing-up

https://github.com/kaytida/RL-Project-2/assets/72248519/86d0f8c7-ca8f-4d18-b6b9-b92ec7e87ba8
