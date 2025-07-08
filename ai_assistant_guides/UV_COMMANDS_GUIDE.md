# UV Commands Guide


This guide provides essential UV commands for Python project dependency management and automation. Use these commands to ensure reproducible environments and efficient workflows. All usage MUST comply with the AI Assistant Guidelines:
- Use imperative, unambiguous language (MUST, NEVER, ALWAYS).
- Name files and directories in English by default, following the naming policy.
- Validate and document all file operations and changes.
- Ensure autonomy in routine documentation and cleanup actions.

## Basic Commands

- `uv sync`  
  Install all dependencies from `pyproject.toml` and `uv.lock`.

- `uv add <package>`  
  Add a new dependency and update lockfile.

- `uv run <command>`  
  Run a command inside the UV-managed environment.

- `uv run pytest tests/ -v`  
  Run all tests with verbose output.

## Example Workflow
```bash
uv sync
uv run pre-commit run --all-files
uv run pytest tests/ -v
uv run python scripts/your_script.py --help
```

## Tips
- Always run `uv sync` after modifying dependencies.
- Use `uv run` to ensure commands use the correct environment.
- Keep `uv.lock` under version control for reproducibility.


> For more details, see https://github.com/astral-sh/uv
