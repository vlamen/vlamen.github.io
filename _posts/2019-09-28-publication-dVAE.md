---
layout: post
title: Diffusion Variational Autoencoders 
authors: Luis A. Pérez Rey, Vlado Menkovski, Jacobus W. Portegies
excerpt:  Rey, L.A., Menkovski, V., & Portegies, J.W. (2019). Diffusion Variational Autoencoders. ArXiv, abs/1901.08991.
modified: 06/9/2019, 9:00:24
tags: [computer vision, convolutional neural networks, evolutionary computing]
comments: true
category: publication
---

**Authors: Luis A. Pérez Rey, Vlado Menkovski, Jacobus W. Portegies**

**Abstract** 
A standard Variational Autoencoder, with a Euclidean latent space, is structurally incapable of capturing topological properties of certain datasets. To remove topological obstructions, we introduce Diffusion Variational Autoencoders with arbitrary manifolds as a latent space. A Diffusion Variational Autoencoder uses transition kernels of Brownian motion on the manifold. In particular, it uses properties of the Brownian motion to implement the reparametrization trick and fast approximations to the KL divergence. We show that the Diffusion Variational Autoencoder is capable of capturing topological properties of synthetic datasets. Additionally, we train MNIST on spheres, tori, projective spaces, SO(3), and a torus embedded in R3. Although a natural dataset like MNIST does not have latent variables with a clear-cut topological structure, training it on a manifold can still highlight topological and geometrical properties.

**[Arxiv link](https://arxiv.org/abs/1901.08991)**
