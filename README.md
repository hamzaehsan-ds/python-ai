# python-ai

A small Python learning project and starter package for experimenting with Python and AI-related tools. The current command-line entry point prints a greeting; the repository also includes a NumPy arrays lab handout.

## Requirements

- Python 3.13 or newer
- [uv](https://docs.astral.sh/uv/) for environment and package management

## Getting started

Clone the repository and enter its directory:

```bash
git clone https://github.com/hamzaehsan-ds/python-ai.git
cd python-ai
```

Sync the project dependencies and create the virtual environment:

```bash
uv sync
```

Run the command-line application:

```bash
uv run python-ai
```

The current output is:

```text
Hello from python-ai!
```

You can also run the package module directly from the source tree:

```bash
uv run python -c "from python_ai import main; main()"
```

## Project layout

```text
.
├── labs/
│   └── Lab1-Using-NumPy-Arrays.pdf
├── src/
│   └── python_ai/
│       └── __init__.py
├── pyproject.toml
└── uv.lock
```

- `src/python_ai/` contains the installable Python package and its `python-ai` command.
- `labs/` contains learning materials, including the NumPy arrays PDF.
- `pyproject.toml` defines the package metadata and dependencies; `uv.lock` pins the resolved environment.

## Development

Install the project, including its declared dependencies, into the local environment with:

```bash
uv sync
```

Then invoke the CLI with `uv run python-ai`. The project currently has no test suite configured.
