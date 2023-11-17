---
aliases:
  - development set
  - dev set
tags:
  - machine-learning
---
A validation data set is a data-set of examples used to tune the [[hyperparameter]] (i.e. the architecture) of a classifier. It is sometimes also called the development set or the "dev set".[13] An example of a [[hyperparameter ]]for artificial neural networks includes the number of hidden units in each layer. It, as well as the [[Test set|testing set]] (as mentioned below), should follow the same probability distribution as the [[Training set|training data]] set.

In order to avoid [[Bad Algorithms#Overfitting|overfitting]], when any classification parameter needs to be adjusted, it is necessary to have a validation data set in addition to the [[Training]] and [[Test set|test]] datasets. For example, if the most suitable classifier for the problem is sought, the [[Training set|training data]] set is used to [[Training|train]] the different candidate classifiers, the validation data set is used to compare their performances and decide which one to take and, finally, the [[Test set|Test data]] set is used to obtain the performance characteristics such as [[Accuracy]], sensitivity, specificity, F-measure, and so on. The validation data set functions as a hybrid: it is [[Training set|training data]] used for testing, but neither as part of the low-level training nor as part of the final testing. 
## See also:
[Wikipedia Validation Set](https://en.wikipedia.org/wiki/Training,_validation,_and_test_data_sets#Validation_data_set)