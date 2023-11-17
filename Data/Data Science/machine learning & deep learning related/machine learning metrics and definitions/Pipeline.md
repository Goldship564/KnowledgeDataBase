---
tags:
  - machine-learning
---

A sequence of data processing components is called a data pipeline. 

Pipelines are very common in a [[The machine learning landscape#What is machine learning|Machine learning]] syste, since there is a lot of data to manipulate and many [[Data transformation|data transformations]] to apply.

Component typically run [[Asynchrony|asynchronously]]. Each component pull in a large amount of data, process it, and splits out the result in another data store. Then, some other process do the same.  

## Benefit

This make the system simple to gasp and different teams can focus on different components.

## Drawback

IF a component go broken, it can go unnoticed for some time if proper monitoring is not implemented.