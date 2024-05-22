---
queries:
   - categories: orders.sql
---

# {params.id}

```sql orders_filtered
select * from ${orders}
where id = '${params.id}'
```

<DataTable data={orders_filtered}/>
