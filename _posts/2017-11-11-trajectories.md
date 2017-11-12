---
layout: post
title: Learning efficient representations for pedestrian trajectories 
excerpt: "Developing models for the shape of pedestrian trajectories can allow for developing pattern recognition methods for this type of data. Due to the high dimensionality of such time series data we consider deep recurrent neural network models."
modified: 11/12/2017, 11:00:00
tags: [lstm, time series, neural networks, deep learning, recurrent neural networks, pedestrian tracking, trajectory modelling]
comments: false
category: mscproject
---

Analysis of the shape of sequences of measurements is of interest in different domains and applications. Tracking movement of objects, analyzing shape of geographical features and particularly when large number of objects or trajectories demonstrate certain emergent properties.

In recent years, at Eindhoven University of Technology, a number of pioneering experimental observations of crowds have been performed with high spatial and temporal resolution and with the ability to reconstruct exhaustively the trajectories of individuals inside crowds [1][2]. As the trajectories are produced by tracking different people with different roles in the given context they also demonstrate different properties. A self-lerning solution that automatically uncovers the patterns in the traffic and finds clusters of trajectories is motivated. It is furthermore suitable to have a solution with which a domain expert can interact and provide a supervision signal that would guide the learning process. In this project we propose investigation of developments in sequence to sequence modelling with Deep Learning, particularly with recurrent neural network auto-encoders[3] for learning representations of recorded trajectories. The goal of this project is to build upon the developed representations to enable pattern recognition methods on the high dimensional time-series data. 

We consider expanding the scope of any developed methods to other time series data sets where the shape of the sequence is of interest.

This project will involve supervision from Alessandro Corbetta and Vlado Menkovski
 
[1] [](A. Corbetta, C. Lee, R. Benzi, A. Muntean, F. Toschi. Fluctuations around mean walking behaviours in diluted pedestrian flows, Phys. Rev. E. 95, 032316, 2017
)

[2] [](A. Corbetta, J.A. Meeusen, C. Lee, F. Toschi. Continuous measurements of real-life bidirectional pedestrian flows on a wide walkway, Proceedings of Pedestrian and Evacuation Dynamics 2016, 18-24, 2016)

[3] [](Sutskever, Ilya, Oriol Vinyals, and Quoc V. Le. "Sequence to sequence learning with neural networks." Advances in neural information processing systems. 2014.)