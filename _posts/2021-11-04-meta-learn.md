---
layout: post
title: Aspect-based Few-shot classification (Meta-learning) 
excerpt: ""
modified: 04/11/2021, 10:35:24
tags: [few-shot classification, meta learning, deep learning, psychometric learning]
comments: false
category: mscproject
---

Meta-learning (also referred to as learning to learn) is a set of Machine Learning techniques that aim to learn quickly from a few given examples in changing environments [1]. One instantiation of the meta-learning is the task of Few-shot classification.

In this task the problem is formulated as assigning a class value to a query image, where classes are specified by one (or few) examples in a support (data) set (Figure 1). Here both the query image and the example images for each class in the support set have never been seen by the model during training. Moreover the content of the images in the query and support set may be new to the model.

![One-shot 4-class image classification](../../images/posts/one-shot-4-class.png)
Figure 1. One-shot 4-class image classification


The underlying assumption is, however, that all data points (from the support sets and query) have a single and uniquely identifying class association. In a more general setting, we could consider that the support sets define classes that are a subset of classes in other support sets. Furthermore, we could consider examples where support sets define classes that are focused on one of many aspects of the data. Specifically, looking at a set of images of animals. One can consider the aspects of the species (dogs, cats, cod). The family (mammals, fish) is at a higher level in a hierarchy. But also different aspects such as the gender of the animals or how fast they can travel, their living environment (water, on land), and many others. 

In the one-shot (few-shot) learning context, this aspect is defined by the support set. If all images in the support set are of lions. The class definition cannot be about the species of the animal as this does not change in any of the examples. For example consider Figure 2, 3 and 4. In each of these figures classification based on the species is not possible. Any meta-learning model that is capable of dealing with classification of the animals in the images based on the species (even for unseen species during training) may not be able to identify the right class assignment as all support set images are of lions. However, in the given support set, different aspects do vary. For example whether the animal is running, sitting, roaring, or being a toy rather than alive. Based on these different aspects one could actually determine the class association. 

![One-shot 4-class image classification](../../images/posts/aspect-query1.png)
Figure 2. Roaring aspect based query  

![One-shot 4-class image classification](../../images/posts/aspect-query2.png)
Figure 3. Sitting aspect based query

![One-shot 4-class image classification](../../images/posts/aspect-query3.png)
Figure 4. Running aspect based query

Humans are very capable of inferring the aspect of the question in this setting. However, meta-learning algorithms are not specifically designed for this given the assumption of a single discriminating class description. 

The goal of this project is to extend the capabilities of meta-learning models towards aspects-based meta-learning. One of the possible reasons for lack of a solution for this problem formulation may be the incompatibility of the traditional label-based supervision learning approaches for dealing with the variable aspects of high-dimensional data. However, much progress has been made in learning from other types of supervision such as psychometric testing [2]. Enabled with such techniques, the goal of the project is to develop a method that can address the challenge of Aspect-based meta-learning. 


Supervisor: Vlado Menkovski

[1] [https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html](https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html)

[2] Yin, L., Menkovski, V., & Pechenizkiy, M. (2020). Knowledge Elicitation using Deep Metric Learning and Psychometric Testing. arXiv preprint arXiv:2004.06353. [arxiv link](https://arxiv.org/abs/2004.06353)
 


