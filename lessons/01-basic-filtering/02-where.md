# Lesson 2: WHERE

`WHERE` is used to filter rows from a table.

Imagine this `Customers` table:

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | John | Manchester |
| 3 | Priya | London |
| 4 | Sara | Birmingham |

To display customers from London:

```sql
SELECT *
FROM Customers
WHERE City = 'London';
```

- `WHERE` means which rows you want.
- `City = 'London'` checks whether the city is London.
- Text values such as `London` must be inside single quotes.

To display only the names of customers from London:

```sql
SELECT CustomerName
FROM Customers
WHERE City = 'London';
```

To display the name and city of a specific customer:

```sql
SELECT CustomerName, City
FROM Customers
WHERE CustomerId = 2;
```

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name
WHERE condition;
```

## Exercise

Write a query that displays `CustomerName` and `City` for customers who live in `Birmingham`.
