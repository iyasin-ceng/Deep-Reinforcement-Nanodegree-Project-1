# Project : Continuous Control of Deep-Reinforcement Nanodegree
### BY: Imran Yasin

## Description 
For this project, we train a double-jointed arm agent to follow a target location.

<p align="center">
	<img src="images/reacher_gif.gif" width=50% height=50%>
</p>

## Problem Statement 
A reward of +0.1 is provided for each step that the agent's hands is in the goal location.
Thus, the goal of the agent is to maintain its position at
the target location for as many
steps as possible.

The perception space comprises of 33 factors relating to position, revolution, speed, and rakish speeds of the arm. Each activity is a vector with four numbers, relating to forcing the material to two joints. Each passage in the activity vector ought to be a number between - 1 and 1.

The task is episodic, with 1000 timesteps per episode. In order to solve
the environment, the agent must get an average score of +30 over 100 consecutive
episodes.

## Files 
- `Continuous_Control.ipynb`: Notebook used to control and train the agent 
- `ddpg_agent.py`: Create an Agent class that interacts with and learns from the environment 
- `model.py`: Actor and Critic classes  
- `config.json`: Configuration file to store variables and paths
- `utils.py`: Helper functions 
- `report.pdf`: Technical report

## Dependencies
To be able to run this code, you will need an environment with Python 3 and 
the dependencies are listed in the `requirements.txt` file so that you can install them
using the following command: 
```
pip install requirements.txt
``` 

Furthermore, you need to download the environment from one of the links below. You need only to select
the environment that matches your operating system:
- Linux : [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
- MAC OSX : [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
- Windows : [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

## Running
Run the cells in the notebook `Continuous_Control.ipynb` to train an agent that solves our required
task of moving the double-jointed arm.