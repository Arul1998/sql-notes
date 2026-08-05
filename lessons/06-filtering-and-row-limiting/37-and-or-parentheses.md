# Lesson 37: Combining AND and OR with Parentheses

Parentheses control how SQL evaluates combined `AND` and `OR` conditions.

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
SELECT columns
FROM table_name
WHERE condition1 AND (condition2 OR condition3);
```

## Example

```sql
SELECT *
FROM Customers
WHERE CustomerId > 1
  AND (City = 'London' OR City = 'Manchester');
```

Use parentheses to make the intended logic clear.

## Exercise

Display customers with `CustomerId` greater than 2 who live in London or Birmingham.