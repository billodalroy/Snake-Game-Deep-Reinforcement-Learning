# Deep Reinforcement Learning for Playing Snake Arcade Game

## Overview
This repository contains deep reinforcement learning agents implemented in PyTorch to play the classic Snake game. The agents use DQN, DDQN, and A2C algorithms to learn policies to maximize the snake's length by collecting apples while avoiding collisions.

## Game Animation

The animation above shows the Snake game environment. The snake needs to collect apples to increase its length while avoiding the walls and its own body.

## Algorithms

Three different deep RL algorithms were implemented and compared:

    DQN: Deep Q-Network
    DDQN: Double Deep Q-Network
    A2C: Advantage Actor-Critic

DQN and DDQN use deep neural networks to approximate the Q-value function. A2C uses separate actor and critic networks.

## Getting Started

Each of the algorithms have a distinct jupyter notebook. To run the code, you will need Python 3 nand run the following libraries installed:

- PyTorch
- Gym
- NumPy
- Matplotlib

Simply open the notebook and run all cells to train each agent from scratch and evaluate them.

## Results

The agents were trained for over 100,000 episodes. DDQN achieved the best performance, reaching **10 apples** per episode during evaluation. DQN reached **7 apples**, while A2C only managed **1 apple** per episode.

**DQN:**

Training result: 12 apples per episode,
Test result: 10 apples per episode

**DDQN:**

Training result: 10 apples per episode,
Test result: 7 apples per episode

**A2C:**

Training result: 1 apple per episode,
Test result: 1 apple per episode
