# GAN-Project


Introduction

Generative adversarial model is an ingeniously designed unsupervised learning algorithm. It can be used to generate realistic images of high accuracy. The key ideas are to build two competing neural networks and have them take part in a zero-sum game using mini-max.

Background 

Generative adversarial network model was originally published by Goodfellow et al in 2014. It has since become well know for its ability to generate realistic looking images.

One of the biggest challenges people face when training GANs is balancing the generator and discriminator so that one can’t dominate another. This has limited GANs to getting compelling results only when training models using images from narrow domains, examples include Yu et al 2015 on bedroom scenes and Lie et al 2015 on human faces. Recently David Ward-Farley and Yoshua Bengio (2017) attempted image synthesis from datasets comprising a diverse set of categories, using a denoising auto-encoder to purpose high-level targets for the generator.

The GAN Framework 

As the name suggests, GAN framework involves two adversaries, one is the generator, which learns from the training data and creates new instances of objects similar to those in the training data. The other is the discriminator, which given a set of labeled data, trains a classifier to determine whether or not a sample comes from the original dataset. As Goodfellow mentioned in his tutorial, this is like a game between a police and a counterfeiter, where the counterfeiter tries to product counterfeits that are made by the original manufacturer(in our case, probability distributions), while the police tries to spot those counterfeits.

Why use generative modeling? 

Several good applications for the usage of generative modeling were outlined in Goodfellow’s original guide. These include:

Generative models can be used to test our ability to manipulate and represent high dimensional probability distributions, which are important in many areas of applied maths and engineering.
Can be used in reinforcement learning.
Upping the resolution of an image [1].
Creating new artwork computationally.
Image-to-Image transition, such as sketch to photo, aerial photos to maps.

Additionally, GAN has been used to model rudimentary patterns of motion in video by Facebook[2].
