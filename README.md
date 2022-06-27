# reacher-continuous-control-p2-drlnd
Deep reinforcement learning nanodegree project 2

[//]: # (Image References)
<!-- [image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent" -->
[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"



# Introduction
This project is part of Udacity Deep Reinforcement Learning Nanodegree. In this project we will train a double jointed arm to follow the target as it moves using Unity ML environment.

![Trained Agent][image1]

# Objective of the project (Version 1)- 
A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The task is episodic, and in order to solve the environment, your agent must get an average score of +30 over 100 consecutive episodes.

## State Space and Action Space- 

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

# Requirements - 

1. First requirement to run this project is to setup drlnd repository. Follow the instructions mentioned on their github repository - [link](https://github.com/udacity/deep-reinforcement-learning#dependencies)

2. After creating a new environment and installing drlnd repository and its dependencies, clone this repo and run the following command to install all the python libraries.

```bash
git clone https://github.com/milind97/reacher-continuous-control-p2-drlnd.git
cd reacher-continuous-control-p2-drlnd
pip install -r requirement.txt
```
3. After this you will also need Unity ML agents environment for the simulation to run. Download the environment from one of the links below.  You need only select the environment that matches your operating system

    - **_Version 1: One (1) Agent_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

    - (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    - (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) and then download the environment for the **Linux** operating system above.
    
4. Place the downloaded file into "data" folder for this repository.

# Project Structure - 

- src
    - reacher_agent.py
    - reacher_model.py
- data
    - checkpoint_actor.pth
    - checkpoint_critic.pth
- Continuous_Control.ipynb
- README.md
- Report.md
- requirements.txt


This repository contains 2 folders - 
1. `src` - This folder has all the required code to train the agent.
2. `data` - This folder contains the saved model weights for the trained agent.
3. Continuous_Control.ipynb - This jupyter notebook has codes to train the agent using ddpg algorithm and to run the trained agent.
4. README.md - Contains intructions to use this repository
5. Report.md - Contains information about the algorithm used to train the agent.

# Steps to run it

1. Install all the dependencies and run the cells in Continuous_Control.ipynb jupyter notebook.



