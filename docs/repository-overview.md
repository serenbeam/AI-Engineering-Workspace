# Repository Overview

## Purpose

Provide a high-level index of this personal AI Engineering Workspace so AI assistants can locate its reusable guidance, prompt assets, environment records, and planning documents with minimal exploration.

## Context

This repository is a documentation-first workspace for standardizing AI-assisted software engineering across projects. `ROADMAP.md` records Phases 1-3 as complete; `WORKSPACE_STATE.md` records Phase 4, Repository Intelligence, as in progress.

The workspace separates reusable engineering standards, operational instructions, task prompts, and repository knowledge. This overview describes the repository itself; detailed guidance remains in its authoritative documents.

## Scope

This overview covers the workspace identity, major structure, confirmed tooling, documented development environment, and high-level components.

It excludes detailed architecture, feature mapping, decisions, task procedures, personal AI behavior rules, and prompt contents. Those belong in their dedicated documents or directories.

## Information

### Repository Identity

| Item | Confirmed information |
| --- | --- |
| Repository type | Personal AI engineering workspace and reusable documentation asset library. |
| Primary objective | Standardize AI-assisted engineering practices, reusable prompts, repository guidance, and repository intelligence. |
| Current milestone | Repository Intelligence v1.0. |
| Current phase | Phase 4 - Repository Intelligence. |

### Structure

| Path | Responsibility |
| --- | --- |
| `agents/` | Personal, technology-agnostic AI development standards. |
| `instructions/global/` | Global guidance for AI behavior, workflows, prompting, search, tool selection, and RTK usage. |
| `instructions/repository/` | Template for repository-specific Copilot instructions. |
| `prompts/` | Reusable Markdown prompt library, its template, and task-, language-, and technology-specific prompts. |
| `docs/` | Repository-intelligence documentation and its shared template. |
| `ROADMAP.md` | Authoritative workspace phase plan, deliverables, and future direction. |
| `WORKSPACE_STATE.md` | Current workspace state, documented environment, installed tools, and active priorities. |

### Confirmed Technologies and Tools

| Category | Confirmed use |
| --- | --- |
| Documentation format | Markdown is the primary format for guidance, templates, prompts, roadmap, and workspace state. |
| AI tools | GitHub Copilot, GitHub Copilot CLI, Cursor, and ChatGPT are listed as primary workspace tools. |
| Development tools | Git, GitHub CLI, RTK, `rg`, `fd`, `jq`, `bat`, and `delta` are listed as installed. |

### Development Environment

- Documented operating system: Windows 11.
- Documented editor and terminal: Visual Studio Code and PowerShell.
- The repository contains no detected package manifest, runtime-version declaration, build configuration, test-runner configuration, or deployment configuration.
- Markdown documentation changes require no repository-specific build or runtime setup.

### Key Components

| Component | Responsibility |
| --- | --- |
| `agents/PERSONAL_AGENTS.md` | Personal engineering principles and AI collaboration standards. |
| `instructions/global/` | Reusable operating guidance for AI-assisted engineering tasks. |
| `prompts/README.md` and `prompts/TEMPLATE.md` | Prompt-library conventions and base structure for new reusable prompts. |
| `instructions/repository/copilot_instructions-template.md` | Starting template for repository-specific AI guidance. |
| `docs/TEMPLATE.md` | Shared standard for repository-intelligence documents. |
| `ROADMAP.md` and `WORKSPACE_STATE.md` | Workspace plan, completion status, priorities, and environment record. |

## References

- `ROADMAP.md` - authoritative plan, phase status, core deliverables, and workspace scope.
- `WORKSPACE_STATE.md` - authoritative current objective, environment, installed tools, and active priorities.
- `agents/PERSONAL_AGENTS.md` - personal engineering and AI collaboration standards.
- `instructions/global/` - operational guidance for AI-assisted development.
- `prompts/README.md` - prompt-library purpose, organization, and authoring conventions.
- `docs/TEMPLATE.md` - required standard for repository-intelligence documents.

## Maintenance

Update this overview when the repository purpose, phase status, major directory structure, core tooling, documented development environment, or key workspace components change.

Revise or remove claims when their source documents no longer support them. Do not update this overview for individual prompt wording or temporary task activity unless it changes repository-level understanding.

## Notes

- The absence of application tooling is a confirmed observation from the current repository root; revise this statement if package, build, test, runtime, or deployment configuration is added.
- The repository instruction template is `instructions/repository/copilot_instructions-template.md`.
- `ROADMAP.md` labels the current Phase 4 section "Ready to Start" and leaves its core tasks unchecked, while `WORKSPACE_STATE.md` reports the phase as in progress and all four core documents are present in `docs/`. Treat the current state as a documented status discrepancy until the roadmap is updated.
