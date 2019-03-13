---
layout: post
title:  Neural Networks from Scratch
date:   2018-06-09 20:20:29 -0400
permalink: /wip2/
tags: nn numpy mlp 
tags_visible: true
excerpt: "Some nice introduction to the article"
has_paper: false
comments: true
paper: https://github.com/
github: https://github.com/
---

In this post, I describe the implementation of a basic neural network from 
scratch. 

I provide you with a very minimalistic Python code that will allow 
you to see the essentials of deep learning in action beyond the theory.

_**Disclaimer**: this post assumes you're already familiar with the theory 
behind neural networks and that you want to put into action what you have
learned from books, video, papers, etc._

Here's the outline for this post:
1. Our neural net
2. Our building blocks
3. Feed forward
4. Loss
5. Backpropagation
6. Training and testing on a dataset
7. Conclusions

The code is available [here](https://github.com/tavo91/dl_from_scratch/)

## 1. Our neural net

![Basic NN](/assets/images/basic-nn-1.png)

We are going to implement a minimalistic network with single hidden layer as in the 
picture above. The input layer only contains two neurons (i.e., two features),
and the output layer holds a single neuron (i.e., for binary predictions). Also, we 
are going to used a `ReLU` activation function for the hidden layer and a
sigmoid function for the output layer.

### 2. Our building blocks

As you may be familiar already, recall that 
* **Neurons** receive an input based on the output of previous neurons. Then, they
process their input by applying an activation function to it. The result is what neurons
provide as output.

* **Connections** between layers are represented by matrices. For example, the connections
between the input and the hidden layers, we have a matrix of shape 2x3. Similarly,
the connections between the hidden and output layers are represented by a matrix
of shape 3x1

* **Activation functions** are nonlinear functions that allow our networks handle very complex
decision boundaries. In this post, we only use ReLU and sigmoid.

### 3. 
   