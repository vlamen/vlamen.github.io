---
layout: post
title: Anomaly Detection with Bayesian Networks and Generative Models 
excerpt: "Anomaly Detection with Bayesian Networks and Generative Models..."
modified: 11/05/2020, 10:35:24
tags: [Machine Learning, Bayesian networks, Generative Models, Anomaly detection, embeddings for sparse tabular data]
comments: false
category: mscproject
---

Thermo Fisher is a company that, among other things, builds electron microscopes. Their MSD Service Innovation department would like to be able to detect anomalies in the operations of those microscopes based on sensor data, event logs, and machine settings. Our goal is to help them do explainable anomaly detection in an unsupervised or semi-supervised way.
 
Because the different sensors are registered at different frequencies, and different events trigger different logging behaviour, the dataset consists of very sparse tabular data. We want to embed this sparse tabular data into a small number of meaningful signals. Based on these signals we want to then detect and explain anomalies.
 
Because not all machines have the same sensors and subsystems, and because the context in which the machines operate varies, the model we use needs to be flexible. This is where Bayesian Networks come into play: they provide a way of building models that can combine information from different sources and can handle unknown and unobserved variables. The end goal is to not only detect but also explain anomalies in terms of partially provided labels. 
 
This project may be also done as a internship with Thermo Fisher, conditioned on their approval.  

Supervisor: Vlado Menkovski, Mike Holenderski, Simon Koop



