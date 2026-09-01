# RTK Workflow Guide

Version: 1.0

Status: Stable

---

# Purpose

This document defines the recommended workflow for using RTK during AI-assisted software engineering.

The objective is to improve repository exploration, terminal readability, and developer productivity while reducing unnecessary context and repetitive terminal interactions.

These recommendations are technology-agnostic and apply regardless of programming language or framework.

---

# Scope

These guidelines apply when using RTK during:

- repository exploration
- code review
- feature implementation
- bug investigation
- Git review
- terminal-based development

Repository-specific workflows may extend these recommendations.

---

# Core Principles

Use RTK to improve navigation and readability rather than replace existing development tools.

Prefer:

- incremental exploration,
- focused analysis,
- structured terminal output,
- efficient repository navigation.

Avoid using RTK when standard terminal commands already provide sufficient information.

---

# RTK Responsibilities

RTK is intended to improve the developer experience when working with large or complex terminal output.

Typical responsibilities include:

- repository exploration,
- Git inspection,
- large search results,
- command output navigation,
- context reduction.

RTK complements existing CLI tools rather than replacing them.

---

# Recommended Workflow

Use RTK as part of the normal engineering workflow.

Developer Request

↓

Understand the objective

↓

Determine the required information

↓

Select the appropriate tool

↓

Use RTK when output becomes large or difficult to navigate

↓

Analyse the relevant information

↓

Implement or review changes

---

# When to Use RTK

RTK is most beneficial when:

- analysing unfamiliar repositories,
- reviewing large Git diffs,
- navigating extensive search results,
- working with verbose terminal output,
- exploring large codebases,
- reducing repetitive terminal interaction.

Use RTK only when it improves clarity or efficiency.

Use direct commands for focused output. Switch to RTK when output exceeds what
can be reviewed in one focused pass, requires repeated narrowing, or would
otherwise require copying excessive terminal content into AI context.

---

# When RTK Is Not Required

RTK is generally unnecessary for:

- reading a single file,
- locating a known file,
- simple Git commands,
- inspecting small JSON files,
- reviewing short terminal output,
- straightforward repository navigation.

Prefer simpler tools when they adequately solve the problem.

---

# Integration with Other Tools

RTK works alongside the existing development tools.

| Tool | Primary Responsibility |
|------|-------------------------|
| Git | Version control |
| GitHub CLI | GitHub operations |
| fd | File discovery |
| rg | Content search |
| bat | File reading |
| jq | JSON inspection |
| delta | Git diff review |
| RTK | Improve navigation of large terminal output |

Each tool should continue serving its primary responsibility.

---

# Recommended Decision Process

Before using RTK, consider:

1. Is the terminal output difficult to navigate?
2. Will RTK improve readability?
3. Can the task be completed efficiently without RTK?
4. Will RTK reduce unnecessary context gathering?

Use RTK only when it provides a measurable improvement to the workflow.

---

# Typical Engineering Scenarios

## Repository Exploration

Objective

Understand an unfamiliar project.

Recommended Workflow

- Read project documentation.
- Locate relevant files.
- Explore implementation.
- Use RTK if repository exploration becomes extensive.

---

## Bug Investigation

Objective

Identify the root cause of an issue.

Recommended Workflow

- Search for relevant implementation.
- Review related changes.
- Use RTK when analysing large search results or extensive terminal output.

---

## Code Review

Objective

Review recent changes.

Recommended Workflow

- Inspect Git changes.
- Review affected files.
- Use RTK if the review spans many files or large diffs.

---

## Feature Implementation

Objective

Implement a new feature.

Recommended Workflow

- Understand requirements.
- Explore relevant modules.
- Analyse existing implementation.
- Use RTK only if repository exploration becomes complex.

---

# Relationship with Other KHWAMI Documents

This document complements the other KHWAMI documents.

| Document | Primary Responsibility |
|----------|------------------------|
| `agents/PERSONAL_AGENTS.md` | Engineering principles |
| `copilot_instructions.md` | AI behaviour |
| workflow.md | Standard engineering workflow |
| prompting-guide.md | Communication with AI |
| search-strategy.md | Repository exploration strategy |
| tool-selection.md | Tool selection guidance |
| rtk-workflow.md | RTK usage within the development workflow |
| Repository Copilot Instructions | Repository-specific knowledge |
| AGENTS.md | Project-specific rules and business context |

Each document has a distinct responsibility and should avoid duplicating information.

---

# Common Mistakes

Avoid:

- using RTK for every terminal command,
- replacing specialised tools with RTK,
- exploring unrelated parts of the repository,
- collecting unnecessary context,
- assuming RTK replaces engineering judgement.

RTK enhances workflows—it does not replace sound engineering practices.

---

# Future Expansion

As RTK evolves, this document may include additional workflow recommendations.

Updates should focus on workflow improvements rather than implementation details or command syntax.

---

# Guiding Principle

Use RTK when it improves clarity, navigation, or productivity.

Prefer simple workflows for simple tasks and reserve RTK for situations where it provides meaningful value.

---

# End of Document