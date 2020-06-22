# Udacity-MADDPG-Tennis
Implementation of an MADDPG agent to solve the Unity Tennis task.

## Task
In this envirnoment two players are tasked to play tennis with each other. The goal for each player is
to hit the ball so that it crosses the net, in which case a reward of +0.1 is granted to the respective player.
On the contrary, if either hits the ball out of bounds or lets it drop to the ground, a reward of -0.01 is received.

Ultimately, this leads to a cooperation between the players to maintain the rally for as long as possible.

At the end of an episode, the maximum of the collected rewards of the two players is counted as the reward of a single episode. The task is considered to be solved if the agent manages to collect an average of 0.5 units over 100 consecutive episodes.

## States
Each player only observes the world partially. Thus, there are two 24-dimensional states at each timestep.

## Actions
The action space consists of two different continuous actions which determine the movement of the tennis rack.

## Getting Started
Everything that is needed is included in the `Tennis.inpynb` notebook.

There is no installation of Unity needed to run the code, you are however required to download
the built of the environment and change the path in the first cell of the Notebook to the location
of it. There are some further Python packages need of which most (if not all) should be automatically
installed by running `!pip -q install ./python` in the first cell of the Notebook.
If this should fail, please install the listed packages manually from your terminal.

## Training the Agent
To train the agent, simply run the Jupyter Notebook. If you wanna tweak details of the models and / or
the agent, just change the hyperparameters within the corresponding cells.


