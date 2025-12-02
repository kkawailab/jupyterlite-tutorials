# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

JupyterLite tutorials repository containing interactive Jupyter notebooks for learning Python data science libraries. Designed for browser-based delivery via JupyterLite (no local installation required for end users).

## Development Commands

```bash
# Environment setup
python -m venv .venv && source .venv/bin/activate
pip install -U jupyterlab jupyterlite nbconvert

# Edit notebooks
jupyter lab <notebook_name>.ipynb

# Verify notebook runs end-to-end (headless execution)
jupyter nbconvert --execute --inplace <notebook>.ipynb

# Build static JupyterLite site (outputs to _output/)
jupyter lite build
```

## Repository Structure

Flat structure by design. All notebooks at repo root follow naming pattern: `<topic>_jupyterlite_tutorial[_variant].ipynb`

Exercise notebooks: `python_[level]_exercises_[count].ipynb`

Large datasets or assets go in subdirectory named after the notebook (e.g., `pandas_jupyterlite_tutorial_assets/`).

## Coding Conventions

- 4-space indentation in Python cells
- Explicit imports (`import pandas as pd`) at top of first code cell
- Consistent Markdown headings across notebooks: `# Overview`, `## Setup`, etc.
- Helper functions in dedicated "Utilities" cell
- Strip cell outputs before committing unless tutorial depends on rendered chart (keep final output only)
- Set `numpy.random.seed` for any randomness (Monte Carlo, etc.) to ensure reproducibility

## Testing

No formal test framework. Each notebook execution is the test:
```bash
jupyter nbconvert --execute --inplace <notebook>.ipynb
```

Add assert statements or smoke checks in critical cells to surface failures early.

## Commit Guidelines

- Short imperative subjects under 60 characters (e.g., "Add folium layer walkthrough")
- Group notebook, asset, and documentation edits in same commit
- PRs should describe tutorial goal, list notebooks touched, include screenshots/GIFs for visual changes
