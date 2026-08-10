# Lesson 65 Answer: LEFT Function

## Exercise

Display `CustomerName` and `FirstTwoLetters`.

Use `LEFT` to return the first two characters.

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
       LEFT(CustomerName, 2) AS FirstTwoLetters
FROM Customers;
```

## Expected Result

### Result

| CustomerName | FirstTwoLetters |
|---|---|
| Sarah | Sa |
| David | Da |
| Priya | Pr |
| James | Ja |
| Amina | Am |
