## Project Details

In this project I train a DQN Deep Reinforcement Learning Agent to improve it's performance in a Unity (https://unity.com/) powered environment.
The environment is a large, square world and the agent is trained to navigate and collect bananas.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions.

The action space has four discrete actions, corresponding to:

- move forward
- move backward
- turn left
- turn right

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

## Software Dependencies

The project was done using python 3 and has the following library dependencies that can be installed using pip:

- unityagents
- numpy
- torch
- matplotlib

## File Descriptions

- Navigation.ipynb - jupyter notebook used to open environment, instantiate and train agent, and save trained model parameters.
- model.py - python module containing Q-Network architecture class.
- dqn_agent.py - python module containing DQN Agent, and Replay Buffer classes.
- checkpoint.pth - saved trained model parameters.
- Report.md - explains the model parameters, training, and potential future improvements.

## Instructions

To run the code and train the model yourself you'll need to download the Unity environment as well Navigation.ipynb, model.py, and dqn_agent.py from this repository.

Open the Navigation.ipynb jupyter notebook in your browser and run the code cells from top to bottom. In the notebook you'll see a visualization of the agent learning the task and after the agent has scored an average of at least +13 over 100 consecutive episodes the agent's model parameters will be saved to a .pth file.
