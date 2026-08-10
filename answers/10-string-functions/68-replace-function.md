# Lesson 68 Answer: REPLACE Function

## Exercise

Display `CustomerName`, `City`, and `UpdatedCity`.

Change `London` to `Greater London` in the `City` column.

## Sample Table

| CustomerId | CustomerName | City | Country |
|---:|---|---|---|
| 1 | Sarah | London | UK |
| 2 | David | NULL | UK |
| 3 | Priya | Chennai | India |
| 4 | James | Manchester | NULL |
| 5 | Amina | London | UK |

## Answer

```sql
SELECT CustomerName,
       City,
       REPLACE(City, 'London', 'Greater London') AS UpdatedCity
FROM Customers;
```

## Expected Result

### Result

| CustomerName | City | UpdatedCity |
|---|---|---|
| Sarah | London | Greater London |
| David | NULL | NULL |
| Priya | Chennai | Chennai |
| James | Manchester | Manchester |
| Amina | London | Greater London |
