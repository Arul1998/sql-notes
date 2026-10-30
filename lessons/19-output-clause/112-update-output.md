# Lesson 112: OUTPUT with UPDATE

`OUTPUT` with `DELETED` and `INSERTED` shows the values before and after an update.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | 250 |
| 102 | 400 |

## Syntax

```sql
UPDATE table SET column = value OUTPUT DELETED.column, INSERTED.column WHERE condition;
```

## Example

```sql
UPDATE Orders SET Amount = Amount + 50
OUTPUT DELETED.Amount AS OldAmount, INSERTED.Amount AS NewAmount
WHERE OrderId = 101;
```

## Exercise

Update OrderId 101 by increasing Amount by 50. Return old and new amounts.
