# Wessel Developer Platform (WDP)

# Platform Structure

## Purpose

This document defines the structure of the **WDP repository itself**.

WDP is the engineering platform that provides shared knowledge, standards, templates, reusable patterns, and automation for all future projects.

---

## Repository Layout

WDP
│
├── docs/
├── templates/
├── shared/
├── tools/
│
├── README.md
├── CHANGELOG.md
├── LICENSE
└── .gitignore
```

---

## Folder Definitions

### docs

Contains all WDP platform documentation.

Examples:

* Vision
* Architecture
* Engineering Principles
* Naming Conventions
* Git Workflow
* Coding Standards
* Roadmap
* Decision Log

This folder documents **how WDP works**.

---

### templates

Contains project templates for different technology stacks.

Examples:

templates/
├── framework48/
├── dotnet8/
├── python/
└── winforms/
```

Each template contains a complete project structure that can be used as the starting point for a new application.

---

### shared

Contains reusable assets that can be shared across multiple projects.

Examples:

shared/
├── auth/
├── logging/
├── utilities/
├── ui/
└── patterns/
```

The `patterns/` folder stores documented solutions to recurring engineering problems.

---

### tools

Contains automation and developer tooling.

Examples:

tools/
├── cli/
├── generators/
└── scripts/
```

This folder will eventually contain the WDP CLI and project-generation automation.

---

## Platform Philosophy

* Keep the platform structure shallow and easy to navigate.
* Add new top-level folders only when there is a demonstrated need.
* Shared knowledge belongs in `docs`.
* Reusable code and patterns belong in `shared`.
* Project starting points belong in `templates`.
* Automation belongs in `tools`.

The WDP repository should remain the single source of truth for the platform’s standards, templates, and reusable engineering assets.
