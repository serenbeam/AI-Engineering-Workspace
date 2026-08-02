# Documentation Update Prompt

## Objective

Create or update the specified documentation so it accurately, clearly, and concisely reflects the current implementation, behavior, architecture, or workflow.

## Context

Provide the documentation request, relevant implementation or change set, affected behavior, target audience, existing documentation, repository conventions, and applicable guidance.

## Scope

Update only the specified documentation and the directly related sections needed to keep information accurate and consistent. Identify the source of truth, affected documents, and work that is explicitly out of scope.

## Requirements

- Understand the documentation objective and verify relevant implementation, behavior, requirements, or workflow before editing.
- Use the implementation and applicable repository guidance as the source of truth; distinguish confirmed facts from assumptions.
- Preserve established documentation structure, terminology, style, formatting, and audience expectations.
- Update only information affected by the requested change, including related references, examples, commands, configuration, or links when necessary.
- Remove or correct outdated, contradictory, or duplicated information within the confirmed scope.
- Keep documentation concise, actionable, and appropriate for its intended audience.
- Explain behavior and decisions accurately without inventing details or making unsupported claims.
- Maintain a single source of truth and link to existing authoritative documentation instead of duplicating it.
- Verify internal links, paths, commands, examples, and terminology relevant to the change.
- Preserve unrelated documentation and update implementation only when the confirmed documentation request requires it.

## Constraints

- Do not modify unrelated files or documentation.
- Do not make unsupported assumptions about behavior, requirements, architecture, or future work.
- Do not change implementation, public interfaces, or architecture unless explicitly required by the confirmed scope.
- Do not introduce new documentation frameworks, dependencies, or broad reorganization without clear justification.
- Do not duplicate information that is maintained elsewhere as the authoritative source.
- Do not remove useful context, warnings, or instructions without confirming they are obsolete.

## References

Review applicable guidance and task context:

- `agents/PERSONAL_AGENTS.md`
- `ROADMAP.md`
- `WORKSPACE_STATE.md`
- `prompts/README.md`
- `prompts/TEMPLATE.md`
- `prompts/general-engineering/analysis.md`
- `prompts/general-engineering/planning.md`
- `prompts/general-engineering/feature-implementation.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide:

1. Confirmed documentation scope, source of truth, target audience, and assumptions.
2. A concise summary of the documentation changes made.
3. Files and sections updated, including any corrected links, examples, or references.
4. Consistency checks performed against the relevant implementation or documentation.
5. Remaining gaps, risks, or follow-up documentation work.

## Effort

Medium

## Notes

Review the relevant implementation and existing documentation before editing. If the source of truth, intended audience, or requested behavior is unclear, state the missing information and request clarification rather than guessing. Prefer focused updates over broad rewrites.
