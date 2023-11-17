---
tags:
  - machine-learning
---

## Working with Real Data

When learning about [[The machine learning landscape#What is machine learning|Machine Learning]], it is best to experiment with real world data, not artificial datasets.

### Some places to look for data
- Popular open data repo
	- [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/)
	- [Kaggle datasets](https://www.kaggle.com/datasets)
	- [Amazon's AWS datasets](https://aws.amazon.com/opendata/)
- Meta portals
	- Data Portals
	- Open Data Monitor
	- Quandl
- Other pages listing many popular open data repo
	- [Wikipedia's list of Machine Learning Datasets](https://en.wikipedia.org/wiki/List_of_datasets_for_machine-learning_research)
	- [Quora.com](https://www.quora.com/)
	- [The datasets subreddit](https://www.reddit.com/r/datasets/)


## Look at the Big pictures

### First Step: Frame the problem

Ask your boss what is the business objective. Building the model is not the end goal. How does the company expect to use and benefit from this model? Knowing this is important, because it will determine how you frame the problem, which [[The machine learning landscape#Types of Machine Learning Systems|algorithms]] you will select, which [[The machine learning landscape#Example of Machine learning|performance measures]] you will use to evaluate the model, and how much effort you will spend tweaking it.

> [!Check also]
> [[Pipeline]]

Another question is ask your boss what the current solutions looks like. This gives you a reference for [[The machine learning landscape#Example of Machine learning|performance]], as well as insights on how to solve the problems.

### Second Step: Select a performance measure

one of the typical performance measure for regression problems is [[Root Mean Square Error]]. 

Another performance measure you can consider is [[Mean absolute error]].  (Good for outlier)

Both RMSE and the MAE are ways to measure the distance between two vectors: the vector of predictions and the vector of target values. Various distance measures, or norms are possible.