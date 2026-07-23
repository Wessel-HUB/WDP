# Wessel Developer Platform (WDP)

# Engineering Principles

## Purpose

This document defines the engineering philosophy used throughout the Wessel Developer Platform.

Every project created using WDP should follow these principles unless there is a clear and documented reason not to.

---

# 1. Understand Before Building

Design comes before implementation.

Before writing code:

- Understand the problem.
- Identify constraints.
- Ask questions.
- Produce a plan.
- Wait for approval.

Never write code simply because it is possible.

---

# 2. Simplicity Over Cleverness

Write code that is easy to understand.

Avoid unnecessary complexity.

Future maintainability is more important than writing fewer lines of code.

---

# 3. Consistency Creates Quality

Projects should feel familiar.

Folder structures, naming conventions, documentation, and architecture should remain consistent across every WDP project.

Consistency reduces mistakes.

---

# 4. Build Once. Reuse Forever.

If something can be reused:

- move it into Shared
- create a template
- document it

Every project should improve WDP.

---

# 5. Documentation Is Part of the Product

Documentation is never optional.

Architecture changes require documentation updates.

Database changes require documentation updates.

API changes require documentation updates.

Documentation should evolve alongside the code.

---

# 6. AI Assists. Humans Decide.

AI is a development partner.

It is not the architect.

It is not the product owner.

It is not responsible for production.

Humans make engineering decisions.

---

# 7. Features Are Built Incrementally

Large projects are divided into milestones.

Every milestone should:

- compile
- be testable
- be documented
- be commit-ready

Avoid long-lived unfinished work.

---

# 8. Protect the Main Branch

The main branch should always represent a stable version of the project.

Every feature should be developed on its own branch.

Changes should be reviewed before merging.

---

# 9. Automate Repetitive Work

If a task is repeated multiple times:

Automate it.

Examples include:

- project setup
- deployments
- testing
- documentation generation
- code formatting

Time spent automating is an investment.

---

# 10. Improve WDP Continuously

Every completed project should improve the platform.

Examples include:

- reusable libraries
- improved templates
- better documentation
- stronger Claude rules
- automation
- developer tooling

WDP is a living platform.

Every project leaves it better than it was before.

---

# Final Principle

The goal of WDP is not to write software faster.

The goal is to build better software with less repetitive effort while continuously improving the engineering platform that creates it.