# Deep Reinforcement Learning for Playing Snake Arcade Game

## Overview
This repository contains deep reinforcement learning agents implemented in PyTorch to play the classic Snake game. The agents use DQN, DDQN, and A2C algorithms to learn policies to maximize the snake's length by collecting apples while avoiding collisions.

## Game Animation

![Gameplay Animation](https://github.com/billodalroy/snake-game/assets/46433931/773aba24-9d17-4643-a119-b260b01ab34d)

The animation above shows the Snake game environment. The snake needs to collect apples to increase its length while avoiding the walls and its own body.

## Algorithms

Three different deep RL algorithms were implemented and compared:

    DQN: Deep Q-Network (Q-Learning)
    DDQN: Double Deep Q-Network (Q-Learning)
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

<img width="846" alt="Test-Results" src="https://github.com/billodalroy/snake-game/assets/46433931/cbb8ef9e-d10d-4457-bdb0-0c6e8819d8df">

The agents were trained for over 100,000 episodes. DDQN achieved the best performance, reaching **10 apples** per episode during evaluation. DQN reached **7 apples**, while A2C only managed **1 apple** per episode.

**DQN:**

<img width="846" alt="DQN" src="https://github.com/billodalroy/snake-game/assets/46433931/8ed26037-0cf4-4bec-92fc-e4e5fd62536c">

Training result: 12 apples per episode,
Test result: 10 apples per episode

**DDQN:**

<img width="846" alt="ddqn" src="https://github.com/billodalroy/snake-game/assets/46433931/bcb54350-d0b5-481a-89bd-1b1b8849a5c5">

Training result: 10 apples per episode,
Test result: 7 apples per episode

**A2C:**

<img width="846" alt="a2c" src="https://github.com/billodalroy/snake-game/assets/46433931/e26393f7-7458-4e83-8533-23d98212cc9f">

Training result: 1 apple per episode,
Test result: 1 apple per episode
