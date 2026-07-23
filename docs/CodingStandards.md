# Wessel Development Platform (WDP)

# Coding Standards

## Purpose

This document defines the coding standards used across all WDP projects.

The objective is to produce software that is:

- Readable
- Maintainable
- Consistent
- Testable
- Reusable
- Easy for humans and AI to understand

Consistency is valued over personal preference.

---

# Core Principles

Code should be:

- Simple
- Explicit
- Predictable
- Modular
- Self-documenting

Code is read far more often than it is written.

Optimize for readability first.

---

# General Rules

- Write code for humans first.
- Prefer clarity over cleverness.
- Keep methods focused on a single responsibility.
- Avoid duplicate logic.
- Prefer composition over inheritance.
- Avoid premature optimization.
- Always leave the codebase cleaner than you found it.

---

# SOLID Principles

WDP follows the SOLID principles.

- Single Responsibility Principle
- Open/Closed Principle
- Liskov Substitution Principle
- Interface Segregation Principle
- Dependency Inversion Principle

These principles guide architectural decisions rather than being followed dogmatically.

---

# Class Design

Classes should have one clear responsibility.

Avoid "God Classes" that perform multiple unrelated tasks.

Prefer dependency injection over creating dependencies directly.

---

# Method Design

Methods should:

- Perform one task.
- Have descriptive names.
- Avoid excessive nesting.
- Return early where appropriate.
- Minimize side effects.

If a method requires extensive comments to explain what it does, consider refactoring it.

---

# Method Length

There is no fixed line limit.

However:

- If a method no longer fits comfortably on one screen, consider extracting smaller methods.
- If a method performs multiple logical operations, split it.

Methods should be easy to understand at a glance.

---

# Comments

Prefer self-explanatory code over comments.

Use comments to explain:

- Why something is done.
- Business rules.
- Non-obvious decisions.

Avoid comments that simply repeat the code.

Bad:

// Increment i

i++;

Good:

// Legacy payment gateway requires a one-second delay before retrying.
Thread.Sleep(1000);

---

# Error Handling

Handle expected exceptions gracefully.

Do not silently swallow exceptions.

Always log unexpected errors.

Provide meaningful error messages.

---

# Logging

Log:

- Application startup
- Authentication events
- Critical business operations
- Errors
- Warnings

Do not log:

- Passwords
- JWT tokens
- Connection strings
- Personal information unless required

---

# Dependency Injection

Dependencies should be injected whenever practical.

Avoid creating dependencies directly inside classes.

Good:

private readonly IUserRepository _userRepository;

Avoid:

new UserRepository();

---

# Repository Pattern

Business logic should not directly communicate with the database.

Use repositories or data access abstractions.

---

# Configuration

Configuration belongs in configuration files.

Avoid hard-coded values.

Examples:

- Connection strings
- API URLs
- Feature flags
- Timeout values

---

# Magic Numbers

Avoid unexplained numeric values.

Bad:

if (attempts > 5)

Good:

if (attempts > MaxLoginAttempts)

---

# Async Programming

Use asynchronous programming when appropriate.

Avoid blocking operations on UI threads.

Do not use async without a clear benefit.

---

# Database Access

Prefer parameterized queries.

Use stored procedures where appropriate.

Follow WDP SQL naming conventions.

Never concatenate SQL strings using user input.

---

# Security

Never:

- Commit secrets
- Store passwords in plain text
- Disable authentication for convenience
- Trust client-side validation

Always validate input on the server.

---

# Testing

New functionality should be testable.

Where practical:

- Unit tests
- Integration tests
- Manual validation

Testing requirements may vary depending on the project.

---

# Refactoring

Refactor continuously.

Do not postpone obvious improvements indefinitely.

Large refactors should be isolated into dedicated branches.

---

# AI Collaboration

AI-generated code should:

- Follow all WDP standards.
- Match the existing coding style.
- Avoid unnecessary dependencies.
- Explain significant architectural decisions.
- Prefer reusable solutions over one-off implementations.

Generated code should be reviewed before being committed.

---

# Engineering Principle

Clean code is not code with fewer lines.

Clean code is code that is easier to understand tomorrow than it was yesterday.

# Pragmatism

WDP values practical engineering over theoretical perfection.

Choose the simplest solution that:

- Solves the business problem.
- Can be maintained.
- Can be explained.
- Can evolve over time.

Avoid unnecessary complexity introduced solely because a design pattern or technology is fashionable.

Technology should serve the business—not the other way around.