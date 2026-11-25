# Chapter 7, Module 4 · Python Automation and DevSecOps

[Back to index](../README.md)

## Topics Covered

- Reading and writing text files
- Parsing and counting log records
- Debugging syntax, runtime, and logic errors
- Security checks in CI/CD

## Study Notes

Use `with open(..., encoding='utf-8')` to close files automatically. Read with `r`, append with `a`, and overwrite with `w`. Split simple whitespace-delimited records or use a parser for structured data. Count matching records and verify threshold behavior against known examples. CI/CD checks can review dependencies, configurations, and secrets handling, then enforce a documented release policy.

## Key Takeaways

- Test empty files, malformed records, and exact threshold values.
- Keep credentials in a secret manager and out of source and logs.
- Make automation failures visible and distinguish failed checks from tool errors.

## Source

Personal course notes in `ch 7 module 4.docx`.
