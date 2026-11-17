# Project: Human Activity Recognition

## Overview
Classify human activities (walking, sitting, standing, stairs) from smartphone
accelerometer and gyroscope data. Course: Big Data Analytics, Group 11.

## Commands
- Setup: `uv sync`
- Test: `uv run pytest`
- Lint: `uv run ruff check . && uv run ruff format .`
- Train: `uv run python -m har train`
- Dashboard: `uv run streamlit run app/dashboard.py`

## Conventions
- Code lives in `src/har/`, tests in `tests/` mirror the module names
- Type hints on all functions, short docstrings
- No hardcoded paths or magic numbers: use `configs/default.yaml`
- Fixed random seed (42) for reproducibility
- Never commit raw data or large model files

## Workflow
- Branch from main: `feature/<short-name>`
- Commit style: Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`)
- Every change goes through a pull request; CI must pass