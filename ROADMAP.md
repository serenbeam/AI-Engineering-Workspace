# AI Engineering Workspace Roadmap

> Last Updated: 2026-08-19
> Version: 3.1
> Status: Phase 4 complete

---

# Purpose

This roadmap is the single source of truth for the AI Engineering Workspace.

Its objectives are to:

- Track workspace progress across development phases.
- Standardize AI-assisted software engineering practices.
- Prevent repeating completed work.
- Organize AI-related documentation and workflows.
- Build a maintainable, reusable, and scalable AI engineering environment.

---

# Scope

This roadmap applies to my personal AI Engineering Workspace.

Its purpose is to standardize AI-assisted software engineering workflows, development standards, prompt engineering, repository guidance, and reusable engineering assets across projects.

The roadmap focuses on:

- AI engineering workflow
- Development standards
- AI instructions
- Prompt library
- Repository intelligence
- Development tooling
- Workspace evolution

---

# Current Environment

Operating System

- Windows 11

Editor

- Visual Studio Code

Terminal

- PowerShell

Primary AI Tools

- GitHub Copilot
- GitHub Copilot CLI
- Cursor
- ChatGPT
- RTK

---

# Installed CLI Tools

| Tool | Status |
|------|--------|
| Git | ✅ |
| GitHub CLI | ✅ |
| GitHub Copilot CLI | ✅ |
| RTK | ✅ |
| rg | ✅ |
| fd | ✅ |
| jq | ✅ |
| bat | ✅ |
| delta | ✅ |

---

# Workspace Architecture

```text
AI-ENGINEERING-WORKSPACE
│
├── agents/
│   └── PERSONAL_AGENTS.md
│
├── instructions/
│   ├── global/
│   │   ├── copilot-instructions.md
│   │   ├── workflow.md
│   │   ├── prompting-guide.md
│   │   ├── search-strategy.md
│   │   ├── tool-selection.md
│   │   └── rtk-workflow.md
│   │
│   └── repository/
│       └── copilot-instructions-template.md
│
├── prompts/
│   ├── README.md
│   ├── TEMPLATE.md
│   │
│   ├── general-engineering/
│   │   ├── analysis.md
│   │   ├── planning.md
│   │   ├── bug-investigation.md
│   │   ├── code-review.md
│   │   ├── refactoring.md
│   │   ├── feature-implementation.md
│   │   ├── documentation.md
│   │   ├── architecture-review.md
│   │   ├── performance-review.md
│   │   └── testing.md
│   │
│   ├── programming-languages/
│   │   ├── javascript.md
│   │   └── typescript.md
│   │
│   └── technologies/
│       ├── react.md
│       ├── react-native.md
│       ├── nodejs.md
│       └── express.md
│
├── ROADMAP.md
└── WORKSPACE_STATE.md
```

---

# Completed Phases

## Phase 1 — Foundation

Status

Completed

Completed Items

- GitHub CLI
- GitHub Copilot CLI
- RTK
- CLI development tools
- Git configuration
- Delta configuration

---

## Phase 2 — AI Workflow Optimization

Status

Completed

Completed Items

- Personal AI Development Standards
- Advanced Global Copilot Instructions
- Repository Copilot Instructions Template
- AI Engineering Workflow
- AI Prompting Guide
- AI Search Strategy
- AI Tool Selection Guide
- RTK Workflow Guide

Do not repeat completed phases.

---

## Phase 3 — Prompt Library

Status

Completed

Objective

Create a reusable Prompt Library that standardizes AI-assisted software engineering tasks.

Completed Items

### Core

- Prompt Library README
- Prompt Template

### General Engineering

- Analysis
- Planning
- Bug Investigation
- Code Review
- Refactoring
- Feature Implementation
- Documentation
- Architecture Review
- Performance Review
- Testing

### Programming Languages

- JavaScript
- TypeScript

### Technologies

- React
- React Native
- Node.js
- Express

Deliverables

```text
prompts/
```

Prompt Library v1.0 is complete.

Do not repeat completed phases.

---

# Latest Completed Phase

## Phase 4 — Repository Intelligence

Status

Completed

Objective

Help AI understand repositories faster and more accurately by providing reusable repository intelligence documents that reduce unnecessary repository scanning, improve engineering context, and standardize project documentation.

---

# Roadmap

## Phase 4 — Repository Intelligence

Goal

Help AI understand repositories faster and more accurately by providing reusable repository intelligence documents that reduce unnecessary repository scanning, improve engineering context, and standardize project documentation.

### Core Tasks

- [x] repository-overview.md
- [x] architecture.md
- [x] feature-map.md
- [x] decisions.md

### Optional Extensions

Create only when they provide clear value for the repository.

- dependency-map.md
- glossary.md
- known-issues.md

Deliverables

```text
docs/
```

---

## Phase 5 — AI Workspace Optimization

Goal

Continuously improve the AI Engineering Workspace.

Tasks

- [ ] Improve AI instructions
- [ ] Optimize repository guidance
- [ ] Reduce unnecessary AI context
- [ ] Improve repository understanding
- [ ] Improve token efficiency
- [ ] Standardize documentation maintenance
- [ ] Evaluate additional AI tooling when beneficial

---

## Phase 6 — Advanced AI Engineering

Goal

Expand the workspace with advanced AI capabilities when they provide clear value.

Potential Topics

- Agent Skills
- Graphify
- MCP
- AI automation
- Prompt engineering
- Repository templates
- Knowledge graph
- Local AI workflow

This phase is intentionally deferred until earlier phases are complete.

---

# Milestones

| Milestone | Status |
| ------------------------- | ------ |
| Workspace Foundation | ✅ |
| AI Workflow Optimization | ✅ |
| Prompt Library | ✅ |
| Repository Intelligence | ✅ |
| AI Workspace Optimization | ⬜ |
| Advanced AI Engineering | ⬜ |

---

# AI Rules

When continuing this roadmap:

- Never repeat completed phases.
- Continue from the current phase.
- Prefer improving workflows before introducing new tools.
- Avoid unnecessary dependencies.
- Keep documentation synchronized.
- Maintain a single source of truth.
- Prefer reusable assets over one-off solutions.
- Design documentation to be technology-agnostic whenever possible.
- Consider token efficiency in every recommendation.
- Prefer `rg` for repository search.
- Prefer `fd` for file discovery.
- Prefer `bat` for reading files.
- Prefer `jq` for JSON inspection.
- Prefer `delta` for Git review.
- Use RTK when working with large repositories or lengthy terminal output.

---

# Progress

```text
Phase 1

██████████ 100%

Phase 2

██████████ 100%

Phase 3

██████████ 100%

Phase 4

██████████ 100%

Phase 5

□□□□□□□□□□ 0%

Phase 6

□□□□□□□□□□ 0%
```

---

# Next Chat

Phase status

**Phase 4 — Repository Intelligence is complete.**

Assume:

- Phase 1 is complete.
- Phase 2 is complete.
- Phase 3 is complete.
- Phase 4 is complete.
- All workflow documentation already exists.

Current state

The Repository Intelligence v1.0 core documents are complete. Do not begin Phase 5 until it is separately scoped.

Do not restart the roadmap.

Continue building on the existing AI Engineering Workspace.

---

# End of Document