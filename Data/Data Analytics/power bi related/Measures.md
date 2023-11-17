---
tags:
  - data-analytics
  - power-bi
  - business-intelligence
---
## Overview
Formulas that are stored in the data model that can dynamically recalculate as you interact with the report

When we define a measure in Power BI desktop, we're adding a text formula to our data model definiton.

When we define a measure in [[Power  BI]] desktop, what we are doing is adding a text formula to our [[Dataset|data model]] definition. 


> [!note] The best way to visualize this is to add a simple measures and see they are not added in the table. But you can add those in any visuals.

## Basic structure of Measures
> [!example] <pre>Measures = COUNT(States[State])</pre>
> <ul style = "list-style-type:none;"><li>The left hand side of the formula is the name of the measure</li><li>The right hand side is the calculation of the measures</li></ul>

## Explicit measures 
Explicitly defined using the [[Data Analysis eXpressions (DAX)|DAX]] formula language, can be easily identified by the calculator icon that sit next to each measure's name. 

It is considered best practice to use explicit measure whenever possible in [[Power  BI]], below are the reasons:
- By writing explicit measures. You force yourself to write [[Data Analysis eXpressions (DAX)|DAX]] and it helps user to learn [[Data Analysis eXpressions (DAX)|DAX]] quicker.
- Explicit measures are reusable in other explicit measures and save time
- Explicit measures are more flexible, Implicit measure are preset and might not be suitable for your case
- Explicit measure can use to create dynamic text labels that you can add to your reports, such as in your chart titles.
- Implicit measures cannot be used with the "Analyze in Excel" feature

> [!note] With all the difference, one thing explicit and implicit measures are similar are performance. They are doing similar calculation regardless which one you use.

## Implicit measures
Created by dragging columns onto visuals and then assign an aggregation to those columns. Any type of columns can be used to crate an implicit measure.

Using implicit measures for your visualization is discouraged by the vast, vast majority of [[Power  BI]] experts.

## Measure Tables
Empty table the only purpose to store measures. We create tables and attached them to the measure tables so all of our measures are grouped together in one place somewhere in our model.

Using Measures tables is a best practice that is generally agreed upon among most professional [[Power  BI]] professions.