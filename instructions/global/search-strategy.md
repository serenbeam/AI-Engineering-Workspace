# AI Search Strategy

Version: 1.0

Status: Stable

---

# Purpose

This document defines the recommended strategy for exploring repositories efficiently during AI-assisted software development.

The objective is to minimise unnecessary repository scanning, reduce context usage, improve response quality, and locate relevant information quickly.

These guidelines are technology-agnostic and apply regardless of programming language, framework, or AI coding assistant.

---

# Scope

These search strategies apply whenever understanding an existing codebase.

Examples include:

- feature implementation
- bug investigation
- code review
- refactoring
- repository exploration
- documentation review

Repository-specific documentation may override these recommendations when necessary.

---

# Search Principles

Always search with intention.

Prefer:

- targeted exploration
- incremental context gathering
- reading only what is necessary
- understanding before implementation

Avoid:

- scanning the entire repository
- reading unrelated files
- collecting unnecessary context
- repeating the same searches

---

# Search Decision Guide

Choose the appropriate strategy based on what information is already known.

| Situation | Recommended Strategy |
|-----------|----------------------|
| Exact file is known | Read the file directly |
| File name is partially known | Discover files |
| Implementation location is unknown | Search file contents |
| Understanding project structure | Read documentation first |
| Reviewing configuration | Inspect configuration files |
| Investigating JSON | Use structured inspection |
| Reviewing code changes | Review Git changes before source code |
| Large terminal output | Prefer RTK or paged output |

Always choose the narrowest search that provides sufficient context.

---

# Recommended Search Order

Prefer the following order whenever exploring a repository.

1. Project documentation
2. Repository structure
3. Relevant files
4. Related implementation
5. Dependencies
6. Configuration
7. Git history (when relevant)

Expand the search only when additional context is required.

---

# Documentation First

Before reading implementation, determine whether documentation already answers the question.

Examples include:

- README
- Architecture documentation
- Feature documentation
- Decision records
- API documentation

Documentation often provides sufficient context without reading implementation.

---

# File Discovery

Locate files before reading them.

Prefer searching by responsibility rather than scanning directories manually.

Examples:

- feature names
- module names
- service names
- configuration names

Avoid opening multiple unrelated files.

---

# Content Search

Search for implementation details rather than browsing manually.

Typical search targets include:

- function names
- interfaces
- classes
- configuration keys
- constants
- API endpoints
- feature identifiers

Review only the most relevant matches before expanding the search.

---

# Repository Exploration

Understand the repository progressively.

Recommended sequence:

1. Repository purpose
2. Project structure
3. Relevant modules
4. Related implementation
5. Supporting utilities

Avoid exploring unrelated modules.

---

# Configuration Search

Configuration often explains application behaviour.

Review configuration before assuming implementation details.

Examples include:

- environment configuration
- application settings
- build configuration
- dependency configuration

---

# JSON Inspection

Inspect structured data rather than reading raw JSON manually.

Typical examples:

- package metadata
- configuration files
- API responses
- lock files

Prefer structured inspection over manual scanning.

---

# Git Review

When analysing existing work, review recent changes before modifying implementation.

Focus on:

- current changes
- affected files
- recent commits
- modified behaviour

Understanding change history often provides valuable context.

---

# Large Output Handling

Large outputs should be reviewed incrementally.

Avoid processing large terminal output all at once.

Prefer tools that improve readability and navigation.

Examples include:

- paged output
- syntax highlighting
- structured formatting

---

# Context Optimisation

Context is valuable.

Gather only the information required for the current task.

Prefer:

- relevant files only
- nearby implementation
- related documentation

Avoid:

- repository-wide analysis
- unnecessary repeated searches
- duplicate context

Expand context only when evidence suggests it is required.

---

# Search Workflow

Follow this general workflow whenever exploring unfamiliar code.

Understand the objective

↓

Determine what information is already known

↓

Locate relevant documentation

↓

Locate relevant files

↓

Inspect implementation

↓

Expand search only when necessary

↓

Implement or analyse

---

# Search Tool Guidance

Choose tools based on the type of information required.

| Goal | Preferred Tool |
|------|----------------|
| Find files | `fd` |
| Search file contents | `rg` |
| Read files | `bat` |
| Inspect JSON | `jq` |
| Review Git changes | `delta` |
| Handle long terminal output | RTK |

Use each tool for its intended responsibility.

Avoid using one tool to perform every type of search.

---

# Common Mistakes

Avoid:

- searching the entire repository without a clear objective,
- opening many unrelated files,
- ignoring available documentation,
- repeatedly reading the same implementation,
- collecting more context than necessary,
- assuming behaviour without evidence.

---

# Relationship with Other AI Workspace Documents

This document complements the other documents in the AI Engineering Workspace.

| Document | Primary Responsibility |
|----------|------------------------|
| PERSONAL_AGENTS.md | Engineering principles |
| copilot-instructions.md | AI behaviour |
| workflow.md | Engineering workflows |
| prompting-guide.md | Communication with AI |
| search-strategy.md | Repository exploration strategy |
| Repository Copilot Instructions | Repository-specific knowledge |
| AGENTS.md | Project-specific rules |

Each document serves a distinct purpose and should avoid duplicating information.

---

# Guiding Principle

Search intentionally, gather only the necessary context, and expand exploration only when evidence indicates that additional information is required.

Efficient repository exploration leads to better engineering decisions while reducing unnecessary context usage.

---

# End of Document