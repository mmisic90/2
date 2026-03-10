# CLAUDE.md

This file provides guidance for AI assistants (Claude and others) working in this repository.

## Repository Overview

**Name:** 2
**Owner:** mmisic90
**Status:** Newly initialized — no source code yet.

This is a fresh Git repository with a single initial commit. There are no frameworks, languages, or build tools configured yet.

## Current Structure

```
/
├── README.md       # Minimal placeholder readme
└── CLAUDE.md       # This file
```

## Development Conventions

Since no stack has been chosen yet, follow these general conventions when adding code:

### General
- Keep the root directory clean. Group source code under `src/`, tests under `tests/` or `__tests__/`, and documentation under `docs/`.
- Commit messages should be clear and imperative: `Add login endpoint`, `Fix null pointer in parser`, not `stuff` or `WIP`.
- Never commit secrets, credentials, or `.env` files. Add them to `.gitignore` immediately.

### Starting a New Project
When a language or framework is introduced, update this file with:
- The chosen stack and why
- How to install dependencies
- How to run the project locally
- How to run tests
- Linting / formatting commands
- Any environment variables required (document them in `.env.example`)

## Git Workflow

- **Main branch:** `main` (tracked as `master` locally)
- **Feature branches:** Use descriptive names, e.g. `feature/user-auth`, `fix/typo-in-readme`
- Claude development branches follow the pattern: `claude/<task-slug>`
- Always push with: `git push -u origin <branch-name>`
- Do not force-push to `main`/`master`

## AI Assistant Guidelines

- Read existing code before suggesting modifications.
- Prefer editing existing files over creating new ones.
- Do not add boilerplate, comments, or docstrings to code you didn't change.
- Do not introduce over-engineered abstractions for simple tasks.
- When unsure about requirements, ask before implementing.
- After completing changes: commit with a clear message and push to the designated branch.
