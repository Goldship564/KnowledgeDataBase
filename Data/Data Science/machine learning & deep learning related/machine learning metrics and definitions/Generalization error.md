---
aliases:
  - out-of-sample error
tags:
  - machine-learning
  - statistics
---
For [[Supervised learning]] applications in [[The machine learning landscape#What is machine learning|machine learning]] and statistical learning theory, generalization error[1] (also known as the out-of-sample error[2] or the risk) is a measure of how accurately an algorithm is able to predict outcome values for previously unseen data. Because learning algorithms are evaluated on finite samples, the evaluation of a learning algorithm may be sensitive to [[sampling error]]. As a result, measurements of prediction error on the current data may not provide much information about predictive ability on new data. Generalization error can be minimized by avoiding [[Bad Algorithms#Overfitting|overfitting]] in the learning algorithm. The performance of a machine learning algorithm is visualized by plots that show values of estimates of the generalization error through the learning process, which are called learning curves. 

Simple terms: This value tell you how well your model will perform on instances it has never seen before

If the training error is low but the generalization error is high, it means that your model is overfitting the training data.
## See also
[Wikipedia](https://en.wikipedia.org/wiki/Generalization_error)