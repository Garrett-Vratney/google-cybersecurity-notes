# Chapter 7, Module 3 · Python Strings, Lists, and Regular Expressions

[Back to index](../README.md)

## Topics Covered

- String conversion, methods, and slicing
- List mutation and iteration
- Regular expressions for log parsing

## Study Notes

String and list indexing starts at zero. A slice includes its start index and excludes its stop index. Strings are immutable, while lists support operations such as `append`, `insert`, and `remove`. The `index` method returns the first matching position and raises `ValueError` if the item is absent. Use raw strings for regex patterns. `re.findall(r'\buser=([\w.-]+)', log_text)` extracts usernames from a simple synthetic log format.

## Key Takeaways

- Use list operations to collect parsed values and string methods to normalize them.
- Match against realistic and malformed sample lines before relying on a regex.
- Use `ipaddress` to validate and group IP addresses.

## Source

Personal course notes in `Ch 7 module 3.docx`.
