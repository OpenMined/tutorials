## Create Reinforcement Learning Demos with OpenMined


### What's Reinforcement Learning?

You have probably heard about AI breackthroughs where an AI agent is able to play [Attari games](https://deepmind.com/research/publications/playing-atari-deep-reinforcement-learning/) or [beat world champions at Go](https://deepmind.com/research/alphago/). These accomplishments have all been made possible because of one specific machine learning area: Reinforcement Learning. 

Reinforcement Learning (RL) consists of learning best actions based on reward or punishment. The RL agent learns by interacting with an environment (e.g. an Attari game or Go board) through many trials and errors. Its actions take place in a state, which describes the current situation. For example, on a Go board, the state is the positions of all the pieces on the board. At every state, the RL agent receives a reward that can be positive or negative based on the action taken. Over time, the RL agent will learn a sequence of actions that leads to a long-term reward.  

To continue to learn more about Reinforcement Learning, you can read this excellent [blog post](http://karpathy.github.io/2016/05/31/rl/) written by Andrej Karpathy.


### Why Apply Reinforcement Learning with OpenMined?

In order to be as portable as possible, OpenMined has built its backend on the game development platform Unity. Data Scientists are therefore able to train their model quickly by accessing GPUs across a wide range of platforms - from Xbox, Mac OS X, to mobile platforms like iOS and Android. This implementation leads to several benefits for RL. As mentioned in the introduction, Agents are trained in a game environment most of the time. Luckily with Unity, you can create all the environments you can imagine. It's therefore an amazing platform for AI/Research development. You can learn more about the Unity research team's latest innovations on [Unity's blog](https://blogs.unity3d.com/2017/09/19/introducing-unity-machine-learning-agents/) and on their [GitHub page](https://github.com/Unity-Technologies/ml-agents).

<p align="center">
	<img width="460" height="300" src="https://blogs.unity3d.com/wp-content/uploads/2017/09/image2-2.gif"> 
</p>

So because OpenMined uses Unity as a backend, a game developer, for example, could train a RL agent for her game directly on her console instead of having to use a cloud service to access GPUs. 

Another benefit of OpenMined is that you could train your RL agent concurrently on several devices (computer, gaming console, etc) by using [OpenMined Grid](https://github.com/OpenMined/Grid). This approach could drastically speed up the agent's training.

### Different ways to contribute

Here are a couple ideas for how you can contribute to OpenMined:

#### Find an existing demo and replicate it using PyTorch or Keras interface

OpenMined has created a PyTorch and Keras interface to make it as easy as possible for Data Scientists to create their model. One way to contribute would be to find an existing RL demo and replicate it using the PyTorch or Keras interface. You can find two examples here: 
* [CartPole-v0 with PyTorch interface](https://github.com/OpenMined/OpenMined/blob/master/notebooks/torch/PyTorch%20Interface%20Demo.ipynb)
* [MountainCar-v0 with Keras interface](https://github.com/OpenMined/OpenMined/blob/master/notebooks/keras/Reinforcement%20Learning%20with%20Keras%20DQN.ipynb)

For these demos you could experiment with different RL algorithms on the [Gym environments](https://gym.openai.com/envs/) from [OpenAI](https://openai.com/):

* Policy Gradients
* Deep Q-network
* Actor Critic Algorithm 
* Etc.

In order to make your demos work with OpenMined, you might have to perform the following steps:
* Install OpenMined and PySift. Instructions are [here](https://github.com/OpenMined/tutorials/tree/master/installation/OpenMined).
* Add new functions to the PyTorch and Keras interface. If the function exists in PySyft but is missing in the PyTorch or Keras interface, you can add the function [here](https://github.com/OpenMined/PySyft/tree/master/syft/interfaces).
* If the function doesn't already exist, you can add it to the OpenMined backend and PySyft library. Here are the [instructions](https://github.com/OpenMined/tutorials/blob/master/intermediate/adding-a-new-tensor.markdown).
* Identify and fix any bottlenecks in the current implementation that could improve the performance of the Deep Learning framework.

#### Create your own Unity environment and train your agent using PyTorch or Keras interface

Another way to contribute would be to create your own Unity environment, or use an existing one, to train your agent using PyTorch or Keras interface.

OpenMined has already created a proof of concept showing how OpenMined can be a plugin into a separate Unity framework to train Reinforcement Learning agents. You can find the repository with Unity Machine Learning agents powered by OpenMined [here](https://github.com/OpenMined/ml-agents). There are two excellent examples already implemented: 1)An agent, blue square, learns how to move to one direction. 2)A pole learns to remain upright. 

<p float="left">
  <img src="https://media.giphy.com/media/xUOwGkgPytuUuYpfiM/giphy.gif" height="170" width="300" />
  <img src="https://media.giphy.com/media/l4pTiIojVSurPWg12/giphy.gif" height="170" width="300" /> 
</p>

The notebooks for these examples are in this [folder](https://github.com/OpenMined/OpenMined/tree/master/notebooks/ml-agents). 


#### Replicate Unity RL Demos Using PyTorch or Keras Interface

Another idea would be to replicate an existing Unity RL demo using OpenMined. In the [Unity Github repository](https://github.com/Unity-Technologies/ml-agents), the Unity research team shared an awesome demo where they trained multiple independent agents to balance a ball on a platform. 

<p align="center">
<img width="460" height="300" src="https://blogs.unity3d.com/wp-content/uploads/2017/12/image12.gif"> 
</p>

This demo was implemented using [TensorFlow](https://github.com/Unity-Technologies/ml-agents/tree/master/python/ppo). You could replace the Tensorflow implementation with the PyTorch interface. 

#### Let's chat!
I hope you found this helpful and interesting. Let's continue this discussion on [openmined.slack.com](https://openmined.slack.com/join/shared_invite/enQtMjU5MzE5ODk4MTc3LWI2ZGE1ODc1YjdkZDJiNjdmYTdkZmE4ZTY5N2NkNDgxZjUyNjgxMTVhMmJkOTZhZjEyZDA3MTM2MThkZWVhMjg)

