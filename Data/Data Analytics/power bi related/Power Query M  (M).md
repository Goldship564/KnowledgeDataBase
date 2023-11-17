---
tags:
  - power-bi
  - data-analytics
  - business-intelligence
aliases:
  - M
  - Power Query M
---
## Overview
A language used by Power Query to extract, transform and load data from your [[Data source]] into your [[Report]]'s [[Dataset]].

> [!example]
> <pre>Table.AddColumn(#"Changed Type"), "First Characters", each Text.Start([name],1), type text)</pre>
>
> What this formula do is it add a new column to the table, named that column first characters, and ran a quick operations to extract the first character of each state's name from our state name column. Finally it set the column be using the text data type


Most Power Query M queries operate in linear fashion where you are building a sequence of steps. However not all queries are linear. You can build queries that use [[branching]] and [[nest|nested]] logic.





