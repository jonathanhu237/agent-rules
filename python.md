# python.md

The rules in python.md are designed to instruct the agent how to use the tools within my system to execute Python scripts.

## Guidelines

- Use `mamba` to manage virtual environments. If not specified, the default virtual environment name will be the same as the working directory's name.
- If you need to print information to show the program's execution process, you should use `logging` package instead of directly using `print`.
- If a log contains multiple lines of information, consider using a raw string to output multiple lines instead of logging multiple times.