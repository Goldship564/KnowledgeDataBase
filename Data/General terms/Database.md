---
aliases:
  - database
tags:
  - computer-science
  - data-science
  - data-analytics
---
## Tabular model

Tabular models in Analysis Services are databases that run in-memory or in DirectQuery mode, connecting to data from back-end relational data sources. By using state-of-the-art compression algorithms and multi-threaded query processor, the Analysis Services VertiPaq analytics engine delivers fast access to tabular model objects and data by reporting client applications like Power BI and Excel.

### Direct Query
While in-memory models are the default, DirectQuery is an alternative query mode for models that are either too large to fit in memory, or when data volatility precludes a reasonable processing strategy. DirectQuery achieves parity with in-memory models through support for a wide array of data sources, ability to handle calculated tables and columns in a DirectQuery model, row level security via DAX expressions that reach the back-end database, and query optimizations that result in faster throughput.

### Creation
Tabular models are created in Microsoft Visual Studio with the Analysis Services projects extension. The extension installs a tabular model designer, which provides a design surface for creating semantic model objects like tables, partitions, relationships, hierarchies, measures, and KPIs.

Tabular models can be deployed to Power BI Premium, Azure Analysis Services, or an instance of SQL Server Analysis Services configured for Tabular server mode. Deployed tabular models can be managed in SQL Server Management Studio or by using many different tools.

Source: [Tabular modeling overview Microsoft learn](https://learn.microsoft.com/en-us/analysis-services/tabular-models/tabular-models-ssas?view=asallproducts-allversions)