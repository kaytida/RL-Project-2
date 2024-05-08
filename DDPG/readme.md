# DDPG AGENT
Contains the Implementation of Deep Deterministic Policy Gradient algorithm. Integrates the actor, critic, replay buffer, and training procedure into a cohesive DDPG agent for solving the pendulum swing-up problem.

# Actor 
Defines the actor neural network model responsible for learning the policy function that maps states to actions.

# Critic
Defines the critic neural network model responsible for learning the Q-value function that estimates the expected return given a state-action pair.

# Simulate Pendulum 
Simulates the dynamics of the pendulum system based on the current state and action, returning the next state of the system.

# OrnsteinUhlenbeckNoise
To alter the action predicted by the Actor to avoid over-fitting.Implements Ornstein-Uhlenbeck process noise for exploration during action selection.
