# Engineering Planning Prompt

## Objective

Create an implementation plan for the specified software engineering task before making code or documentation changes.

## Context

Provide only the relevant requirements, analysis findings, repository guidance, affected areas, and existing patterns.

## Scope

Define the intended outcome, affected files, modules, or systems, and explicitly identify work that is out of scope.

## Requirements

- Review available analysis before planning implementation.
- Identify the minimum changes needed to achieve the objective.
- Reuse existing patterns and implementations where appropriate.
- Identify dependencies, sequencing, assumptions, risks, and verification needs.
- Prioritize work by impact, dependency order, and risk.
- Divide the work into small, ordered, independently reviewable steps.
- State trade-offs when multiple reasonable approaches exist.
- Preserve existing architecture and behavior unless a change is explicitly required.

## Constraints

- Do not implement changes.
- Do not modify files.
- Do not invent requirements or business rules.
- Do not include unrelated refactoring or scope expansion.
- Do not recommend new dependencies or architectural changes without clear justification.

## References

Review applicable guidance and task context:

- `PERSONAL_AGENTS.md`
- `ROADMAP.md`
- `WORKSPACE_STATE.md`
- `prompts/README.md`
- `prompts/TEMPLATE.md`
- `prompts/general-engineering/analysis.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide a concise plan containing:

1. Objective and confirmed scope.
2. Relevant findings and assumptions from analysis.
3. Affected areas and dependencies.
4. Ordered, prioritized implementation steps, including files or components where known.
5. Expected deliverables and completion criteria.
6. Risks, trade-offs, and unresolved questions.
7. Verification steps with successful criteria that demonstrate the objective has been met.
8. Required documentation updates, if applicable.

## Effort

Medium

## Notes

Clearly distinguish confirmed facts from assumptions. Plan before coding, prefer incremental delivery, and recommend the smallest maintainable change. If information is insufficient, state what is missing and request clarification rather than guessing.
