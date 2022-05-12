---
layout: post
title: Learnable and interpretable priors for VAEs 
excerpt: "In a VAE, we typically have a fixed prior distribution p(z) on the latent space, which the encoder q(z|x) tries to match. However, in practice, the actual distribution of codes according to the encoder (taken over all datapoints) typically doesn’t actually resemble the prior distribution."
modified: 02/11/2021, 10:35:24
tags: [Deep learning, generative models, neural networks, VAE, Variational Auto Encoders, energy based models, EBM]
comments: false
category: mscproject
---

In a VAE, we typically have a fixed prior distribution p(z) on the latent space, which the encoder q(z\|x) tries to match. However, in practice, the actual distribution of codes according to the encoder (taken over all datapoints) typically doesn't actually resemble the prior distribution. This becomes problematic when trying to sample new data from the VAE, as there are regions of the latent space for which you are either likely to sample codes from p(z) but which the decoder hasn't seen during training, or regions of the latent space where a sizeable part of the data distribution is encoded to, but which isn't reached by sampling from p(z). 


![encoder distribution](https://keras.io/img/examples/generative/vae/vae_16_0.png)

Figure 1: Latent codes for a VAE trained on MNIST. Source: Keras tutorial https://keras.io/examples/generative/vae/

One way to overcome this is by learning a parameterized p(z). There are various ways of parametrizing p(z), but the one we're interested in is by using an 'energy function', in this case simply a neural network.

![energy function](../../images/posts/energy-landscape.png)

Figure 2: an example of an energy function in 2-d. 

When an energy function is learned on the latent space, its local minima correspond to clusters of latent codes and can be interpreted as learned classes. Paths through the latent space with minimal energy can be regarded as natural interpolations between data points.

In the case of a two-dimensional latent space, the energy function can be plotted and visually inspected in order to find minima and see natural interpolations. This is however not possible when the latent space is higher-dimensional. This begs the question: how can we inspect and interpret the learned energy function in higher dimensions?

The following are some questions that can be investigated as a master project:

-	What's the best way to learn an energy-based model as a prior in a VAE?
-	How to inspect and interpret the learned energy function in higher dimensions?
-	How can we combine other methods for interpretability in VAEs with this EBM prior?
-	How can we incorporate domain knowledge into the EBM prior?


Supervisor: Vlado Menkovski, Simon Koop 

