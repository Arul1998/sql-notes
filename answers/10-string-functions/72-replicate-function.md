# Lesson 72 Answer: REPLICATE Function

## Exercise

Display `CustomerName` and `NamePattern`.

Repeat each customer name three times.

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
       REPLICATE(CustomerName, 3) AS NamePattern
FROM Customers;
```

## Expected Result

### Result

| CustomerName | NamePattern |
|---|---|
| Sarah | SarahSarahSarah |
| David | DavidDavidDavid |
| Priya | PriyaPriyaPriya |
| James | JamesJamesJames |
| Amina | AminaAminaAmina |
