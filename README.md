# rl-testing

  This is an ongoing personal project to make reinforcement learning experimentation as efficient and modular as possible. Implement algorithms (DQN, DDPG, etc) by filling out the provided PyTorch template for agents, and modify hyperparameters (environments, learning rate, discount rate, number of epochs, number of episodes, etc) in the `config.py` file. Agents are tested in OpenAI gym environments, and smoothed reward plots of median epoch rewards re automatically generated. Models with the best average deterministic performance over a number of episodes will have their weights automatically saved in a specified directory. [check out the graphs](#graphs) [the renderings](#renderings)


# Prerequisites

Here are the required libraries to run the scripts:
* Python 3.6
* NumPy
* OpenAI gym
* PyTorch 0.4+
* Matplotlib

I personally use and highly recommend the [Anaconda Distribution](https://www.anaconda.com/what-is-anaconda/) and the conda package installer to ensure compatibility in the dependencies.

# Implementing Custom Agents


# The `config.py` File


# Generated Files


#### Renderings <a name="renderings"></a>
*Trained DDQN Agent, CartPole-v1*
![alt text](https://github.com/kphng/rl-testing/blob/master/assets/giphyCartPole.gif)

*Trained DDQN Agent, Acrobot-v1*
![alt text](https://github.com/kphng/rl-testing/blob/master/assets/giphyAcrobot.gif)

*Trained DDQN Agent, MountainCar-v0 (actions repeated 10x)*
![alt text](https://github.com/kphng/rl-testing/blob/master/assets/giphyMountainCar.gif)

#### Graphs <a name="graphs"></a>

Training graphs are automatically created and saved after the training process. After each epoch (batch of episodes) of training, the specified agent deterministically generates a number of rollouts. The resulting smoothed median rewards are plotted, with the interquartile range (25th to 75th percentile) filled in.

![alt text](https://github.com/kphng/rl-testing/blob/master/assets/dqn_ddqn_classic_control.png)
