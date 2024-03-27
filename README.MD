# Policy_gradient_CartPole_and_PixelCopter

This repo implements Policy Gradient from scratch and solves the CartPole and PixelCopter environments. 

## What is Policy Gradient? 
Policy Gradient is a policy-based method. The basic idea is that we have a parameterized policy that we try to update to ensure the policy chooses actions that are more optimal. We use an objective function to measure the performance of our policy. We then essentially use the objective function as a loss function for our policy fucntion and update parameters on our policy based on the gradient of our objective function, hence the gradient portion of the policy gradient.
## Pre-requisites
```
pip install torch
```
```
pip install gym
```
```
pip install gym_ple
```
```
pip install tqdm
```
## About CartPole-v1
CartPole is the quintessential RL environment. In this environment we control a cart that has a pole attached to a unactuated joint on the cart. The pole starts at an upright position at the start of the episode. Our goal is to move the cart left and right such that we keep the pole in the upright positon without the end of the pole touching the ground. We receive a reward of +1 for each step that our agent takes. The episdoe terminated when the pole touches the ground or the cart moves away from the frame. 
## About Pixelcopter
The Pixelcopter environment is simplified version of the Flappy Bird game. Our agent must move through a cavern and avoid obstacles. The game is side scrolling meaning that the environment always moves to the right, with the obstacles changing. The agent can only move up or not take any actions causing the agent to move down due to gravity. The agent receives a reward of +1 for each vertical block it clearns, and a reward of -1 if it hits a vertical block at which point the episode also ends. 
