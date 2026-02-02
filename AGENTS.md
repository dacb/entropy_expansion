# AGENTS.md: Python Project Guidelines

This project is a simple Python application for computing the entropy of a random variable.  It is primarily a demonstration of how to build a project and test a simple file.

## Project Structure
*   `src/`: Contains all application-level Python code.
*   `tests/`: Contains test files for `pytest`.
*   `pyproject.toml`, `uv.lock`: Configuration files for package management and tools.

## Setup Commands
*   This project uses `uv` for all package management.
*   **Never** run commands directly (e.g., `python`, `pip`, `pytest`).
*   **Always** prefix commands with `uv run <command>`.

### Examples:
*   To run a script: `uv run python src/main.py`
*   To install dependencies: `uv sync` (or `uv pip install -r requirements.txt` if using a `requirements.txt` file)
*   To run tests: `uv run pytest`

## Testing Instructions
*   Tests are located in the `tests/` directory.
*   The command `uv run pytest` will run the entire test suite.
*   Ensure all tests pass before committing any changes.

## Coding Style
*   Maintain existing code formatting.
*   Use `ruff` for linting and formatting.
*   You can run `uv run ruff format` and `uv run ruff check` to ensure compliance.
*   Prefer type hints where appropriate.
