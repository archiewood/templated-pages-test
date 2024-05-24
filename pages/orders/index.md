---
title: Orders
queries:
   - orders: orders.sql
---

<DateRange
   name=daterange
   start="2019-01-01"
   end="2021-12-31"
/>

Click on an item to see more detail

```sql orders_with_link
select id, order_datetime, '/orders/' || id as link
from ${orders}
where order_datetime between '${inputs.daterange.start}' and '${inputs.daterange.end}'
limit 20
```

<DataTable data={orders_with_link} link=link/>
