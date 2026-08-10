# Lesson 63 Answer: LOWER Function

## Exercise

Display `CustomerName` and `LowercaseName`.

Use `LOWER` on each customer name.

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
       LOWER(CustomerName) AS LowercaseName
FROM Customers;
```

## Expected Result

### Result

| CustomerName | LowercaseName |
|---|---|
| Sarah | sarah |
| David | david |
| Priya | priya |
| James | james |
| Amina | amina |
