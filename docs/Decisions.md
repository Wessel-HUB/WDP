# Wessel Development Platform (WDP)

# Decisions

## Purpose

This document records significant architectural and engineering decisions made during the evolution of WDP.

Capturing the reasoning behind decisions prevents knowledge loss and provides context for future contributors.

Every major decision should include:

- Decision
- Reason
- Date
- Status

---

# Decision 001

Title

Documentation First

Status

Accepted

Reason

Engineering standards should be documented before automation or implementation begins.

This ensures consistency across projects and provides clear guidance for both developers and AI assistants.

---

# Decision 002

Title

Adopt GitHub Flow

Status

Accepted

Reason

GitHub Flow is simple, scalable, and well suited to solo developers and small teams.

---

# Decision 003

Title

AI-Agnostic Platform

Status

Accepted

Reason

WDP should not depend on a single AI provider.

Engineering standards belong to WDP, while AI-specific behaviour belongs to individual AI profiles.

---

# Decision 004

Title

Separate Patterns from Shared Code

Status

Accepted

Reason

Patterns represent reusable engineering knowledge.

Shared contains reusable code.

These concepts evolve independently and should remain separate.

---

# Decision 005

Title

EngineeringAssistant.md

Status

Accepted

Reason

A universal engineering profile allows multiple AI assistants to inherit the same engineering standards while maintaining their own behaviours.

---

# Decision 006

Title

Use Markdown as the Source of Truth

Status

Accepted

Reason

Markdown is portable, version-controlled, AI-friendly, and easily searchable.

Documentation should remain independent of any specific tooling.

---

# Proposed Decision 007

Title

Milestone Branches

Status

Experimental

Reason

Milestone branches may provide a useful way to group related feature work around major project objectives.

Further real-world validation is required before adoption.

---

# Proposed Decision 008

Title

WDP CLI

Status

Planned

Reason

A CLI should automate project creation, AI configuration, documentation generation, Git initialization, and engineering standards.

---

# Engineering Principle

Good decisions are documented.

Great decisions include the reasoning behind them.