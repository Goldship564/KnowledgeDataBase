---
aliases:
  - RMSE
tags:
  - statistics
  - machine-learning
---
## Equation for Root Mean Sauare Error

$$ RMSE(X,h) = \sqrt{\frac1m \sum_{i=1}^m(h(x^{(i)})-y^{(i)}})^2 $$

## Uses in Machine Learning

It gives an idea how much error the system typically makes in its predictions, with higher weight for learge errors

## Notations

This equations introduces several very common Machine Learning notations that we will use. 

| Variable | Description | Example |
| -- | --| -- |
|m|number of instances in the dataset you are measuring the RMSE on|If you are evaluating the RMSE on a [[Validation set]] of 2000 districts, then $$m=2,000$$ |
| $$x^{i}$$|A vector of all the feature values (excluding the label) of the $$i^{th}$$ instance in the dataset, and $$y^{(i)}$$ is its label|If the first district in the dataset is located at longitude -118.29, latitude 33.91, and has 1,416 habitants with a median income 38372, and the median house values is 156,400 then $$x^{(1)}=\begin{pmatrix}-118.29\\33.91\\1,416\\38,372\end{pmatrix}$$ and: $$y^{1}=156,400$$|
|X|a matrix containing all the feature values (excluding labels) of all instances in the dataset. There is one row per instances, and the $$i^{th}$$ row is equal to the transpose of $$x^{(i)}$$, note $$(x^{(i)})^T$$|$$X=\begin{pmatrix}(x^{(1)})^T\\(x^{(2)})^T\\\vdots\\(x^{(2000)})^T\end{pmatrix}=\begin{pmatrix}-118.29&33.91&1416&38372\\\vdots&\vdots&\vdots&\vdots\end{pmatrix}$$|
|h| system's prediction function, also called an [[hypothesis]], When your system is given an instance's feature vector $$x^{(i)}$$, it outputs a predicted value $$\hat{y}^{i}=h(x^{(i)})$$ for that instance | If your system predicts that the median housing price in the first district is \$158,400, then  $$\hat{y}^1=h(x^{1})=158,400$$. The prediction error for this district is $$\hat{y}^{(1)}-y^{(1)}=2000$$
|$$RMSE(X,h)$$|The cost function measured on the set of examplese using your [[hypothesis]] h | |








