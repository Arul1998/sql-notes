# Lesson 69 Answer: CHARINDEX Function

## Exercise

Display `CustomerName` and `LetterPosition`.

Find the position of the first letter `a` in each name.

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
       CHARINDEX('a', CustomerName) AS LetterPosition
FROM Customers;
```

## Expected Result

### Result

| CustomerName | LetterPosition |
|---|---:|
| Sarah | 2 |
| David | 2 |
| Priya | 5 |
| James | 2 |
| Amina | 1 |
