---
tags:
  - power-bi
  - data-analytics
---
By default all the visuals are linked to each other
## Creating and Formatting Visuals
To insert a visuals, you can use the visuals menu (in the home tab or in the insert tab) or you can right click anywhere in the report canvas. Some [[Power  BI]] have it on the side next as a collapsible tab like Data. For those you can drag and drop those visuals on the plane

### Adding data to the visuals 
You can use the on-object editor by clicking the add data button, which open up another menu to the side where you can see all of your tables and columns that are avaliable to added. Some [[Power  BI]] have it on the side and you can just drag and drop it to the respective fields.

### Resizing the visuals. 
You can drag and drop as well as resizing the visuals by holding or dragging the boundaries.

### Visuals Tab
Allow you to configure the how you want your visuals to look. They are different by which visuals you choose. 

### Properties
Allow you to configure other attributes of the table visual such as tool tips 

### Table visuals 
A simple and versatile tools.They are powerful since they can be interactively sorted. They can include images and icons where you can link users to external web.


## Visual interaction
By default, [[Power  BI]] visuals interact with each other. If you click on an item in one visual it will filter items in other visuals on the same page. 

### Edit interactions 
They control how a visuals react when user interact with other visuals. There are three major visual interactions.

### Highlighting
When user interact with another visual, the visual will highlight the user selection. 

### Filtering
When user interact with another visual, the visual will filter out the user selection

## None
The visual will not change when other visuals are interacted.

> [!note] Not all visuals have all the visual interaction 


## Introducing basic measure with [[Data Analysis eXpressions (DAX)|DAX]]
Please refer to [[Data Analysis eXpressions (DAX)|DAX]] section

## Adding Measures to our Report
The information that a [[Data Analysis eXpressions (DAX)|DAX]] measure returns is dependent on its visual context.

Using color as a visual cue is a vitial component of good report and dashboard design, regardless of which tool you're using

## Using Slicers and Hierarchies to Filter Data
### Slicers
Slicers are a little more than a filter control that sits on the report page. They come in different flavors and they're extremely useful for letting your rerport users slice and dice the data in various ways.

### Hierarchies
A hierarchy is a combination of two or more columns that have a relationship to each other, specifically a [[tree|parents-child relationship]], where one column is treated as a child or subordinate of the other column

Two basic way to create 
- putting two columns together
- putting two field to the slicer fields

### Explicit Hierarchy
They do the same thing as implicit hierarchy, however this give different analyst a shortcut they can use and tell them "The hierarchy is really important" and this is how we analyze our data

## Adding more data to [[Power Query]]

### Unpivot tables
Turning wide tables into skinny two colulmn tables. For more info: Check [[Key-Value pair]]. The way this work is by setting a pivot point, where in this case the year column, and then translating the other column in the table into the attribute value pair structure

Benefits:
- Decrease column number

Disadvantage:
- Make it harder for user to read

## Modeling Table Relationships
Table relationships are one of the most difficult part of building effective data model in Power BI. However, it is also one of the most important aspect of data modeling since it is common for people to report across multiple tables from multiple source.

The ability to create [[Cardinality|relationships]] in your data model allows you to bridge the gap, it also allow you to report on data that might have different [[Granularities|granularities]] 

When we first load new data into Power BI desktop, it automically scan the table and see if the new data have matching columns with the old data. Then it will attempt to create [[Cardinality|relationships]] between tables.

## Creating Calculated Columns with [[Data Analysis eXpressions (DAX)|DAX]]
Check section [[Data Analysis eXpressions (DAX)#Creating Calculated Columns with Data Analysis eXpressions (DAX) DAX]] 