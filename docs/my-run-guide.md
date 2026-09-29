# Run Guide: Library Loan Demo

## Prerequisites

- JDK 17 or later (`java` and `javac` must be on your `PATH`)
- Python 3.9 or later
- A clone of this repository (no Maven, Gradle, or third-party library is needed)

## Run the demo

From the repository root:

```text
python3 run.py demo
```

On Windows, use `py -3 run.py demo` if that is how you start Python 3.

## What the demo does

`run.py` compiles the Java sources in `src/library/` into a temporary directory and runs `library.Main`.
The demo uses a fixed date (2026-09-01) so its output is reproducible. It:

1. Adds three books to the catalog and registers a student (Alex) and a faculty member (Dr. Lee).
2. Prints the student and faculty borrowing limits.
3. Searches the catalog for `git`.
4. Lets the student borrow *Git Essentials*, prints the loan receipt and due date, then returns the book and prints the return fee and the number of active loans.
