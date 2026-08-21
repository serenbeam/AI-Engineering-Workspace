# Repository Intelligence Document Template

Use this template when creating or maintaining repository intelligence documentation.

Repository intelligence documents provide concise, evidence-based knowledge that helps AI understand a repository with minimal unnecessary exploration. They describe what AI should know about the repository; they do not define AI behavior, workflows, prompts, or task-specific instructions.

## Purpose

Describe the repository knowledge this document provides.

State the document's reusable value to an AI assistant. Do not include task-specific objectives or instructions.

## Context

Provide only the repository context necessary to interpret this document.

Prefer stable, high-value facts. Reference related repository-intelligence documents when they provide necessary context.

## Scope

Define the repository areas, boundaries, components, features, architectural concerns, or decisions covered by this document.

State what is intentionally outside its scope when that prevents overlap or ambiguity.

## Information

Provide the core repository knowledge in a structure appropriate to this document's purpose.

Use concise tables, lists, diagrams, or links when they improve retrieval. Do not force identical information across repository-overview, architecture, feature-map, and decisions documents.

Summarize stable, decision-relevant findings. Reference authoritative source code, configuration, documentation, and decision records instead of duplicating them.

Clearly distinguish confirmed facts from assumptions, unknowns, and items requiring verification.

## References

List the authoritative repository-relative sources that support or extend this document.

Prefer source code, configuration, package manifests, existing documentation, architecture documents, and decision records. Do not duplicate their detailed contents.

## Maintenance

State when this document must be reviewed or updated.

Update it when information covered by this document changes or when its authoritative sources change.

Revise or remove claims that are no longer supported by their authoritative sources.

Do not update it for unrelated or temporary implementation details.

Before updating, identify whether the change also affects a repository-level
decision, phase plan, or current workspace state. Update only
`docs/decisions.md`, `ROADMAP.md`, or `WORKSPACE_STATE.md` when their
respective source-of-truth responsibilities are affected.


## Notes

Include only repository-level information that is important but does not fit the preceding sections.

Keep the document concise, technology-agnostic where practical, and optimized for efficient AI context use.
