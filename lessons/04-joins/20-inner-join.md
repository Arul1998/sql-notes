# Lesson 20: INNER JOIN

`INNER JOIN` combines matching rows from two tables.

Imagine these tables:

**Customers**

| CustomerId | CustomerName |
|---:|---|
| 1 | Arul |
| 2 | Priya |
| 3 | John |
| 4 | Sara |

**Orders**

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |

To display customers and their orders:

```sql
SELECT
    Customers.CustomerName,
    Orders.OrderId,
    Orders.Amount
FROM Customers
INNER JOIN Orders
    ON Customers.CustomerId = Orders.CustomerId;
```

`ON` specifies how the tables are connected. Sara is excluded because she has no matching order.

SQL generally follows this pattern:

```sql
SELECT columns
FROM first_table
INNER JOIN second_table
    ON first_table.shared_column = second_table.shared_column;
```

## Exercise

Display `CustomerName` and `Amount` by joining `Customers` and `Orders`. Show only orders whose amount is at least £300.
