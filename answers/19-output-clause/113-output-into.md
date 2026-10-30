# Lesson 113 Answer: OUTPUT INTO

## Exercise

Change OrderId 101 to Shipped and save its old and new status in an existing OrderAudit table.

## Sample Tables

**Orders**

| OrderId | Status |
|---:|---|
| 101 | Pending |

**OrderAudit (empty)**

| OrderId | OldStatus | NewStatus |
|---:|---|---|

## Answer

```sql
UPDATE Orders SET Status = 'Shipped'
OUTPUT INSERTED.OrderId, DELETED.Status, INSERTED.Status INTO OrderAudit (OrderId, OldStatus, NewStatus)
WHERE OrderId = 101;
```

## Expected Result

| OrderId | OldStatus | NewStatus |
|---:|---|---|
| 101 | Pending | Shipped |
