# python.md

The rules in python.md are designed to instruct the agent how to use the tools within my system to execute Python scripts.

## Guidelines

- Use `mamba` to manage virtual environments. If not specified, the default virtual environment name will be the same as the working directory's name.
- If you need to print information to show the program's execution process, you should use `logging` package instead of directly using `print`.
- If a log contains multiple lines of information, consider using a raw string to output it as a single log entry, rather than logging multiple times. For example:
```python
logging.info(f"""User Update Event:
ID: {user.id}
Status: {user.status}
Timestamp: {datetime.now()}""")
```
- A Python function's parameters and return value should include type hints. For example:
```python
def greet(name: str, is_formal: bool) -> str:
    if is_formal:
        return f"Good day, {name}."
    else:
        return f"Hello, {name}!"
```