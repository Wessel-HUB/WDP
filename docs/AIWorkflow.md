# Wessel Developer Platform (WDP)

# AI Workflow

## Purpose

This document defines the standard workflow for collaborating with AI assistants during software development.

Within WDP, AI is treated as an engineering partner that accelerates development while the human developer remains responsible for architecture, design decisions, and final approval.

AI assists with implementation.

Humans own the product.

---

# Core Philosophy

The purpose of AI within WDP is not to replace engineering.

Its purpose is to eliminate repetitive work, improve consistency, accelerate development, and help capture engineering knowledge.

Every AI-generated solution should improve both the current project and the WDP platform itself.

---

# Roles and Responsibilities

## Human Responsibilities

The human developer is responsible for:

- Understanding the business problem
- Defining requirements
- Making architectural decisions
- Approving implementation plans
- Reviewing generated code
- Making final engineering decisions
- Approving merges into the main branch

The human is always accountable for production software.

---

## AI Responsibilities

The AI assistant is responsible for:

- Explaining concepts
- Producing implementation plans
- Generating code
- Refactoring existing code
- Writing documentation
- Suggesting improvements
- Identifying potential issues
- Updating project documentation
- Following WDP standards

AI should always work within the engineering principles defined by WDP.

---

# Standard Development Workflow

```
Business Idea
        │
        ▼
Define Requirements
        │
        ▼
Review Requirements
        │
        ▼
AI Creates Implementation Plan
        │
        ▼
Human Reviews Plan
        │
        ▼
Create Feature Branch
        │
        ▼
AI Implements Feature
        │
        ▼
Human Reviews Code
        │
        ▼
AI Updates Documentation
        │
        ▼
Commit Changes
        │
        ▼
Push Branch
        │
        ▼
Pull Request
        │
        ▼
Review
        │
        ▼
Merge
```

---

# Planning Phase

Before code is generated, AI should:

- Clarify unclear requirements
- Identify assumptions
- Suggest architecture
- Identify risks
- Break work into milestones
- Produce an implementation plan

Implementation should only begin after the plan is approved.

---

# Implementation Phase

During development, AI should:

- Follow WDP naming conventions
- Follow coding standards
- Reuse existing patterns where possible
- Avoid unnecessary complexity
- Keep changes focused
- Explain significant design decisions

---

# Documentation Phase

Documentation is part of the implementation.

AI should update documentation whenever changes affect:

- Architecture
- APIs
- Database schema
- Configuration
- Deployment
- User workflows
- Engineering decisions

Documentation should evolve with the code.

---

# Pre-Commit Checklist

Before creating a commit, AI should verify:

- Code compiles successfully
- Naming conventions are followed
- Coding standards are followed
- Documentation has been updated
- No debug code remains
- No temporary files are included
- No secrets are committed
- The feature is complete for its intended scope

---

# Pull Request Checklist

Before opening a Pull Request, AI should confirm:

- The feature branch is up to date
- The feature has been tested
- Documentation reflects the implementation
- Changes remain focused on a single objective
- Commit history is clean

---

# Continuous Improvement

After completing a feature, AI should ask:

"What can be contributed back to WDP?"

Examples include:

- New reusable patterns
- Improved templates
- Better documentation
- Shared libraries
- New automation
- Engineering lessons learned

Every completed project should improve the platform.

---

# AI Collaboration Principles

AI should:

- Ask questions when requirements are unclear.
- Explain recommendations and trade-offs.
- Prefer maintainable solutions over clever ones.
- Reuse existing WDP patterns before creating new ones.
- Highlight risks and assumptions.
- Avoid making architectural decisions without approval.

The human developer remains responsible for final decisions.

---

# Engineering Memory

One of WDP's core objectives is to preserve engineering knowledge.

Every project should contribute reusable knowledge back into the platform.

Lessons learned should become:

- Documentation
- Patterns
- Templates
- Standards
- Automation

Knowledge should compound over time.

---

# WDP AI Philosophy

AI is not a replacement for engineering.

AI is a force multiplier.

The goal is not to write software faster.

The goal is to build better software through consistent collaboration between human expertise and AI assistance.