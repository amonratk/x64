# How to look structure of table

## MySQL

```bash
> describe tableName;
```

## SQL Server

```bash
> select * from Information_schema.columns  where table_name='table_name';
```