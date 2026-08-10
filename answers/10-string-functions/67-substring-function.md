# Lesson 67 Answer: SUBSTRING Function

## Exercise

Display `CustomerName` and `NamePart`.

Return three characters starting from the second character.

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
       SUBSTRING(CustomerName, 2, 3) AS NamePart
FROM Customers;
```

## Expected Result

### Result

| CustomerName | NamePart |
|---|---|
| Sarah | ara |
| David | avi |
| Priya | riy |
| James | ame |
| Amina | min |
