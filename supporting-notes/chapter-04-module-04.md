# Chapter 4, Module 4 · SQL for Security Analysis

[Back to index](../README.md)

## Topics Covered

- Relational databases and keys
- SELECT, WHERE, and ORDER BY
- Pattern, range, and logical filters
- Joins and aggregate functions

## Study Notes

A primary key identifies each row. A foreign key references a key in a related table. Use `SELECT` to choose columns, `WHERE` to specify conditions, and `ORDER BY` to sort. `LIKE` uses `%` for zero or more characters and `_` for one character. `BETWEEN` includes both endpoints. An inner join keeps matched rows, while a left join also preserves unmatched rows from the left table. Use `IS NULL` to check missing values.

```sql
SELECT username, COUNT(*) AS failed_attempts
FROM login_attempts
WHERE outcome = 'failure'
GROUP BY username
ORDER BY failed_attempts DESC;
```

## Key Takeaways

- Query the fields you need and use a clear time range.
- Check whether joins duplicate rows before interpreting counts.
- Use parentheses to make combinations of AND and OR explicit.

## Source

Personal course notes in `Untitled document(1).docx`.
