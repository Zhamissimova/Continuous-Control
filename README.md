# Continuous-Control
Submission of second project in Deep Reinforcement Learning Nanodegree Program in Udacity
## Background
The goal of the project is to maintain double-jointed arm position at the target location for as many time steps as possible.This is a continuous reinforcement learning task and Deep Deterministic Policy Gradients (DDPG) algorithm is used to solve this Reacher environment problem. This DDPG algorithm has actor-critic architecture, where actor learns policy function and controls how our agent acts. Critic, on the other hand, learns value function and measures how good these actions are. Therefore, actor-critic algorithms combine value-based and policy gradient approaches.

## Environment
This “Reacher” environment is provided by The Unity Machine Learning Agents Toolkit (ML-Agents). This Unity plugin, which Machine Learning Agents (ML-Agents) is an open-source Unity plugin that enables games and simulations to serve as environments for training intelligent agents. In other words, Unity gives a chance for machine learning scientists to train their algorithms and visualize how the trained agent is performing through animations (which is really cool and fun!). 
### State space: 33. 
It includes position, rotation, velocity, and angular velocities of the robotic arm..
### Action space: 4, continuous.
It corresponds to torque applicable to two joints.
### Reward.
A reward of +0.1 is provided for each step that the agent's hand is in the goal location.
### Number of agents: 20.
20 identical agents, each has its own copy of the environment, thus distributing task of gathering experience and increasing learning speed.

### Task
The task is episodic, and in order to solve the environment, the average score among agents over 100 consecutive episodes must be higher than 30.
The problem was solved with DDPG algorithm in 153 episodes.
The code was written in python v3, using pytorch. GPU is provides fairly good speed up. 

### How to run:
There are 5 files required to run the project. 
* Continuous_Control.ipynb is a Jupiter notebook with main code and the only file that need to be run.
* ddpg_agent.py is a python script which contains our actor-critic reinforcement learning algorithm.
* model.py is a python script which contains our 2 separate deep neural networks.
* checkpoint_actor.pth and checkpoint_critic.pth are our files with saved weights.

### Useful links:
* You can study DDPG paper [here](https://arxiv.org/abs/1509.02971)
* Reacher Environment [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher)
* More about Unity agents [here](https://github.com/Unity-Technologies/ml-agents)
* More about Udacity Deep Reinforcement Learning [here](https://udacity.com)
* If you got really excited about RL, then you can read book written by “father” of Reinforcement Learning [here](http://incompleteideas.net/book/the-book-2nd.html)
