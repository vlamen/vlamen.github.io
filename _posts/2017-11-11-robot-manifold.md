---
layout: post
title: Learning to orient from video pixels 
excerpt: "Deep learning in unsupervised settings for computer vision in robotics"
modified: 07/12/2017, 9:45:24
tags: [unsupervised learning, robotics, computer vision, neural networks, deep learning, metric learning]
comments: false
category: mscproject
---

Deep Learning (DL) methods have shown significant success learning complex model from low level data such as pixel in images or video [1]. In this master project, you will investigate how the little robot Cozmo can learn, by himself, the geometry of the space it lives in, using methods from unsupervised machine-learning. These methods can extract the most important features, and in fact underlying low-dimensional geometry in high-dimensional data [2][3][4]. The goal is to use this constructed geometry to orient it self in the given space.

Cozmo has a front-facing camera, with which it shoots 15-30 pictures per second. These pictures are stored as matrices with gray-scale values. If the room around Cozmo does not change, there are really only four coordinates that, up to noise, completely determine the picture that Cozmo records: Cozmo's xy-coordinates in the plane, its orientation and the tilt of its head. These are easy to identify by us humans as outside observers, but this project is all about letting Cozmo learn this representation by himself.

Once Cozmo can reliably learn the geometry in stationary rooms, you will examine whether it can still find and use the coordinates in practical situations when the room is subject to change. The project aims at investigating whether Cozmo can use the learned representation of the space for the completion of simple tasks, such as parking himself backwards.

This project will be jointly supervised by Jim Portegis and Vlado Menkovski
 
[1] [Mnih, Volodymyr, et al. "Playing atari with deep reinforcement learning." arXiv preprint arXiv:1312.5602 (2013).](https://arxiv.org/abs/1312.5602)

[2] [Coifman, Ronald R., and Stéphane Lafon. "Diffusion maps." Applied and computational harmonic analysis 21.1 (2006): 5-30.](http://www.sciencedirect.com/science/article/pii/S1063520306000546)

[3] [Kingma, Diederik P., and Max Welling. "Auto-encoding variational bayes." arXiv preprint arXiv:1312.6114 (2013).](https://arxiv.org/abs/1312.6114)

[4] [Roweis, Sam T., and Lawrence K. Saul. "Nonlinear dimensionality reduction by locally linear embedding." science 290.5500 (2000): 2323-2326.](http://science.sciencemag.org/content/290/5500/2323)
