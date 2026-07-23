# Wessel Developer Platform (WDP)

# Branch Strategy

## Purpose

This document defines the branching strategy used by WDP projects.

The objective is to keep development simple, maintain a stable `main` branch, and ensure all work is isolated into focused, short-lived branches.

WDP adopts the **GitHub Flow** branching model.

---

# Branch Philosophy

Branches represent **a single objective**.

A branch should answer one question:

> What capability or change is being developed?

Avoid mixing unrelated work in the same branch.

---

# Main Branch

The `main` branch is the source of truth.

It should always represent the latest stable version of the project.

Rules:

- Never commit directly to `main`.
- All changes arrive through Pull Requests.
- `main` should always be in a buildable state.

---

# Feature Branches

Every new feature starts from `main`.

Naming:

feature/<feature-name>

Examples:

feature/login

feature/report-export

feature/user-management

Feature branches should remain focused on a single feature.

---

# Bug Fix Branches

Bug fixes should be isolated.

Naming:

bugfix/<issue>

Examples:

bugfix/login-timeout

bugfix/payment-rounding

bugfix/report-filter

---

# Hotfix Branches

Production-critical fixes.

Naming:

hotfix/<issue>

Examples:

hotfix/security-patch

hotfix/payment-failure

Hotfixes should be merged into `main` as soon as they have been validated.

---

# Documentation Branches

Documentation improvements may be developed independently.

Naming:

docs/<topic>

Examples:

docs/architecture

docs/git-workflow

docs/api-documentation

---

# Refactoring Branches

Structural improvements that do not introduce new functionality.

Naming:

refactor/<area>

Examples:

refactor/authentication

refactor/repository-pattern

refactor/logging

---

# Branch Lifecycle

Every branch follows the same lifecycle.

```
main
    │
    ▼
Create Branch
    │
    ▼
Implement
    │
    ▼
Commit
    │
    ▼
Push
    │
    ▼
Pull Request
    │
    ▼
Review
    │
    ▼
Merge
    │
    ▼
Delete Branch
```

Branches should be deleted immediately after they are merged.

---

# Branch Lifetime

Branches should remain short-lived.

Prefer completing one feature before beginning another.

Long-lived branches increase merge conflicts and reduce visibility.

---

# Engineering Principle

One branch.

One objective.

One Pull Request.

Small branches are easier to review, easier to test, and easier to merge.

---

# AI Collaboration

When working with AI assistants:

- AI should suggest an appropriate branch name before implementation.
- AI should verify the current branch before making changes.
- AI should never implement multiple unrelated features on the same branch.
- AI should remind the developer to merge and delete completed branches.

AI should encourage disciplined version control throughout the development process.