---
queries:
   - categories: categories.sql
---

# {params.category}

```sql categories_filtered
select * from ${categories}
where category = '${params.category}'
```

<DataTable data={categories_filtered}/>
