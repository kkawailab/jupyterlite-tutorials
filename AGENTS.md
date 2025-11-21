# Repository Guidelines

## Project Structure & Module Organization
The repository is intentionally flat: each `.ipynb` at the repo root is a fully scoped tutorial (e.g., `pandas_jupyterlite_tutorial.ipynb`, `leaflet_folium_jupyterlite_tutorial.ipynb`). Notebook names follow the pattern `<topic>_jupyterlite_tutorial[_variant].ipynb`; keep new content consistent so automation and humans can locate related notebooks quickly. Put large datasets or reusable assets beside the notebook in a subdirectory named after the notebook (for example, `pandas_jupyterlite_tutorial_assets/`) to avoid cluttering the top level.

## Build, Test, and Development Commands
Run notebooks locally with JupyterLab or publish them through JupyterLite:

- `python -m venv .venv && source .venv/bin/activate` — create an isolated environment.
- `pip install -U jupyterlab jupyterlite nbconvert` — install the lightweight toolchain used across tutorials.
- `jupyter lab pandas_jupyterlite_tutorial.ipynb` — open a notebook for interactive editing.
- `jupyter lite build` — bundle the notebooks into a static JupyterLite site (outputs to `_output/`).
- `jupyter nbconvert --execute statsmodels_jupyterlite_tutorial_v2.ipynb` — execute a notebook headlessly to verify it still runs end-to-end.

## Coding Style & Naming Conventions
Use 4-space indentation inside Python cells, prefer explicit imports (`import pandas as pd`) at the top of the first code cell, and keep Markdown headings mirrored across notebooks (`# Overview`, `## Setup`, etc.) for navigability. When adding helper functions, place them in a dedicated “Utilities” cell so downstream readers can locate reusable snippets. Strip lingering output before committing unless the tutorial depends on the rendered chart; in that case, keep the final cell output only.

## Testing Guidelines
Treat each notebook execution as the primary test. Run `jupyter nbconvert --execute --inplace <notebook>` before opening a PR to ensure all cells run with a clean kernel. If you introduce randomness (e.g., Monte Carlo examples), set a `numpy.random.seed` in the setup cell so reproducible builds remain deterministic. There is no formal coverage gate, but add assert statements or simple smoke checks in critical cells to surface failures early.

## Commit & Pull Request Guidelines
Use short, imperative commit subjects under 60 characters (`"Add folium layer walkthrough"`). Group notebook, asset, and documentation edits in the same commit so reviewers can follow the narrative end-to-end. Pull requests should describe the tutorial’s goal, list the notebooks touched, and embed screenshots or GIFs when visual output changes. Link to any issue or roadmap item and mention required follow-up tasks (such as dataset size reductions) before requesting review.
