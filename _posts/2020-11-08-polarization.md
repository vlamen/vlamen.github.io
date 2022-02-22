---
layout: post
title: ML for Scanning Electron Microscopy with Polarization Analysis 
excerpt: "The goal of this project is developing machine learning models that can support the analysis of Scanning Electron Microscopy with Polarization Analysis (SEMPA) images."
modified: 11/05/2020, 10:35:24
tags: [generative models, electron microscopy, phyiscs]
comments: false
category: mscfinished
---

The development of next generation of magnetic data storage devices requires beter understanding of physical effects at nanoscale structures of certain materials [1, 2]. The goal of this project is developing machine learning models that can support the analysis of Scanning Electron Microscopy with Polarization Analysis (SEMPA) images.  

In conventional magnets (such as fridge magnets) there is one magnetic north pole and one south pole. The magnetization vector (which points towards the local north pole) inside the material therefore points in the same direction everywhere. However, in the systems that we study, the magnetization is not unidirectional, but can instead form complex 3 dimensional patterns and structures where the magnetization vector rotates on nanometer length scales. The exact size and shape of these structures is intricately connected to the physical effects that play a role at the nanoscale.  By imaging and studying such structures we gain information about the nature of these effects. 

We investigate such patterns using Scanning Electron Microscopy with Polarization Analysis. This technique enables measurements of the 3D magnetization vector inside a magnetic sample with nanometer resolution. The generated data consists of 2D images containing projections of this 3D vector field, that are mutually orthogonal. An example is shown in Figure 1. Currently, these data sets are analyzed manually which is a time consuming process that is prone to errors. 

The goal of the proejct is to develop a machine learning model to detect and identify physically relevant features in these data sets. Moreover, we are particularly interested in developing adeep generative model that incorporates the experimental parameters of the measurements in its latent structure. Such models can provide more insight into the fundamental physics underlying these processes.
 
![SEMPA](../../images/posts/nano-mat.png)

Figure 1: a) Vector map of a magnetization texture where rotation occurs along thin structures called domain walls, from [3]. b-c) SEMPA images of such a pattern in a real magnet. The pixel value corresponds to the projection of the magnetization texture onto the y-axis (b) and x-axis (c). In white pixels the magnetization points either upwards (b) or to the right (c) and in dark purple pixels it points down (b) or towards the left (c). d) Reconstruction of the magnetization texture made using the data in b) and c). In the white and black regions the magnetization points out of and into the screen and in the colored regions its direction is given by the color wheel. 


Supervisor: Vlado Menkovski, Reinoud Lavrijsen, Marielle Meijer, Mark de Jong


[1] Lucassen, J. et al., Tuning magnetic chirality by dipolar interactions, PRL, 123, 157201, (2019)

[2] Meijer, M.J. et al., Magnetic chirality controlled by the interlayer exchange interaction, 124, 207203, (2020)

[3] Chen, G. et al., Tailoring the chirality of magnetic domain walls by interface engineering, Nat. Commun., 4:2671 (2013)


