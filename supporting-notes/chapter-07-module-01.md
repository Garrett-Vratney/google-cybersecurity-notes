# Chapter 7, Module 1 · Python Fundamentals for Security Automation

[Back to index](../README.md)

## Topics Covered

- Data types and variables
- Comparisons and Boolean operators
- Conditionals and loops
- Break and continue

## Study Notes

Strings represent text, lists hold ordered values, tuples hold fixed sequences, and dictionaries map keys to values. Use `if`, `elif`, and `else` to choose an action. `and` requires both conditions to be true, while `or` requires at least one. Use a `for` loop to iterate through a collection and a `while` loop to repeat while a condition holds. `break` exits the loop and `continue` skips to the next iteration.

```python
for status in [200, 404, 503]:
    if 500 <= status < 600:
        print(f"Review server error {status}")
```

## Key Takeaways

- Match the data type to the task and use type() when debugging.
- Test the endpoints of a range and every conditional branch.
- Make sure a while loop can reach its stopping condition.

## Source

Personal course notes in `Course 7 Module 1.docx`.
