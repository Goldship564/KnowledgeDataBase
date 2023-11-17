---
tags:
  - power-bi
  - data-analytics
  - business-intelligence
aliases:
  - DAX
---
## Overview
Data Analysis eXpressions (DAX) serves multiple purpose in [[Power  BI|power BI]]. It's the query language that is used by the report to retrieve the data it needs from the [[Dataset]]. (A communicate tools between the [[Report]] and the [[Dataset]])

For instance, if you build a line chart in your report, [[Power  BI|power BI]] will dynamically generate a [[Data Analysis eXpressions (DAX)|DAX]] query based on the data you put in that chart and will then send that [[Data Analysis eXpressions (DAX)|DAX]] query down to the dataset to calculate and then retrieve the data it needs, and then it will render the results in your chart. 

A great thing about [[Data Analysis eXpressions (DAX)|DAX]] is its ability to take advantage of table [[Cardinality|relationships]].

## Basic measures in DAX
[[Measures]] are one of the most important concepts in [[Power  BI|power BI]] development. Written using the DAX formula language, they are an integral part of every data model that attempts to aggregate data for reporting purposes.

They exist independently of the tables in your data model. 

### Dax Formula 
> [!example] <pre> Measure = Formula</pre>
Anything on the left side in the name and anything on the right side is the formula. 

For more info: Check [[Measures]]


## Creating Calculated Columns with [[Data Analysis eXpressions (DAX)|DAX]]
[[Calculated Columns]] are created in your data model through writing [[Data Analysis eXpressions (DAX)|DAX]] formulas and add them to your table.

For more info, Check [[Calculated Columns]]

## Using Variables in [[Data Analysis eXpressions (DAX)|DAX]]
You can perform multiple calculations inside a single measure and combine them together and return the results.

To start a calculation you will need to assign variables (keyword var), and tell the system what to return (keyword return)

### Benefits
- It breaks down the [[Data Analysis eXpressions (DAX)|DAX]] formula into component and make it easier to understand what is happening
- it makes it easier to troubleshoot and debug your [[Data Analysis eXpressions (DAX)|DAX]] formula
- It can bring some performance of your measures

## Using Comments to Explain [[Data Analysis eXpressions (DAX)|DAX]] Formulas
Adding comments allow us to explain what the code is doing in plain language and document history and aid in troubleshooting

There are two way of commenting in DAX
- In line comments 
- Block comments

### Inline comments
create be created by using two // or two --

### Block comments
created by /* and end with \*/
