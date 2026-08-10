# Lesson 70 Answer: REVERSE Function

## Exercise

Display `CustomerName` and `ReversedName`.

Reverse each customer name.

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
       REVERSE(CustomerName) AS ReversedName
FROM Customers;
```

## Expected Result

### Result

| CustomerName | ReversedName |
|---|---|
| Sarah | haraS |
| David | divaD |
| Priya | ayirP |
| James | semaJ |
| Amina | animA |
