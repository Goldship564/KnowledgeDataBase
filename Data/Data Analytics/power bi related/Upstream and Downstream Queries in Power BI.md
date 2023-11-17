---
tags:
  - data-science
  - data-analytics
  - power-bi
---
Terms commonly use by data professionals. 
## Benefits
- Sometime making changes to the upstream queries would create more efficiency to Power Query
- Consolidating business logic using upstream and downstream queries can make your power query more easy to understand for you and for other developers. 
- If you need to update logic in the future you will only need to update the upstream queries and it will reflect in the downstream queries. However, this can also be a disadvantage as it can create unintended effect to the downstream queries

## Upstream Queries
The source queries (the original).
Modifying it will affect all the downstream queries. Thus if you need to update all the downstream queries. You should modify the upstream queries

## Downstream Queries
Queries created using the upstream queries