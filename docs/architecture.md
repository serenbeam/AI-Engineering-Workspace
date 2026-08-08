# Repository Architecture

## Purpose

Describe the workspace's documentation architecture: its responsibility layers, their relationships, and the paths AI assistants should consult for repository-level context.

## Context

This is a documentation-first AI Engineering Workspace, not a deployable software system. Its architecture organizes reusable engineering assets by responsibility so that guidance, task requests, and repository knowledge remain distinct.

`ROADMAP.md` and `WORKSPACE_STATE.md` identify Repository Intelligence as the current Phase 4 focus. This document complements `docs/repository-overview.md` by describing relationships and boundaries rather than repeating the repository inventory.

## Scope

This document covers the architecture of the workspace's Markdown documentation and its conceptual information flows.

It excludes application architecture, runtime execution, deployment, and detailed feature ownership because no application or deployment architecture is present in the repository.

## Information

### Responsibility Layers

| Layer | Primary responsibility | Authoritative location | Boundary |
| --- | --- | --- | --- |
| Personal standards | Defines durable engineering principles and AI collaboration expectations. | `agents/PERSONAL_AGENTS.md` | Does not define repository-specific knowledge. |
| Global instructions | Defines reusable AI workflows, prompting, exploration, tool selection, and RTK usage. | `instructions/global/` | Does not replace project-specific rules or repository facts. |
| Repository instruction template | Provides a starting structure for repository-specific AI guidance. | `instructions/repository/copilot_instructions-template.md` | Does not replace source-of-truth implementation or repository-intelligence documents. |
| Prompt library | Defines reusable task-request structures for engineering activities, languages, and technologies. | `prompts/` | Does not define persistent repository knowledge. |
| Repository intelligence | Records concise, evidence-based knowledge about a repository. | `docs/` | Does not define AI behavior, workflows, or task-specific instructions. |
| Workspace governance | Records workspace direction, phase status, priorities, and environment. | `ROADMAP.md`, `WORKSPACE_STATE.md` | Does not duplicate the detailed content owned by the layers above. |

### Component Relationships

```text
agents/PERSONAL_AGENTS.md
        -> engineering principles

instructions/global/
        -> AI operating methods

instructions/repository/
        -> project-specific instruction starting point

prompts/
        -> reusable task-request structures

docs/
        -> repository knowledge for AI-assisted work

ROADMAP.md + WORKSPACE_STATE.md
        -> workspace direction and current status
```

The arrows express responsibility and intended consultation, not runtime dependencies or automated execution.

### Information Flows

| Flow | Confirmed or inferred | Description |
| --- | --- | --- |
| Workspace evolution | Confirmed | `ROADMAP.md` defines phases and deliverables; `WORKSPACE_STATE.md` records current status, priorities, and environment. |
| Reusable asset authoring | Confirmed | Templates in `prompts/TEMPLATE.md`, `instructions/repository/`, and `docs/TEMPLATE.md` standardize assets created in their respective directories. |
| AI-assisted repository work | Inferred from document responsibilities | An AI assistant combines applicable personal standards, operating instructions, task prompts, and repository intelligence while treating the target repository as the source of truth. |
| Repository intelligence maintenance | Confirmed | Repository knowledge is updated when its covered structure, architecture, features, decisions, dependencies, configuration, or authoritative sources change. |

### Architectural Constraints

- Keep responsibility layers separate to avoid duplicating AI behavior, workflows, task instructions, and repository facts.
- Use templates as shared structures, then specialize the information for their document type.
- Prefer authoritative repository-relative references over copying detailed source, configuration, or decision content.
- Maintain the documentation-first structure unless a repository-level change justifies a new layer or component.

## References

- `docs/TEMPLATE.md` - repository-intelligence standard and maintenance model.
- `docs/repository-overview.md` - repository identity, structure, environment, and component index.
- `agents/PERSONAL_AGENTS.md` - personal standards and documentation principles.
- `instructions/global/copilot_instructions.md` - global AI behavior and instruction priority.
- `instructions/global/workflow.md` - reusable engineering workflows.
- `instructions/global/search-strategy.md` - incremental repository exploration strategy.
- `prompts/README.md` and `prompts/TEMPLATE.md` - prompt-library purpose and template conventions.
- `ROADMAP.md` and `WORKSPACE_STATE.md` - workspace phases, priorities, and current state.

## Maintenance

Update this document when responsibility layers, their ownership boundaries, their relationships, or the workspace governance model changes.

Revise or remove architecture claims when the referenced source documents change. Do not update it for individual prompt, instruction, or repository-intelligence wording unless that change alters a documented responsibility or relationship.

## Notes

- No application runtime, service boundaries, data stores, deployment pipeline, or automated orchestration is confirmed in the current repository.
- The AI-assisted repository-work flow is an inferred conceptual model; consult the cited source documents for their exact rules and precedence.
