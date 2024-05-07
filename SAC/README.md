# Soft Actor-Critic (SAC) for Pendulum Control

This repository contains an implementation of the Soft Actor-Critic (SAC) algorithm applied to the pendulum control problem. The goal of the pendulum control problem is to control a pendulum to reach and maintain an upright position while minimizing energy consumption.

## Overview

The SAC algorithm is a reinforcement learning technique used for training agents to make sequential decisions in continuous action spaces. In this implementation, we use SAC to train an agent to control a pendulum to stabilize it in the upright position.

## Implementation Details

### `SAC_Agent`

The `SAC_Agent` class contains the implementation of the SAC algorithm. It includes methods for initializing the agent, choosing actions based on the policy distribution, memorizing experiences, and training the agent.

### `ReplayBuffer`

The `ReplayBuffer` class implements a replay buffer for storing and sampling experiences for training the agent. This helps in reducing the correlation between consecutive experiences and stabilizing the training process.

### Pendulum Dynamics

The `simulate_pendulum` function simulates the dynamics of the pendulum given the current state and control input (action). It returns the next state of the pendulum based on the dynamics equations.

### `PolicyNetwork`

The `PolicyNetwork` class defines the policy network architecture. It is a neural network that takes the current state as input and outputs mean and log standard deviation of the action distribution.

### `QNetwork`

The `QNetwork` class defines the Q-network architecture. It is a neural network that takes the current state and action as input and outputs the state-action values (Q-values).
