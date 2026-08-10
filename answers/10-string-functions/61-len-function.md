# Lesson 61 Answer: LEN Function

## Exercise

Display `CustomerName` and `NameLength`.

Use `LEN` to count the characters in each customer name.

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
       LEN(CustomerName) AS NameLength
FROM Customers;
```

## Expected Result

### Result

| CustomerName | NameLength |
|---|---:|
| Sarah | 5 |
| David | 5 |
| Priya | 5 |
| James | 5 |
| Amina | 5 |
