---
layout: post
title: New patent CN115453880A
date: 2022-09-21 19:11:00-0400
inline: false
---


Training method of generative model for state prediction based on antagonistic neural network

---

The invention provides a training method of a generative model for state prediction based on an antagonistic neural network, wherein the antagonistic neural network comprises the generative model and an arbiter, the generative model and the arbiter both comprise multilayer fully-connected networks, and the method comprises the following steps: s1, sampling a plurality of control action sequences of predicted time domain length from all possible control actions under the constraint condition of a target system, sending each control action sequence into the real environment of the target system for execution to obtain a target state sequence of the target system corresponding to each control action sequence, and sending each control action sequence into a generation model to obtain a target system future state prediction sequence corresponding to each control action sequence; s2, forming a sample by using the current state of the target system, each control action sequence and the target state sequence of the corresponding target system after each control action sequence is executed, and generating a training set; and S3, training the generated countermeasure network for multiple times by adopting the training set until convergence.

[Google patents](https://patents.google.com/patent/CN115453880A/en)


