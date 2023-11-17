---
tags:
  - data-science
  - data-analytics
  - machine-learning
  - statistics
aliases:
  - data model
  - tabular model
---
## Overview
A prepared subset of data from your data source that is designed to meet a specific business purpose. 

Data is extracted from the [[Data source]] and loaded into dataset, so it can be used for analysis. This process is known as [[Extract, Transform, and Load (ETL)]]. 


## BI uses
Datasets must consist of at least one table of data but can consist of dozen if not hundreds of tables. 

Primary goal with the dataset is to build a logical set of tables that are loaded with data and they feed that data into the [[Report]] so that it can be visualize and analyzed. 

### Data models
Sometime data model is use interchangeable with dataset. Data model likely being the structure for the dataset. It is all of the rules, the relationships and the calcualtions that define how the dataset behaves

Underneath the surface, A power BI data model is a little more than metadata stored as text, and tables that are defined in that metadata form the structure of your model.

Until data is actually loaded into your data model, it is a little more than just a bunch of metadata stored as text

Other things that define in a data model:
- [[Measures]]

Once the data model has been populated with data and begins running in the background of Power BI. Its now an active process on your computer that is consuming memory. It is now a type of [[Database]] known as a [[Database#Tabular model|Tabular model]]. (Data been directly copy from source and place in memory)

## Machine learning uses
- [[Validation set]]
- [[Training set]]
- [[Test set]]
- [[class-imbalanced data set]] 