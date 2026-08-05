# Lesson 30: Selecting Distinct Values

`DISTINCT` removes duplicate values from a query result.

## Sample Table

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | Priya | Manchester |
| 3 | John | London |
| 4 | Sara | Birmingham |
| 5 | Maya | Manchester |

## Syntax

```sql
SELECT DISTINCT column_name
FROM table_name;
```

## Example

```sql
SELECT DISTINCT City
FROM Customers;
```

Each different value appears only once.

## Exercise

Display each different `CustomerId` from the `Orders` table.