# Lesson 7 Answer: DISTINCT

## Exercise

Display the unique employee ages from the `Employees` table, sorted from youngest to oldest.

## Sample Table

### Employees

| EmployeeName | Department | Age |
|---|---|---:|
| Arul | IT | 28 |
| Priya | Finance | 32 |
| John | IT | 25 |
| Sara | Finance | 35 |
| Adam | Sales | 29 |

## Answer

```sql
SELECT DISTINCT Age
FROM Employees
ORDER BY Age ASC;
```

## Expected Result

| Age |
|---:|
| 25 |
| 28 |
| 29 |
| 32 |
| 35 |
