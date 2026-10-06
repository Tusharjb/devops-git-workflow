# Git Workflow Documentation

## Overview

This project uses a structured Git workflow to keep development isolated, reviewable, traceable, and release-ready.

## Branch Strategy

### `main`

Production-ready branch containing stable releases.

Direct feature development is not performed on `main`.

### `dev`

Integration branch used to combine completed and reviewed features before production promotion.

### `feature/*`

Short-lived development branches used to isolate individual changes.

Feature branches are created from `dev` and merged back through GitHub Pull Requests.

---

## Workflow

```text
feature/*
    │
    │ Pull Request
    ▼
   dev
    │
    │ Integration / Validation
    │
    │ Pull Request
    ▼
  main
    │
    ▼
 Version Tag