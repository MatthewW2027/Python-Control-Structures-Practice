# Copilot instructions for this repository

## Repository purpose

This repository is a small Python learning exercise focused on control structures. The project is intentionally minimal: all exercises live in a single file, `main.py`, and each section is built around a specific topic such as conditionals, loops, dictionaries, and debugging.

## Build, test, and validation commands

There is no package manager, test runner, or linter configured for this repo.

Use the file itself as the validation target:

- Syntax check: `python -m py_compile main.py`
- Exercise validation: uncomment the matching `print(...)` call in the `if __name__ == "__main__":` block, then run `python main.py`

Example:

```bash
python -m py_compile main.py
python main.py
```

The repository does not define a full automated test suite. Most validation is manual and intentionally exercise-specific.

## High-level architecture

- `main.py` is the entire application and learning scaffold.
- The file is organized into numbered sections, each with a brief prompt and a function skeleton to complete.
- Exercises are intentionally self-contained; each function typically solves one isolated problem without shared state or external dependencies.
- The bottom of the file contains a manual testing section where specific functions are exercised by uncommenting a print statement.
- This is not a production app or library; it is a practice file for mastering Python control-flow patterns.

## Key conventions in this codebase

- Keep the function names and signatures exactly as defined in the prompt comments.
- Follow the instructions in the comments above each exercise; they describe the intended behavior and often include examples.
- Many exercises expect specific Python patterns, such as:
  - `if/elif/else` ordering for precedence
  - `while` loops with a loop-control variable that changes each iteration
  - `range(start, stop, step)` for numeric sequences
  - `enumerate()` when printing numbered output
  - `.items()` for dictionary iteration
  - `continue` and `return` inside loops for filtering and early exit
- The prompt comments are the source of truth for expected behavior, not generic Python style rules.
- When a comment says to answer a conceptual question, the answer belongs in a comment next to the prompt; do not convert it into code unless asked.
- Do not introduce extra modules, frameworks, or project structure unless the task explicitly requires it.

## Working style for future edits

- Prefer small, direct implementations that match the exercise requirements exactly.
- Keep solutions readable and local to the relevant function.
- Do not refactor unrelated exercises or rewrite the file into a larger app structure.
- If an exercise is intentionally incomplete (for example, `pass` is left as a placeholder), fill in only that function body and leave surrounding prompts/comments intact.
