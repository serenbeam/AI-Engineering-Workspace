# AI Tool Selection Guide

Version: 1.0

Status: Stable

---

# Purpose

This document defines the recommended strategy for selecting development tools during AI-assisted software engineering.

The objective is to use the most appropriate tool for each task, reduce unnecessary context usage, improve productivity, and maintain a consistent development workflow.

These guidelines are technology-agnostic and apply regardless of programming language, framework, or AI coding assistant.

---

# Scope

These recommendations apply during:

- repository exploration
- feature implementation
- bug investigation
- code review
- documentation review
- configuration inspection
- Git operations

Repository-specific requirements may extend or override these recommendations where appropriate.

---

# Core Principles

Choose tools intentionally.

Prefer:

- specialised tools over general-purpose tools,
- one primary responsibility per tool,
- incremental information gathering,
- minimal context collection,
- repeatable workflows.

Avoid:

- using one tool for every task,
- unnecessary repository scanning,
- duplicated effort,
- collecting information that is not relevant to the current task.

---

# Supported Tools

KHWAMI currently includes the following tools.

| Tool | Primary Responsibility |
|------|-------------------------|
| Git | Version control |
| GitHub CLI | GitHub operations |
| fd | File discovery |
| rg | Content search |
| bat | File reading |
| jq | JSON inspection |
| delta | Git diff review |
| RTK | Terminal output enhancement |

This document should be updated whenever new core development tools become part of KHWAMI.

---

# Tool Selection Guide

Choose the most specialised tool for the current objective.

| Objective | Recommended Tool |
|-----------|------------------|
| Locate files | `fd` |
| Search implementation | `rg` |
| Read files | `bat` |
| Inspect JSON | `jq` |
| Review Git changes | `delta` |
| Handle long terminal output | `RTK` |
| Local version control | `Git` |
| GitHub repositories, issues, and pull requests | `GitHub CLI` |

Always prefer the narrowest tool capable of completing the task.

---

# Tool Responsibilities

## Git

### Primary Responsibility

Version control.

### Typical Tasks

- commits
- branches
- merges
- history
- staging

---

## GitHub CLI

### Primary Responsibility

GitHub platform operations.

### Typical Tasks

- repositories
- pull requests
- issues
- releases
- authentication

Prefer GitHub CLI over browser-based workflows whenever practical.

---

## fd

### Primary Responsibility

Fast file discovery.

### Typical Tasks

- locate source files
- find configuration files
- locate documentation
- discover project structure

Prefer locating files before reading them.

---

## rg

### Primary Responsibility

Search implementation.

### Typical Tasks

- functions
- classes
- interfaces
- constants
- API endpoints
- feature identifiers
- configuration keys

Search before opening files.

---

## bat

### Primary Responsibility

Read files.

### Typical Tasks

- source code
- documentation
- configuration
- logs

Read only files relevant to the current task.

---

## jq

### Primary Responsibility

Inspect structured JSON.

### Typical Tasks

- package.json
- configuration files
- API responses
- lock files

Prefer structured inspection over manual scanning.

---

## delta

### Primary Responsibility

Review Git changes.

### Typical Tasks

- diffs
- staged changes
- recent modifications
- change review

Review changes before modifying implementation whenever practical.

---

## RTK

### Primary Responsibility

Improve readability of large terminal output.

### Typical Tasks

- long search results
- repository analysis
- large Git output
- extensive terminal logs

Use RTK when terminal output becomes difficult to navigate.

---

# Tool Selection Workflow

Determine the objective.

↓

Identify the required information.

↓

Select the most specialised tool.

↓

Collect only the necessary context.

↓

Proceed with analysis or implementation.

## Tool Evaluation

Evaluate an additional AI or development tool only when a confirmed workflow
gap remains after applying the existing guidance and tools. Record the
objective, evidence of the gap, compatibility, maintenance and security cost,
expected workflow benefit, and context impact. Adopt the tool only when its
measurable benefit outweighs those costs.

Record a material adoption, rejection, or replacement decision in
`docs/decisions.md`. Do not install or introduce a tool solely to evaluate it.

---

# Decision Tree

When selecting a tool, ask the following questions.

Need to locate a file?

↓

Use `fd`

---

Need to find implementation?

↓

Use `rg`

---

Need to read a file?

↓

Use `bat`

---

Need to inspect JSON?

↓

Use `jq`

---

Need to review Git changes?

↓

Use `delta`

---

Need to manage Git history?

↓

Use `Git`

---

Need GitHub operations?

↓

Use `GitHub CLI`

---

Need to navigate large terminal output?

↓

Use `RTK`

---

# Relationship with Search Strategy

This document defines **which tool** should be used.

The companion document **search-strategy.md** defines **how repository exploration should be performed**.

Tool selection answers:

> Which tool is appropriate?

Search strategy answers:

> What information should be gathered, and in what order?

These documents complement each other and should not duplicate responsibilities.

---

# Common Mistakes

Avoid:

- using one tool for unrelated tasks,
- opening many files before searching,
- manually browsing large repositories,
- manually inspecting large JSON documents,
- skipping Git review before implementation,
- gathering unnecessary context.

---

# Relationship with Other KHWAMI Documents

| Document | Primary Responsibility |
|----------|------------------------|
| `agents/PERSONAL_AGENTS.md` | Engineering principles |
| `copilot_instructions.md` | AI behaviour |
| workflow.md | Engineering workflows |
| prompting-guide.md | Communication with AI |
| search-strategy.md | Repository exploration strategy |
| tool-selection.md | Development tool selection |
| rtk-workflow.md | RTK workflow and best practices |
| Repository Copilot Instructions | Repository-specific knowledge |
| AGENTS.md | Project-specific rules |

Each document has a distinct responsibility and should avoid duplicating information.

---

# Future Expansion

As KHWAMI evolves, additional tools may be incorporated into this guide.

Examples include:

- repository graph analysis tools,
- reusable AI skill frameworks,
- static analysis tools,
- code intelligence platforms.

New tools should only be added after they become part of the active development workflow.

---

# Guiding Principle

Use the right tool for the right task.

Selecting specialised tools improves efficiency, reduces unnecessary context usage, and enables more focused software engineering.

---

# End of Document