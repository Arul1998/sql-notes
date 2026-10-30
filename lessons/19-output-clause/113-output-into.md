# Lesson 113: OUTPUT INTO

`OUTPUT INTO` saves changed-row details into another table.

## Sample Tables

**Orders**

| OrderId | Status |
|---:|---|
| 101 | Pending |

**OrderAudit (empty)**

| OrderId | OldStatus | NewStatus |
|---:|---|---|

## Syntax

```sql
UPDATE table SET column = value OUTPUT INSERTED.Id, DELETED.column, INSERTED.column INTO audit_table (Id, OldValue, NewValue) WHERE condition;
```

## Example

```sql
UPDATE Orders SET Status = 'Shipped'
OUTPUT INSERTED.OrderId, DELETED.Status, INSERTED.Status INTO OrderAudit (OrderId, OldStatus, NewStatus)
WHERE OrderId = 101;
```

## Exercise

Change OrderId 101 to Shipped and save its old and new status in an existing OrderAudit table.
