# AI Workspace State

> Last Updated: 2026-07-31
> Version: 2.0

---

# Current Status

Current Phase

Phase 3 — Prompt Library

Status

Ready to Start

---

# Current Objective

Build a reusable Prompt Library for AI-assisted software engineering.

The prompt library should be modular, reusable, and designed for future expansion.

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

# Git Configuration

Configured

- core.pager=delta
- interactive.diffFilter=delta --color-only
- delta.navigate=true
- delta.side-by-side=true
- delta.line-numbers=true

---

# RTK

Status

Installed

Verified

- rtk git status
- rtk git diff
- rtk gain

Global Copilot Hook

Enabled

---

# Workspace Structure

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
├── ROADMAP.md
└── WORKSPACE_STATE.md
```

---

# Completed

## Phase 1 — Foundation

Completed

- GitHub CLI
- GitHub Copilot CLI
- RTK
- CLI development tools
- Git configuration
- Delta configuration

---

## Phase 2 — AI Workflow Optimization

Completed

- Personal AI Development Standards
- Advanced Global Copilot Instructions
- Repository Copilot Instructions Template
- AI Engineering Workflow
- AI Prompting Guide
- AI Search Strategy
- AI Tool Selection Guide
- RTK Workflow Guide

---

# Current Focus

Current work

Design and build the Prompt Library.

Current priorities

- Create reusable prompts.
- Keep prompts modular.
- Reduce AI token usage.
- Improve prompt consistency.
- Standardize engineering workflows.

---

# Next Tasks

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

- TypeScript
- JavaScript

### Technologies

- React
- React Native

---

# Current Decisions

Current priorities

- Prompt Library
- Workflow consistency
- Reusable prompts
- Token-efficient AI collaboration

Current non-priorities

- MCP
- Agent Skills
- Graphify
- Local AI models
- AI automation

These topics will be revisited in later roadmap phases.

---

# AI Instructions

When continuing this workspace:

- Continue from the current phase.
- Assume Phase 1 and Phase 2 are complete.
- Do not repeat completed work.
- Build on the existing workspace.
- Prefer updating existing documentation.
- Maintain a single source of truth.
- Keep recommendations technology-agnostic whenever possible.
- Prefer reusable solutions over project-specific ones.
- Consider token efficiency before introducing additional tooling.

---

# Current Milestone

Prompt Library

Objective

Create a reusable library of engineering prompts that can later be extended with additional languages, technologies, frameworks, libraries, or AI capabilities without restructuring the workspace.

---

# End of Document