---
layout: post
title: Curiosity driven Deep Reinforcement Learning 
excerpt: "In Deep Reinforcement Learning (DRL), the concept of curiosity can be leveraged to improve the performance and robustness of learning agents. There is room for investigation and progress here, in terms of evaluating the currently available approaches in different settings, and in augmenting then or developing completely new approaches."
modified: 17/11/2018, 9:00:24
tags: [neural networks, deep learning, reinforcement learning]
comments: false
category: mscproject
---
**TLDR;** In Deep Reinforcement Learning (DRL), the concept of curiosity can be leveraged to improve the performance and robustness of learning agents. There is room for investigation and progress here, in terms of evaluating the currently available approaches in different settings, and in augmenting then or developing completely new approaches.

**Project Description:**
In Reinforcement Learning (RL), an unsupervised agent attempts to perform a task in an environment to the best of its ability. During each try, it receives feedback from the environment based on how well it is performing the task. By processing this feedback and incorporating the obtained lessons into future attempts, the agent get increasingly better at the task. In Deep Reinforcement Learning (DRL), that agent is typically a neural network. Neural network-based agent have shown great potential in RL, to the extent that the majority of the research in this area is related to DRL. In a typical RL setting, the agent takes discrete steps until it has completed the task (or has failed in some way), with each step being rewarded or punished by the environment. However, in many settings, including most real-life settings, most of the steps do not have a natural reward or punishment associated with them. Instead, most steps are neutral, meaning that it is not possible to determine whether they are specifically good or bad. This causes problems for many learning agents, since they use the rewards to guide their path through the space of all possible trajectories (sequence of steps). 

To address this issue, some research in DRL has recently turned to the concept of curiosity. Instead of basing the reward of a step solely on how well the task at hand is being performed, the agent can receive an additional small reward for taking a step that results in it encountering a previously unseen situation. In practice curiosity is defined as failure of the agent to predict the consequences of its own decisions [1][2]. Although this makes the agent more robust in situations with many neutral steps, it has problems of its own. Specifically, many environments are not static, they change over time. The curiosity of an agent can be captured by a small, dynamic part of the environment, effectively deadlocking the agent [3]. An example of this from a recent work is the "noisy TV": An agent with curiosity is exploring a maze in an attempt to find the exit. However, somewhere in the maze it encounters a TV which displays constantly changing images. Each new image triggers a new observation in the agent, which then has no reason to move, since it is being rewarded for curiosity. To remedy this weakness, it was recently proposed to give the agent a memory of observations [4]. Each new observation is stored in memory, and if an observation is already in memory, it no longer triggers a curiosity reward. While this makes the agent more robust against getting stuck, it is not an ideal solution. In large environments, an agent may have to memorize thousands, if not millions of observations. This may not only be infeafsible memory-wise, it will also cause performance issues, as each new observation needs to be compared to each observation in memory.

- Improving the current curiosity-based approaches or developing a competitive alternative
- Comparing different curiosity-based approaches
- Evaluating performance of curiosity-based approaches in environments that have no rewards at all
- Investigate the influence on performance of curiosity-based approaches in cases of very long decision horizons

[1] https://pathak22.github.io/noreward-rl/

[2] https://blog.openai.com/reinforcement-learning-with-prediction-based-rewards/

[3] https://pathak22.github.io/large-scale-curiosity/

[4] https://ai.googleblog.com/2018/10/curiosity-and-procrastination-in.html
