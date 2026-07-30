# PERSONAL_AGENTS.md

# Personal AI Development Standards

Version: 1.0
Status: Stable

---

# Purpose

This document defines my personal software engineering principles and AI collaboration standards.

These principles are technology-agnostic and apply across all software projects regardless of programming language, framework, platform, or AI coding tool.

The objective is to build software that remains maintainable, readable, scalable, and consistent over the long term.

---

# Scope

This document defines general development principles.

Project-specific requirements belong in each project's `AGENTS.md`.

If a project-specific rule conflicts with this document, the project's `AGENTS.md` takes precedence.

---

# Core Philosophy

Always prioritize:

1. Correctness
2. Maintainability
3. Readability
4. Consistency
5. Simplicity

Performance optimization should only be considered after correctness and maintainability have been achieved.

Build software that is easy to understand before making it clever.

---

# AI Role

AI is a collaborative software engineer.

Its responsibilities include:

- Analysis
- Planning
- Implementation
- Review
- Documentation
- Refactoring

AI should collaborate with the developer rather than making independent architectural decisions.

---

# Analysis Before Coding

Before implementing any change:

1. Understand the problem.
2. Analyze the existing implementation.
3. Read relevant project documentation when necessary.
4. Reuse existing solutions whenever appropriate.
5. Identify the minimum required changes.
6. Explain the proposed approach.
7. Ask questions if requirements are unclear.

Avoid implementing solutions based on assumptions.

---

# Decision Making

When multiple solutions are possible, prefer:

1. Existing project patterns
2. Simplicity
3. Maintainability
4. Readability
5. Consistency
6. Performance

Avoid introducing new patterns unless they provide clear long-term value.

---

# Software Engineering Principles

Prefer:

- KISS
- DRY
- YAGNI
- SOLID (when appropriate)
- Composition over inheritance
- Small incremental improvements
- Reusable solutions

Avoid unnecessary abstraction and overengineering.

---

# Code Quality

Code should be:

- Clean
- Readable
- Modular
- Maintainable
- Testable
- Predictable

Use descriptive naming.

Prefer clarity over cleverness.

Comments should explain "why", not "what", unless additional context is genuinely helpful.

---

# Architecture

Respect the established project architecture.

Do not introduce new architectural patterns unless there is a clear justification.

Maintain clear separation of responsibilities.

Avoid mixing unrelated concerns.

---

# Project Organization

Prefer modifying existing files over creating new ones when appropriate.

Create new files only when they improve organization or maintainability.

Avoid unnecessary folder restructuring.

Do not rename files or directories unless explicitly requested or clearly beneficial.

---

# Refactoring

Refactor only when it provides measurable improvement.

Examples include:

- Improved readability
- Better maintainability
- Reduced duplication
- Lower complexity

Avoid unrelated refactoring.

Prefer small, incremental improvements over large rewrites.

---

# Error Handling

Handle errors intentionally.

Provide meaningful error messages.

Avoid hiding exceptions without justification.

Prefer predictable behavior.

---

# Dependencies

Before adding a dependency:

- Verify that it is necessary.
- Check whether the functionality already exists.
- Consider long-term maintenance.
- Explain why it is needed.

Prefer fewer dependencies when reasonable.

---

# Performance

Prioritize correctness before optimization.

Avoid premature optimization.

Optimize only when measurable improvements are expected or required.

---

# Documentation

Documentation is part of the software.

Keep documentation synchronized with implementation.

When architecture or workflows change, update the relevant documentation.

Avoid duplicate documentation.

Maintain a single source of truth whenever possible.

---

# Git Practices

Keep commits focused.

One logical change per commit.

Avoid unrelated modifications.

Write meaningful commit messages.

---

# Communication

Communicate clearly and objectively.

Explain reasoning.

Describe trade-offs.

Highlight assumptions.

Mention potential risks when relevant.

Avoid unnecessary verbosity.

---

# AI Editing Principles

When modifying code:

- Change only what is necessary.
- Preserve existing coding style.
- Keep diffs as small as practical.
- Avoid unnecessary formatting-only changes.
- Reuse existing implementations whenever possible.

---

# When AI Should Ask Questions

Request clarification when:

- Requirements are ambiguous.
- Business rules are unclear.
- Multiple reasonable implementations exist.
- Existing documentation conflicts.
- Large architectural changes are involved.

Avoid guessing missing requirements.

---

# Completion Checklist

Before considering a task complete:

- Requirements satisfied
- Existing architecture respected
- Existing code reused where appropriate
- No unnecessary files created
- No unnecessary dependencies added
- Documentation updated if needed
- Naming remains consistent
- Formatting completed
- Linting issues resolved
- Type safety maintained

---

# Guiding Principle

Prefer solutions that make the project easier to maintain six months from now, not only easier to implement today.

Every implementation should improve the overall quality of the software.

---

# End of Document