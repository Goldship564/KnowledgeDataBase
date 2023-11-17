---
tags:
  - data-analytics
  - power-bi
  - data-science
---
## Getting Data from Web APIs
When developing in [[Power  BI|power BI]], it is not uncommon to work with [[Application Programming Interface|API]] 

To get data from the web API for [[Power  BI|power BI]], just select the web options under "get data". 

## Preparing the Economic Indicators Data with [[Power Query]]
If some data is mssing from a record. It might cause data conversion be not successful. To prevent such scenario happen. You can either filter the data out or remove them.


## Referencing and Duplicating Queries

> [!note] it is helpful to think of queries in [[Power Query]] as a linear sequence of processes. 
> Power Query will perform whatever transformations you tell it to against the original query first. Then it will take the output created by the original query and use that as the source of the new query

### Referencing Queries
It create a second query and references the output of the first query
#### When useful
Useful when you need the output only

### Duplicating Queries
Recreate the first query step by step 
#### When useful
Useful when you want to do some quick changing to the query to create a different query

> [!tip] Also check [[Upstream and Downstream Queries in Power BI]]


## Merging Queries
Linking two tables using one or more columns that they have in common, thus combining them.

The ability to combine data from multiple table using the merge queries features in [[Power Query]] is a foundational skill for [[Power  BI]] developers to learn. This is especally true when you are potentially working with data from multiple sources

### Guideline on merging queries
1. Start from the main query when you're about to merge queries together
2. Then expand the merge queries at the home page and press merge queries as new.
> [!tip] Benefit using merge queries as new will make the merge process a lot less confusing when working with many tables. It also works better for diagramming the flow of the queries
3. . Select the rows you want to match and select a way to join

## Join Kinds in [[Power Query]]
Below are the join type in power bi
- [[Left Outer Join]] (default type) 
- [[Right Outer Join]] 
- [[Full Outer Join]]
- [[Inner join]]
- [[Left Anti Join]]
- [[Right Anti Join]]

## Query Dependencies and Lineage

### Queries dependencies
Use to visualize where the data is coming from