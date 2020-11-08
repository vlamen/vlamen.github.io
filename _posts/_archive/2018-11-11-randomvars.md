---
layout: post
title: Deep representations of low dimensional non-gaussian/intermittent random variables
excerpt: "The aim of this project is to exploit state-of-the-art generative models to learn the probability distribution of random variables connected with mesoscopic representations of rarefied gas flows (obtained via a Direct Simulation Monte Carlo schemes)."
modified: 11/14/2018, 11:00:00
tags: [neural networks, deep learning, density estimation]
comments: false
category: mscproject
---
Deep generative models such as variational autoencoders showed remarkable success in generating new “realistic” data points, e.g. images, resembling the training data. It is understood that this connects with the capability of learning the probability distribution p underlying the training dataset. Generated data would then sample the data space following an approximation of p learned from the training data.
The aim of this project is to exploit state-of-the-art generative models to learn the probability distribution of random variables connected with mesoscopic representations of rarefied gas flows (obtained via a Direct Simulation Monte Carlo schemes). These random variables are defined in low dimensional spaces (usually 18-D) and are highly non-Gaussian.
Notably, in low dimensional spaces the quality of a sampling can be thoroughly checked, as it is computationally feasible to evaluate e.g. histograms or kernel density representations of the sampling. Extensive evaluation of the performance of the model will be a crucial part of the project.
Building a generative models for these probability distributions will bring a substantial speed-up in the simulation of complex rarefied gas flows.
