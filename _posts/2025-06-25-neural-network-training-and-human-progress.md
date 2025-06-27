---
layout: post
title: "Neural Network Training and Life Progress: Gradient Descent as a Life Framework"
date: 2025-06-25 06:30:00
description: I identify the parallelism between how neural networks learn and how individuals make progress in their lives.
tags: AI, Entrepreneurship
---
<div align="center" style="font-weight: bold">Introduction</div>
Throughout the final year of my undergraduate degree at Princeton, I spent a lot of time thinking about how I could best approach the achievement of my goals and the realization of the evolving vision I devised for my life. I also spent a lot of time studying and training neural networks for my thesis. These threads of attention and cognitive effort largely felt orthogonal to one another: the former was strictly a personal and humanistic matter and the latter an impersonal and technical one. I compartmentalized the topics accordingly and never deliberately tried to connect them.

Gradually and organically, however, I began to appreciate -- or manufacture -- their parallelism. The problem of transiting from my current state in life to my desired state in life, I realized, may not be dissimilar from the problem of transiting from a randomly-initialized neural network to one that is maximally performant at a given predictive or generative task. I became interested in translating the intuition I developed around how neural networks iteratively acquire their impressive capabilities into a mental framework for understanding and advancing my own journey. 

In this blog post, I present the product of these translational reflections. I first introduce and briefly explain the essence of gradient descent -- the optimization algorithm through which neural networks learn. I then make the case that gradient descent is a powerful model for the process of making progress in one's life.  I hope the ideas I relay here are as useful to you as they have felt to me.

<div align="center" style="font-weight: bold">The Essence of Gradient Descent</div>
To explain the essence of gradient descent, I'll start by constructing a model that represents the process of neural network training as simple interactions between simple computational objects. 

Suppose there is a list of numerical inputs *[x]* and a list of numerical outputs *[y]*. Suppose further that a function *f(x)* maps each numerical input in *[x]* to a numerical output in *[y]*. The objective is to train a neural network to predict *y* based on *x*, which essentially requires that the neural network learn *f(x)*.

Accordingly, the neural network can be represented as *f'(x)* -- an approximation of *f(x)*. Upon initialization, *f'(x)* is a random function that likely does not resemble *f(x)* at all. The instrument that is employed to change this -- to minimize the difference between *f'(x)* and *f(x)* -- is the gradient descent algorithm. Here's how it works: 
1. Each element of *[x]* is passed through *f'(x)*, generating a prediction *y'*.
2. The error between the predicted output *y'* and the true output *y* is calculated, as defined by a loss function.
3. The derivative -- the "gradient" -- of the loss function with respect to the parameters that define *f'(x)* is calculated; this quantifies how directional alterations in *f'(x)* make *f'(x)* more similar or less similar to *f(x)*.
4. *f'(x)* is updated in the direction that reduces the value of the loss function and thus makes *f'(x)* more similar to *f(x)*. The magnitude of the update is governed by the value of the learning rate hyperparameter defined at the onset of training.

These steps are repeated over several iterations until convergence, at which point *f'(x)* should closely resemble *f(x)*.

This is gradient descent in the context of neural network training. Qualitatively, it is a procedure for minimizing the difference between the initial functionality of a neural network and the desired functionality of a neural network. I'll reinforce these concepts in the next section as I adapt them into a framework for life progress.

<div align="center" style="font-weight: bold">Gradient Descent as a Life Framework</div>
I'll make the case for gradient descent as a life framework by exchanging the mathematical objects on which the algorithm natively operates with the personal objects of progress; I'll use the model I constructed in the previous section to explain this.

Just as the objective of neural network training is to achieve a desired functionality within a neural network starting from a simple initialization, I posit that the objective of human progress is to reach a desired state in life from an initial state in life. 

Accomplishing this objective through one perfect, calculated action feels -- and arguably is -- infeasible, as is training an optimal neural network in one shot. Instead, a reasonable approach to progressing towards a desired state involves first taking an action; it involves first doing *something*, just as neural network training begins by randomly intializing the parameters of the network.

The next step is to assess how far you are from accomplishing your goal after taking that action -- to calculate the error between the result of your action and not your expected result but your North Star.

What follows is analogous to the process of calculating the derivative of the loss function and updating the parameters of the network. You should determine which direction for your next action feels most aligned with your desired state and decide how risky an action you wish to take. The magnitude of risk is captured in the learning rate hyperparameter in neural network training. 

The process of life progress, I believe, is thus no different than vanilla gradient descent.