---
tags:
  - machine-learning
---

## Overview

Constraining a model to make it simpler and reduce the risk of overfitting

The amount of regularization to apply during learning can be controlled by a [[hyperparameter]].

>[!Note] 
>Do not set the value too large as it will result a flat model (a slope close to zero), Tuning hyperparameter is an important part of building a Machine learning system

## Example

Assume you have a linear model with $$ \theta_0\ \&\ \theta_1$$
The above model will provide the learning algorithm with two degree of freedom to adapt the model to the training data. if we force $$\theta_0 = 0$$ the algorithm would have only one degree of freedom and would have a much harder time fitting the data properly. Since the algorithm can only move the line up and down.

By doing operations like this, we manipulate the algorithm to create a model that is simplier than the 2 degree of freedom but more complex then the above example. 

You would want to find the right balance between fitting the training data perfectly and keeping the model simple enough to ensure it will generalize well.
