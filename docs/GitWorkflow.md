# Wessel Developer Platform (WDP)

# Git Workflow

## Purpose

This document defines the standard Git workflow used by all WDP projects.

The objective is to keep the repository stable, maintain a clear history, and ensure every change is isolated, reviewable, and reversible.

WDP follows a simplified GitHub Flow.

---

# Branches

## main

The `main` branch always represents the latest stable version of the project.

Direct commits to `main` are discouraged.

All work should be completed on feature branches and merged back into `main`.

---

## Feature Branches

Every new feature begins with a new branch created from `main`.

Examples

feature/login

feature/payment-report

feature/report-export

feature/github-actions

---

## Bug Fix Branches

Bug fixes should be isolated.

Examples

bugfix/login-timeout

bugfix/payment-rounding

bugfix/api-authentication

---

## Hotfix Branches

Critical production fixes.

Examples

hotfix/security-patch

hotfix/payment-failure

---

## Documentation Branches

Documentation changes may be developed independently.

Examples

docs/naming-conventions

docs/git-workflow

docs/platform-architecture

---

# Development Workflow

1. Switch to the latest `main`

```
git checkout main
git pull
```

2. Create a feature branch

```
git checkout -b feature/my-feature
```

3. Implement the feature

4. Commit regularly using Conventional Commits

5. Push the branch

```
git push -u origin feature/my-feature
```

6. Open a Pull Request

7. Review the changes

8. Merge into `main`

9. Delete the feature branch

---

# Commit Strategy

Commit early.

Commit often.

Each commit should represent a logical unit of work.

Avoid combining unrelated changes into a single commit.

Good examples:

- Create authentication service
- Add login endpoint
- Update documentation

Poor example:

- Fixed stuff

---

# Commit Messages

WDP follows the Conventional Commits specification.

Examples

feat(auth): add JWT authentication

fix(api): correct login validation

docs(platform): add Git workflow documentation

refactor(sql): simplify repository pattern

---

# Pull Requests

Every Pull Request should answer three questions:

- What changed?
- Why was it changed?
- How was it tested?

Pull Requests should remain focused on a single objective.

---

# Branch Cleanup

After merging:

Delete the feature branch locally.

```
git branch -d feature/my-feature
```

Delete the remote branch.

```
git push origin --delete feature/my-feature
```

---

# Release Tags

Stable milestones should be tagged.

Examples

v0.1.0

v0.2.0

v1.0.0

Tags represent meaningful platform or project releases.

---

# WDP Philosophy

Git is more than version control.

It is the engineering history of the project.

A clean Git history tells the story of how software evolved over time.