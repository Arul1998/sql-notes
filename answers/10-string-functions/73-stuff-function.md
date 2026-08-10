# Lesson 73 Answer: STUFF Function

## Exercise

Display `CustomerName` and `HiddenName`.

Replace the first three characters of each name with `***`.

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
       STUFF(CustomerName, 1, 3, '***') AS HiddenName
FROM Customers;
```

## Expected Result

### Result

| CustomerName | HiddenName |
|---|---|
| Sarah | ***ah |
| David | ***id |
| Priya | ***ya |
| James | ***es |
| Amina | ***na |
