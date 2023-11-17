---
tags:
  - power-bi
  - data-science
  - data-analytics
---
[[Calculated Columns]] are created in your data model through writing [[Data Analysis eXpressions (DAX)|DAX]] formulas which makes them seem like measures at first, but there are some crucial difference.

The difference: 
- Measures are dynamically calculated in your report and based on whatever context you add them to. Calculated columns are not, they are calculated only when you refresh your [[Dataset]] from the [[Data source]]
- Measures do not need to be bound to any particular table in your model. Calculated columns do. 
- Measures exist as a metadata while calculated columns stored data in the table (also known as [[Data persistence]]). This can cause calculated columns be faster but taking more space

### Steps to create
use the CALCULATE function. Below is an example of how it looks
> [!example] <pre>2015 Population =</br>CALCULATE(</br><ul style = 'list-style-type:none;'><li>SUM('states population'[state population]),</li><li>'states population'[Year] = 2015</li></ul>)</pre>
> 2015 Population is the calculated column name, as you can see the basic calculate function takes two argument. An action (the SUM) and an argument (state population = 2015)

