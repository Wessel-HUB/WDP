# Wessel Developer Platform (WDP)

# Standard Project Structure

## Purpose

This document defines the standard folder structure used by all projects generated from WDP templates.

The goal is to ensure that every project is organized consistently, making navigation, maintenance, automation, and AI-assisted development predictable.

---

## Standard Project Layout

```text
ProjectRoot
│
├── .claude/
├── .github/
├── .vscode/
│
├── docs/
├── scripts/
├── shared/
├── src/
├── tests/
│
├── README.md
├── PROJECT.md
├── TASKS.md
├── CHANGELOG.md
├── LICENSE
└── .gitignore
```

---

## Folder Definitions

### .claude

Claude-specific configuration and project guidance.

Examples:

* `CLAUDE.md`
* Prompt library
* Engineering rules

---

### .github

GitHub configuration.

Examples:

* GitHub Actions
* Issue templates
* Pull Request templates
* CODEOWNERS

---

### .vscode

Visual Studio Code workspace settings.

Examples:

* `settings.json`
* `launch.json`
* `tasks.json`
* `extensions.json`

---

### docs

Project-specific documentation.

Examples:

* Architecture
* API documentation
* Database documentation
* Deployment guides
* Decision logs

Documentation is considered part of the product.

---

### scripts

Utility scripts used during development and deployment.

Examples:

* Build scripts
* Deployment scripts
* Database migration scripts
* Environment setup scripts

---

### shared

Reusable components shared within the project.

Examples:

* Authentication helpers
* Logging utilities
* Common models
* Shared UI components

---

### src

Application source code.

The internal structure of this folder is defined by the selected WDP template.

Examples:

* `Web`
* `Api`
* `Desktop`
* `Services`

---

### tests

Automated tests.

Examples:

* Unit tests
* Integration tests
* Performance tests

---

## Root Documents

### README.md

Public-facing project overview.

### PROJECT.md

Project requirements, scope, and business context.

### TASKS.md

Development backlog and implementation progress.

### CHANGELOG.md

Version history and release notes.

---

## Project Philosophy

* Every folder has a single, clearly defined purpose.
* Avoid unnecessary nesting.
* Keep related code together.
* Documentation evolves with the code.
* New folders are introduced only when there is a demonstrated need.

Developers should be able to navigate any WDP-generated project with minimal effort because every project follows the same organizational philosophy.
