# Lesson 24: INSERT

`INSERT` adds a new row to a table.

Imagine this `Customers` table:

| CustomerId | CustomerName |
|---:|---|
| 1 | Arul |
| 2 | Priya |
| 3 | John |
| 4 | Sara |

To add a new customer:

```sql
INSERT INTO Customers (CustomerId, CustomerName)
VALUES (5, 'David');
```

- List the columns after the table name.
- List the matching values in the same order.
- Text values require single quotes.
- Numeric values do not require quotes.

SQL generally follows this pattern:

```sql
INSERT INTO table_name (column1, column2)
VALUES (value1, value2);
```

## Exercise

Insert a new order into `Orders` with:

- `OrderId`: 105
- `CustomerId`: 4
- `Amount`: 250
