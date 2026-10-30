# Lesson 119: TRY_PARSE

`TRY_PARSE` safely parses text into a number or date.

## Sample Table

| Value |
|---|
| 125.50 |

## Syntax

```sql
TRY_PARSE(string_value AS data_type [USING culture])
```

## Example

```sql
SELECT TRY_PARSE('125.50' AS DECIMAL(10,2)
USING 'en-US') AS ParsedAmount;
```

## Exercise

Convert '125.50' into DECIMAL(10,2) using TRY_PARSE.
