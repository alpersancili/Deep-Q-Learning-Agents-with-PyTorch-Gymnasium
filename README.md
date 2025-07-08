# Deep-Q-Learning-Agents-with-PyTorch-Gymnasium
This repository showcases my implementation of Deep Q-Learning (DQN) agents, trained to solve environment like FlappyBird-v0, using PyTorch and Gymnasium. It’s a hands-on reinforcement learning project designed to deepen my understanding of Q-learning-based methods in a modular, scalable way. 

Developed under the guidance of the Johnny Code YouTube Channel – A great resource that helped me structure and understand each component of deep reinforcement learning.

**Project Goals**

-Understand and implement Deep Q-Learning (DQN)

-Experiment with extensions like Double DQN and Dueling DQN

-Create a modular agent that can generalize across multiple environments

-Visualize training progress using reward graphs and epsilon decay

-Reproduce results and save the best performing model automatically

**Project Structure**

-agent.py:
The main file that handles environment interaction, agent training, evaluation, and plotting. Reads hyperparameters from a YAML file and can toggle between training and testing modes using command-line arguments.

-dqn.py:
Contains the DQN neural network architecture. Supports both standard DQN and dueling architecture with separate value and advantage streams.

-experience_replay.py:
Implements the Replay Memory using a deque buffer to store and sample past experiences, improving sample efficiency and stability.

-hyperparameters.yml:
A YAML file that allows easy switching between different configurations (e.g., CartPole vs FlappyBird) and tuning hyperparameters like learning rate, batch size, exploration rates, and architecture type.

-launch.json:
VSCode launch configuration for training with a specific hyperparameter set using the integrated terminal.

**Features & Functionality**

-Epsilon-greedy exploration strategy with customizable decay
-Target network synchronization for stabilized learning
-Replay memory sampling
-Real-time graph generation and automatic saving
-Optional rendering during test mode
-Support for CPU and CUDA (manually selectable)
-Easy extension to new environments via the YAML config

**What I Learned**

-How to implement deep reinforcement learning agents from scratch

-Importance of modular design in experimentation-heavy projects

-How epsilon-greedy exploration balances learning and exploitation

-Role of target networks and replay buffers in stable Q-learning

-How to adapt a learning agent to different games/environments

**Acknowledgements**

This project was built and refined by following the Johnny Code YouTube tutorials, which provided clear guidance and strong foundational explanations on reinforcement learning.









