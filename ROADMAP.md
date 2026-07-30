# AI Development Workspace Roadmap (Personal Laptop)

> Last Updated: 2026-07-29
> Status: Phase 1 Completed
> Owner: Laili Kumala

---

# Purpose

This roadmap is the single source of truth for my personal AI development workspace.

It is intended to:

- Keep progress between ChatGPT conversations.
- Prevent repeating completed setup.
- Track completed and upcoming phases.
- Standardize AI tooling and workflow.
- Build an efficient AI-assisted software engineering environment.

---

# Scope

This roadmap ONLY applies to my PERSONAL laptop.

DO NOT discuss or include:

- GitHub Copilot Enterprise
- Office laptop configuration
- Company-specific workflow

Current AI stack:

- GitHub Copilot Individual
- GitHub Copilot CLI
- RTK
- VS Code
- Cursor Free
- ChatGPT

---

# Current Environment

Operating System

- Windows 11

Editor

- VS Code

AI Tools

- GitHub Copilot Individual
- GitHub Copilot CLI
- Cursor Free
- ChatGPT

Terminal

- PowerShell

Git

Installed

GitHub CLI

Installed

RTK

Installed

---

# Installed CLI Tools

| Tool | Status |
|---------|--------|
| rg | ✅ |
| fd | ✅ |
| jq | ✅ |
| bat | ✅ |
| delta | ✅ |

---

# Git Configuration

Configured

core.pager=delta

interactive.diffFilter=delta --color-only

delta.navigate=true

delta.side-by-side=true

delta.line-numbers=true

---

# RTK

Installed

Global Copilot integration enabled.

Current configuration

- Copilot Hook
- Global Instructions
- RTK Hook
- PATH configured

Already tested

- rtk git status
- rtk git diff
- rtk gain

RTK is working correctly.

---

# Completed Phases

## Phase 1

Foundation

Status

Completed

Completed Items

- GitHub CLI
- GitHub Copilot CLI
- RTK
- Global Hook
- Copilot Instructions
- rg
- fd
- jq
- bat
- delta
- Git Delta configuration

DO NOT repeat Phase 1.

---

# Current Phase

Phase 2

AI Workflow Optimization

Status

Not Started

---

# Roadmap

---

## Phase 2

AI Workflow

Goal

Improve AI behaviour rather than adding more tools.

Tasks

- [ ] Create advanced global Copilot instructions.
- [ ] Create repository-level Copilot instructions.
- [ ] Optimize RTK usage.
- [ ] Reduce unnecessary repository scanning.
- [ ] Improve search strategy.
- [ ] Standardize AI workflow.

Deliverables

.github/

copilot-instructions.md

.ai/

workflow.md

---

## Phase 3

Prompt Library

Goal

Create reusable prompts.

Tasks

- [ ] Bug Analysis
- [ ] Refactor
- [ ] Code Review
- [ ] React Native
- [ ] TypeScript
- [ ] Testing
- [ ] Architecture Review
- [ ] Performance Review

Deliverables

.ai/

prompts/

---

## Phase 4

AI Documentation

Goal

Help AI understand repositories quickly.

Tasks

- [ ] architecture.md
- [ ] feature-map.md
- [ ] decisions.md
- [ ] glossary.md
- [ ] known-issues.md

Deliverables

.ai/docs/

---

## Phase 5

Cursor Free Optimization

Goal

Optimize Cursor Free only.

Tasks

- [ ] Improve agent.md
- [ ] Reduce context usage.
- [ ] Improve project understanding.
- [ ] Standardize prompt style.

NOTE

Cursor Free only.

Do NOT discuss Cursor Pro unless requested.

---

## Phase 6

Advanced AI Workspace

Goal

Build an advanced AI-assisted engineering environment.

Potential topics

- MCP
- AI automation
- Prompt engineering
- Local workflow
- Repository templates

Not a priority yet.

---

# AI Rules

When continuing this roadmap:

Never repeat completed phases.

Always continue from the current phase.

Avoid installing unnecessary tools.

Prefer workflow optimization over adding software.

Recommend only practical improvements.

Keep recommendations suitable for React Native and TypeScript development.

Always consider token efficiency.

Prefer rg over recursive file scanning.

Prefer fd over slow file searching.

Use bat when reading files in terminal.

Use jq for JSON inspection.

Use delta for git review.

Use RTK whenever long terminal output is expected.

---

# Progress

Phase 1

██████████ 100%

Phase 2

□□□□□□□□□□ 0%

Phase 3

□□□□□□□□□□ 0%

Phase 4

□□□□□□□□□□ 0%

Phase 5

□□□□□□□□□□ 0%

Phase 6

□□□□□□□□□□ 0%

---

# Next Chat

Continue from:

Phase 2

Task:

Create advanced global GitHub Copilot instructions.

Do NOT restart the roadmap.

Do NOT repeat completed setup.

Assume all Phase 1 tasks are already completed.