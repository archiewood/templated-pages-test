---
queries:
   - orders: orders.sql
---

# {params.order}

```sql orders_filtered
select * from ${orders}
where id = '${params.order}'
```

<DataTable data={orders_filtered}/>
