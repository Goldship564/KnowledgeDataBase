---
tags:
  - data-science
  - data-analytics
  - power-bi
---
## Performance analyzer
Badly optimized [[Data Analysis eXpressions (DAX)|DAX]] can take a long time to query and returns its results from its Dataset. A visual that contains too much info can take a long time to render.

To detect performance issues, you can go to optimize tab can turn on performance analyzer. This will start a counter and record the time to perform different actions. You can then review all the action time and see what is taking more time and try to optimize it.

## Power Query Diagnostics
You can use Power Query Diagnositics in the [[Power Query]] editor to diagnostics the performance

## [[Power  BI]] project
Check section [[Power  BI#File format]] 

## Tabular Model Definition Language (TMDL)
Due to TMSL is hard to read and no resemble the [[Power  BI]] language, a group of [[Power  BI]] users have develop a new language that convert [[Power  BI]] tabular models' metadata into a more readable format.

This new language have gain huge popularity and would be supported by Microsoft in the future. However currently there is no native way extract it. You will need to use Tabular Editor to extract it.

One of the biggest difference between TMDL and BIM is the text that is stored does not contain special characters that the system use to identify newline and others.

TMSL is similar to JSON wihile TMDL is similar to YAML