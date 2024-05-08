---
title: Categories
queries:
   - categories: categories.sql
---

Click on an item to see more detail


```sql categories_with_link
select *, '/categories/' || category as link
from ${categories}
```

<DataTable data={categories_with_link} link=link/>
