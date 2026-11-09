# Lesson 129: TRANSLATE

`TRANSLATE()` replaces individual characters according to their positions in two equal-length character lists. It is available in SQL Server 2017 and later.

## Sample Table

| EmployeeId | EmployeeCode |
|---:|---|
| 1 | EMP-101/IT |
| 2 | EMP/202-HR |
| 3 | EMP-303/FIN |

## Syntax

```sql
TRANSLATE(text, characters_to_find, replacement_characters)
```

## Example

```sql
SELECT TRANSLATE('A-B/C', '-/', '__') AS CleanCode;
```

## Exercise

Using `Employees`, display `EmployeeId` and `UpdatedEmployeeCode`. Replace each hyphen (`-`) in `EmployeeCode` with `_` and each slash (`/`) with `#` using `TRANSLATE()`.
