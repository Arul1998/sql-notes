# Lesson 59 Answer: CONCAT Function

## Exercise

Display `CustomerName`, `City`, and `CustomerLocation` from `Customers`.

Join the name and city in this format: `Sarah - London`.

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
       CONCAT(CustomerName, ' - ', City) AS CustomerLocation
FROM Customers;
```

## Expected Result

### Result

| CustomerName | City | CustomerLocation |
|---|---|---|
| Sarah | London | Sarah - London |
| David | NULL | David -  |
| Priya | Chennai | Priya - Chennai |
| James | Manchester | James - Manchester |
| Amina | London | Amina - London |
