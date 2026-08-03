# Lesson 1: SELECT

`SELECT` is used to read data from a table.

Imagine this `Customers` table:

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | John | Manchester |
| 3 | Priya | London |
| 4 | Sara | Birmingham |

To display every column:

```sql
SELECT *
FROM Customers;
```

- `SELECT` means what information you want.
- `*` means every column.
- `FROM` means which table contains it.

To display only names:

```sql
SELECT CustomerName
FROM Customers;
```

To display names and cities:

```sql
SELECT CustomerName, City
FROM Customers;
```

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name;
```

## Exercise

Write a query that displays only `CustomerId` and `CustomerName` from the `Customers` table.
