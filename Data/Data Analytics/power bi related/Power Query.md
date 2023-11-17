---
tags:
  - power-bi
  - business-intelligence
  - data-analytics
aliases:
  - Power Query
---
An application come bundle with Power Bi and is use to connect the data source is prepared the data before loading into Power BI desktop

## Language behind Power Query
[[Power Query M  (M)]]

## Power Query editior
Things to keep note of.

- Close and apply button: Use to close the file and apply the changes you do
- query and left hand panel is what you are doing with the data, Applied steps is how you do it (the timeline)
- You can edit your applied steps by rightclicking it and edit steps

> [!Note] Nothing you do in the power query is capable of overwriting the data in the [[Data source]]
> Power query works by copying the data from the [[Data source]] into the Power Query mash up engine, running everything through your data recipe and then loading the results into the power query data model. Throught out the process, the [[Data source]] will remain **intact** 


### Formula bar 
- It displays the [[Power Query M  (M)|Power Query M]] formula that is generate by the transformation here in the Power Query editor.
### Tabs
- Home
	- Add new data source to the query, and do basic manipulation just as adding and removing rows and merging queries together
- Transform
	- Tools to help transforming existing column of data such as changing data type, renaming and splitting 
- Add 
	- Allow you to do similar stuff with Transform tab, but instead of overwriting, these will add new columns to [[Power  BI#Power BI]] with the results 
- Views
	- Allow you to view the underlying code for your queries and looking at the dependencies between various queries


## Basic of [[Power Query M  (M)|Power Query M]]
Check section [[Power Query M  (M)|Power Query M]]

## Data preview
A list of function power bi provides to let you preview the data
### Column Profiling
Useful for examining data for errors and inconsistency. Can help to identify data issue you will need to fix.

#### Column Statistics
Gives us a summary of the data in the column. Such as how many values and how many distinct values
>[!faq]- Did you know the difference between unique and distinct?
>	[[Distinct values]] is a count of each value that appears at least once in the column
>	[[Unique values]] is a count of each value that appear only once
>Looking at Distinct and Unique values can help you find outliers of the data.


#### Value distribution
Gives us a summary of the frequency of the each value in the column. If you observe the frequency, you can also discover special relationship such as [[tree|parents-child relationship]] between columns.

### Column distribution
A similar views to value distribution but show on each header of the column and give you less info. Great for overview of the data.

### Column quality
Show you how much of each column that is valid data, empty or not valid.

## Data type in Power Query
When Power Query first loads data from your data source, it will scan each column and attempt to automatically assign a data type. 

The data type of each column in the Power Query editor can be determined by looking at the icon to the left of the column name of each column

> [!note] Numeric Columns can only contain numbers where text columns can contain both letter and numbers

Data type determine what kind of operations you can perform on the column. For instance, mathematical operations can be perform on numeric column but not text. We can also combine different text columns together but not dates.

### Dafault data type
Denotes as "ABC123". This is also known as untyped or unclassified data type. Sometime [[Power  BI|power BI]] would want you to explicit tell them the data type of a column. It would be wise to check if you have the correct data type before going futher on transforming those data.

> [!faq]- How [[Power  BI|power BI]] or excel store dates?
> Dates inside tools like [[Power  BI|power BI]] or excel stored dates as serial numbers, where each day on the calendar day is represented by a whole number and everything smaller then eight days span of time is represented by a portion of that whole number, which is shown after the decimals
> This make it easiers for tools like [[Power  BI|power BI]] or excel to calculate differences between various dates and times.

### Invalid datatype
If you try to convert a column to a incompatible data type. The values in the column will show as Error. To check the error message. you can click on one of the error cells and display the error message. 

## Choosing columns
> [!tip] [[Key principles to good dataset design]]
> Avoid loading your data model with more data than you need

To choose columns. Go to Home tab and find the manage column section or you can go to the small button where the index and header collide (upper right hand corner)



## Working with [[Comma Separated Value]]
- Select the right delimiter
- The delimiter outside the quotation mark "" is used to separate the columns

> [!note] Don't use the load button, use transform instead

