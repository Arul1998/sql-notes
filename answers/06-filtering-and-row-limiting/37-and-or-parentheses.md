# Lesson 37 Answer: Combining AND and OR with Parentheses

## Exercise

Display customers with `CustomerId` greater than 2 who live in London or Birmingham.

## Sample Table

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | Priya | Manchester |
| 3 | John | London |
| 4 | Sara | Birmingham |
| 5 | Maya | Manchester |

## Answer

```sql
SELECT *
FROM Customers
WHERE CustomerId > 2
  AND (City = 'London' OR City = 'Birmingham');
```

## Expected Result

### Result

| CustomerId | CustomerName | City |
|---:|---|---|
| 3 | John | London |
| 4 | Sara | Birmingham |