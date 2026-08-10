# Lesson 66 Answer: RIGHT Function

## Exercise

Display `CustomerName` and `LastTwoLetters`.

Use `RIGHT` to return the last two characters.

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
       RIGHT(CustomerName, 2) AS LastTwoLetters
FROM Customers;
```

## Expected Result

### Result

| CustomerName | LastTwoLetters |
|---|---|
| Sarah | ah |
| David | id |
| Priya | ya |
| James | es |
| Amina | na |
