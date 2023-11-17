---
tags:
  - machine-learning
---

Hold out part of the [[Training set]] to evaluate several candidate models and select the best one. 

The held out set is called the [[Validation set]]. 

you train various model on the reduced [[Training set]], and you select the model that performs best on the [[Validation set]]. Lastly you evaluate the model on the [[Test set]] to get an estimate of the [[Generalization error]].

> [!note]
> If the [[Validation set]] is too smale, then model evaluation will be imprecise. You may end up selecting a suboptimal model by misteak
> 
> If the [[Validation set]] is too big, the remaining training set will be much smaller then the full training set. You can solve this by [[Cross validation]]

