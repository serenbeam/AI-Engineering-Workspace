# Feature Implementation Prompt

## Objective

Implement the specified feature so it integrates naturally with the existing project while preserving established architecture, behavior, and conventions.

## Context

Provide the feature requirements, relevant user or business behavior, affected areas, existing patterns, available analysis or plan, and applicable repository guidance.

## Scope

Implement only the specified feature and the direct changes required to support it. Identify affected files, modules, interfaces, tests, documentation, and work that is explicitly out of scope.

## Requirements

- Understand the requirements and inspect the relevant implementation before making changes.
- Review available analysis or planning before implementation; when neither is available, perform the minimum analysis needed to implement safely.
- Reuse existing architecture, patterns, utilities, and dependencies where appropriate.
- Implement the minimum maintainable change that satisfies the confirmed requirements.
- Preserve existing behavior, compatibility, error handling, naming, style, and separation of responsibilities unless a change is explicitly required.
- Handle relevant edge cases and failure modes intentionally.
- Keep changes focused, readable, testable, and consistent with repository conventions.
- Add or update focused tests when the repository has applicable test coverage.
- Verify the feature, relevant integrations, and regression risks using the project's existing validation procedures.
- Update documentation only when the feature changes information that documentation must accurately describe.

## Constraints

- Do not implement unsupported assumptions or invent business rules.
- Do not modify unrelated files, behavior, or interfaces.
- Do not introduce dependencies, architectural patterns, or broad refactoring without clear justification.
- Do not rename files, modules, or public interfaces unless required by the confirmed scope.
- Do not remove tests or reduce meaningful verification coverage.
- Do not expand the scope beyond direct dependencies unless evidence shows it is necessary.

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
- `prompts/general-engineering/refactoring.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide:

1. Confirmed scope, relevant assumptions, and affected areas.
2. A concise summary of the implementation and how it satisfies the requirements.
3. Files or components changed, including any tests and documentation updates.
4. Verification performed, expected behavior confirmed, and regression considerations.
5. Remaining risks, limitations, or follow-up work.

## Effort

Medium

## Notes

Analyse and plan before coding when the feature is non-trivial, high-impact, or ambiguous. If requirements, expected behavior, or scope remain unclear, state the missing information and request clarification rather than guessing. Prefer incremental delivery and the smallest maintainable implementation.
