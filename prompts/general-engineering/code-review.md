# Code Review Prompt

## Objective

Review the specified changes for correctness, maintainability, consistency, and regression risk. Report only actionable findings supported by evidence.

## Context

Provide the change set, relevant requirements, affected areas, existing patterns, and any known behavior or constraints.

## Scope

Review the specified changes and their direct dependencies. Focus on behavior affected by the change; do not perform a general repository audit.

## Requirements

- Understand the objective and intended behavior before evaluating the changes.
- Review correctness, error handling, data flow, and edge cases relevant to the change.
- Check consistency with established architecture, patterns, naming, and documentation.
- Identify maintainability, readability, and performance concerns when they materially affect the change.
- Consider backward compatibility and regression risks.
- Prioritize findings by impact and likelihood.
- Support each finding with the affected area, observed behavior, and rationale.
- Distinguish confirmed findings from assumptions and questions.

## Constraints

- Do not modify files or implement changes.
- Do not report style preferences that are not supported by repository conventions.
- Do not speculate about defects without evidence.
- Do not expand review beyond the specified scope unless it directly affects the change.
- Do not recommend unrelated refactoring, dependencies, or architectural changes without clear justification.

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
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide a concise review containing:

1. Scope reviewed and relevant context.
2. Findings ordered by priority, each with evidence, impact, and recommended correction.
3. Regression, compatibility, and verification considerations.
4. Assumptions, unresolved questions, and areas requiring clarification.
5. A clear statement when no actionable findings are identified.

## Effort

Medium

## Notes

Focus on defects and material risks rather than minor preferences. If the change or requirements are unclear, state the limitation and request the needed context rather than guessing.
