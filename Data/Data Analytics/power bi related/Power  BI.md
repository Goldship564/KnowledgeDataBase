---
tags:
  - power-bi
  - data-analytics
  - business-intelligence
aliases:
  - introduction
  - power BI
---
## Power BI
Power BI ([[Business Intelligence]]), a software used by people and organization to analyze data for the purpose of deriving [[Domain driven data mining|actionable insights]]. Not everyone use Power BI to the same [[Business Intelligence|BI]] system ([[List of BI system]]]) due to different needs. 

### Goal of Power BI
Allow users to create reports and dashboard to generate [[Domain driven data mining|actionable insights]] so that people know what decision to make. (aka [[Data informed decision making|Data driven decision making]]])

### Development/ Developing 
Reference to building a [[Business intelligence solution]]

Development Generally consist of 75% data preparation and modelling, and only 25% of data visualization

## File format
### PBIX  file
In Power BI desktop, they can be saved as a P-B-I-X file or PBIX file. This stands for Power BI eXchange. Which is the most common file format used in Power BI. It compile everythign together into a single file.

#### Benefit:
- Make the power pi project nice and portable 

#### Drawback
- Size could be big if stored in disk and make it less portable
- Data security might be a concern
- Lack of version control

### PBIT file
Unlike PBIX file, PBIT file does not contain any data, they just have the data model definition and the report definition. 

#### Benefit
- This solved the data security problem with the PBIX files

### PBIP file (Power PI Project)
The application will break the project down into folders and logically organize all of your Power BI assets in one place and in a file format. It can also take your data and save it in a separate cache file and tell your version control system to ignore that file from the rest of your model

#### Benefit
- This makes tracking changes much easier
- Also solve the security issues with PBIX files



## What language Power BI uses 
please refer to [[Data Analysis eXpressions (DAX)]] 




## Power Query
A program that come bundle with Power BI. For details please check [[Power Query|Power Query]]
