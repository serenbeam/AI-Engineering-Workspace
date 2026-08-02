# Refactoring Prompt

## Objective

Improve the maintainability, readability, or structure of the specified code while preserving its observable behavior.

## Context

Provide the affected implementation, relevant requirements, existing patterns, known maintainability concerns, and available tests or verification procedures.

## Scope

Refactor only the specified areas and their direct dependencies. Define the behavior that must remain unchanged and identify work that is out of scope.

## Requirements

- Analyse the current implementation and identify the specific maintainability problem before changing code.
- Explain the expected benefit of the refactoring.
- Preserve public behavior, compatibility, error handling, and established architecture.
- Reuse existing patterns and utilities where appropriate.
- Make small, focused, incremental changes.
- Keep naming, structure, and style consistent with the repository.
- Identify regression risks and verify behavior after each meaningful change.
- Update documentation only when the refactoring changes information it must accurately describe.

## Constraints

- Do not change observable behavior unless explicitly required.
- Do not introduce dependencies or architectural patterns without clear justification.
- Do not combine unrelated refactoring with the requested work.
- Do not rename files, modules, or public interfaces unless required by the approved scope.
- Do not remove tests or reduce meaningful verification coverage.

## References

Review applicable guidance and task context:

- `agents/PERSONAL_AGENTS.md`
- `ROADMAP.md`
- `WORKSPACE_STATE.md`
- `prompts/README.md`
- `prompts/TEMPLATE.md`
- `prompts/general-engineering/analysis.md`
- `prompts/general-engineering/planning.md`
- `prompts/general-engineering/bug-investigation.md`
- `prompts/general-engineering/code-review.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide:

1. The maintainability issue and evidence supporting the refactoring.
2. The intended approach and affected areas.
3. A summary of the focused changes made.
4. Behavior-preservation and regression verification results.
5. Remaining risks, assumptions, or follow-up work.

## Effort

Medium

## Notes

Prefer the smallest refactoring that produces a measurable improvement. If the benefit, expected behavior, or scope is unclear, request clarification before making changes.
