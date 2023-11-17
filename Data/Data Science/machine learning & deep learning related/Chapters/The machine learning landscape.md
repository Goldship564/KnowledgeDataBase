---
tags:
  - machine-learning
  - computer-science
---

Machine learning (ML) is not a *futuristic fantasy*. It was already here (e.g. [Optical Character Recognition](https://en.wikipedia.org/wiki/Optical_character_recognition))

First <abbr title = 'Machine learning'>ML</abbr> application is spam filter at the 1990. 

## What is machine learning

The science (and art) of programming computers so they can learn from data

> [Machine learning is the] field of study that gives computers the ability to learn without being explicitly programmed

\- Arthur Samuel, 1959

> A computer program is said to learn from experience E with respect to some task T and some performance measure P, if its performance on T, as measured by P, improves with experience E

\- Tom Mitchell, 1997

e.g. Spam filter

It is a machine learning program, given examples of spam emails (flagged by users) and examples of regulars (nonspam), emails. The program can learn to flag spams

The example that the system uses to learn is called [[Training set]]. Each training examples is a training instance (or [[Training set#Sample|Sample]] ) 

Spam filter define by Tom analogy:
- T: Flag spam for new emails
- E: The Training Data
- P: e.g. The ratio of correctly classified emails (Also called [[Accuracy]])

## Why use Machine learning

- Problems for which existing solutions require a lot of fine-tuning or long lists of rules: one Machine algorithm can often simplify code and perform better than the traditional approach
- Complex problems for which a traditional approach yield no good solution: the best machine learning techniques can perhaps find a solution
- Fluctuating environment: A Machine learning can adapt to new data
- Getting insights about complex problems and large amount of data

## Example of Machine learning

[Wikipedia Machine learning application](https://en.wikipedia.org/wiki/Machine_learning#Applications)

## Types of Machine Learning Systems

- [[Supervised learning]]
- [[Unsupervised learning]]
- [[Semisupervised learning]]
- [[Reinforcement learning]]

## Batch and Online Learning

Whether the system can learn incrementally from a stream of incoming data

- [[Batch learning]]
- [[Online learning]] 

## Instance-Based versus Model-Based Learning

Categorize the system by how they *generalize*. A machine learning system that have good performance measure on training data is good but if its not performing well on new instance its not a good system.

Two ways to generalization
- [[Instance-based learning]]
- [[Model-based learning]]

## Main challenges of machine learning

"Bad algorithm" and "Bad data" are the two things that can go wrong. 

### Examples of Bad data
- [[Bad Data#Insufficient Quantity of Training Data|Insufficient Quantity of Training Data]]
- [[Bad Data#Nonrepresentative Training Data|Nonrepresentative Training Data]]
- [[Bad Data#Poor quality Data|Poor quality Data]]
- [[Bad Data#Irrelevant features|Irrelevant features]] 

### Examples of Bad algorithms
- [[Bad Algorithms#Overfitting|Overfitting the training Data]]
- [[Bad Algorithms#Underfitting|Underfitting the Training Data]]


## Testing and Validating 

You can test it out on the field and gathered feedback (This might lead to bad customer satisfaction) or split your data set into [[Training set]] and the [[Test set]], and you test it against the [[Test set]]. The error rate on new cases is called the [[Generalization error]].

### Hyperparameter Tuning and Model Selection

One option to decide between models is to train both model (obviously) and see how they generalize using the test set.

Suppose you found a model that [[The machine learning landscape#Instance-Based versus Model-Based Learning|generalize]] better, but you want to apply some [[Regularization|regularization]] to avoid [[Bad Algorithms#Overfitting|overfitting]]. You decide to train 100 different models using 100 different values for the regularization [[hyperparameter]]. When you launch the model to production, it does not perform as well as expected. 

The above scenario happens cause cuase you measured the generalization error multiple times on the test set and you adapt the model and hyperparameters to produce the best model for that particular set.

#### How to solve it?

Use [[Holdout validation]]

### Data mismatch

Sometimes the data you gathered won't be perfectly representative of the data that will be used in production.

In such case, most important rule is to remember the [[Validation set]] and the [[Test set]] must be as representative as possible of the data you expect to use in production. 


