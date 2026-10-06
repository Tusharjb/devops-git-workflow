# Git Workflow

This project follows a structured Git branching workflow to demonstrate version control best practices.

## Branch Strategy

- `main` — stable, production-ready code
- `dev` — integration branch for completed features
- `feature/*` — isolated development branches for individual features

## Workflow

Feature branches are created from `dev`.

Completed features are merged into `dev` through Pull Requests.

After validation, `dev` is promoted to `main` through a final Pull Request.

## Release Strategy

Stable versions on `main` are identified using annotated Git tags such as:

`v1.0.0`