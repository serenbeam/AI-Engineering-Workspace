# Repository Copilot Instructions

Version: 1.0

Status: Template

---

# Repository Profile

| Item | Value |
|------|-------|
| Repository Name | `<Repository Name>` |
| Repository Type | `<Mobile Application / Web Application / Backend Service / Library / CLI Tool / Monorepo>` |
| Primary Language | `<Programming Language>` |
| Framework | `<Framework>` |
| Architecture | `<Architecture Pattern>` |
| Development Stage | `<Prototype / MVP / Active Development / Maintenance / Legacy>` |
| Complexity | `<Small / Medium / Large / Enterprise>` |
| Preferred Change Scope | `<Localized / Feature-Level / Cross-Module>` |
| Testing Strategy | `<Unit / Integration / End-to-End / Manual Verification>` |
| Deployment Target | `<Android / iOS / Web / Server / Desktop / Multiple Platforms>` |

---

# Purpose

Describe the purpose of this repository.

Summarise:

- the project's objective,
- primary responsibilities,
- intended users,
- expected outcomes.

Keep this section concise.

---

# Project Overview

Provide a high-level overview of the repository.

Include:

- what the project does,
- major features,
- major modules,
- overall development approach.

Avoid implementation details.

---

# Technology Stack

List the primary technologies used by this repository.

Examples include:

- programming language
- framework
- runtime
- package manager
- database
- testing framework
- build tools

Only document technologies that are actively used.

---

# Repository Structure

Describe the major directories and their responsibilities.

Focus on responsibilities rather than listing every folder.

Example:

- application
- domain
- infrastructure
- shared
- documentation
- scripts

Avoid documenting every file.

---

# Architecture Overview

Describe the project's architecture.

Examples include:

- Layered Architecture
- Feature-Based Architecture
- Clean Architecture
- Hexagonal Architecture
- Modular Monolith
- MVC

Explain how responsibilities are separated throughout the project.

---

# Coding Conventions

Document repository-specific coding conventions.

Examples:

- naming conventions
- formatting rules
- import organisation
- dependency direction
- configuration management
- error handling

Avoid repeating language-specific best practices unless they differ from common conventions.

---

# Dependency Guidelines

Document dependency expectations.

Examples:

- preferred internal utilities,
- approved third-party libraries,
- restricted dependencies,
- dependency direction,
- reuse expectations.

Prefer existing project solutions before introducing new dependencies.

---

# Development Workflow

Describe the preferred development workflow for this repository.

Typical workflow:

1. Understand
2. Analyse
3. Implement
4. Verify
5. Document (when required)

Replace this workflow if the repository follows a different process.

---

# Testing Expectations

Describe the project's testing strategy.

Examples:

- Unit Testing
- Integration Testing
- End-to-End Testing
- Manual Verification

Explain expectations rather than implementation details.

---

# Documentation

Identify the project's primary documentation.

Examples:

- README
- Architecture documentation
- Feature documentation
- Decision records
- API documentation

Avoid duplicate documentation.

Maintain a single source of truth whenever possible.

---

# AI Expectations

When working in this repository, AI should:

- understand the existing implementation before making changes,
- preserve the established architecture,
- follow existing project conventions,
- reuse existing implementations whenever practical,
- minimise unnecessary changes,
- update documentation when implementation changes require it.

Repository-specific instructions take precedence over generic recommendations.

---

# Repository-Specific Rules

Document rules unique to this repository.

Examples:

- business constraints,
- security requirements,
- compliance requirements,
- performance requirements,
- deployment requirements,
- external integrations.

Remove this section if no repository-specific rules are required.

---

# Customisation Notes

This file is intended to be customised for each repository.

When creating a new repository:

- replace all placeholder values,
- remove sections that do not apply,
- add repository-specific guidance where necessary,
- avoid unnecessary duplication with other documentation.

---

# Guiding Principle

The purpose of this document is to help AI understand the repository quickly while preserving consistency with the existing codebase.

Repository knowledge should be centralised here rather than duplicated across multiple documents.

---

# End of Document