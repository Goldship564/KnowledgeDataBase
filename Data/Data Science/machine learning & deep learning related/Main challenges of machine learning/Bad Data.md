---
tags:
  - machine-learning
---

## Insufficient Quantity of Training Data

It takes a lot of data for most Machine Learning algorithms to work properly. Without sufficient amount of data. The model will not output results that can be properly [[The machine learning landscape#Instance-Based versus Model-Based Learning|generalize]]

> Data matters more than algorithms for complex problems 
> \- Peter Norvig, ["The Unreasonable Effectiveness of Data," IEEE Intelligent Systems 24s, no. 2 (2009)](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/35179.pdf)

## Nonrepresentative Training Data

If your data is not representative of the cases you want to [[The machine learning landscape#Instance-Based versus Model-Based Learning|generalize]]. The model you trained will not likely to make accurate prediction of the population you want to predict.

See also: [Sampling Bias](https://en.wikipedia.org/wiki/Sampling_bias)

## Poor quality Data

If your data is full of errors, outliers, and noise (e.g. due to poor qulity measurements), it will make it harder for the system to detect the underlying pattern, so your system is less likely to perform well. 

It is often well worth the effort to spend time cleaning up your training data

### Examples when you will want to clean up your data
- If some instances are clear outliers, it might help to simply discard them or try to fix the error manually
- If some instances are missing a few features, you must decides whether you want to ignore these attributes, ignore these instances, fill in the missing values or train one model with it and one model without it

## Irrelevant features

*Garbage in, Garbage out*. Your system will only be capable of learning if the training data contains enough relevant features and not too many irrelevant features. A critical part of the success of a machine learning project is coming up with a good set of features to [[Training|train]] on. This process, called [[Feature engineering]].

