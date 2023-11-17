---
tags:
  - machine-learning
---

## Overfitting

Overgeneralizing a population or Overfitting.

E.g. You met a bad driver in a foreign country and you said everyone in that country drive poorly

### When does it happen

When the model is too complex relative to the amount and [[Bad Data#Poor quality Data|noiseness]] of the training data

### Possible solutions
- Simplify the model by selecting one with fewer parameters, by reducing the number of [[Training set#Predictors|attributes]] in the [[Training set|training data]], or by constraining the [[The machine learning landscape#Types of Machine Learning Systems|model]].
- Gather more [[Training set|training data]]
- Reduce the [[Bad Data#Poor quality Data|noise]] in the [[Training set|training data]].

### Also see: 
- [[Regularization]]

## Underfitting

Opposite of overfitting, the model cannot capture the underlying structure of the data

### When does it happen

When the model is too simple to learn the underlying structure of the data

### Possible Solutions
- Select a more powerful model, with more parameters
- Feed better features to the learning algorithm ([[Feature engineering]])
- Reduce the constraints on the model (e.g., reduce the [[Regularization]] hyperparameter)
