# Lesson 62 Answer: UPPER Function

## Exercise

Display `CustomerName` and `UppercaseName`.

Use `UPPER` on each customer name.

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
       UPPER(CustomerName) AS UppercaseName
FROM Customers;
```

## Expected Result

### Result

| CustomerName | UppercaseName |
|---|---|
| Sarah | SARAH |
| David | DAVID |
| Priya | PRIYA |
| James | JAMES |
| Amina | AMINA |
