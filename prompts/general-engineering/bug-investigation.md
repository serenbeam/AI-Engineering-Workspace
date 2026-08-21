# Bug Investigation Prompt

## Objective

Investigate the reported defect, identify its root cause with evidence, and recommend the smallest safe resolution.

## Context

Provide the observed behavior, expected behavior, reproduction steps, relevant error output, affected areas, and recent changes when available.

## Scope

Investigate the reported behavior and its direct dependencies. Expand the scope only when evidence indicates that another area contributes to the defect.

## Requirements

- Reproduce or validate the reported behavior when possible.
- Trace the relevant execution flow and identify the point where actual behavior diverges from expected behavior.
- Distinguish confirmed facts, assumptions, and unknowns.
- Identify the root cause rather than treating symptoms.
- Review existing patterns and error-handling behavior before recommending a correction.
- Identify regression risks and verification requirements.
- Recommend the minimum change necessary to resolve the root cause.

## Constraints

- Do not implement changes.
- Do not modify files.
- Do not make unsupported assumptions.
- Do not recommend unrelated refactoring or scope expansion.
- Do not introduce dependencies or architectural changes without clear justification.

## References

Include only authoritative repository instructions, defect reports, requirements, and implementation evidence directly relevant to this investigation. Link rather than paste long material, and summarize content already inspected.

## Expected Output

Provide a concise investigation report containing:

1. Reported and expected behavior.
2. Reproduction status and evidence reviewed.
3. Affected areas and relevant execution flow.
4. Confirmed root cause, or the information needed to confirm it.
5. Assumptions, unknowns, and unresolved questions.
6. Recommended minimum resolution and potential regression risks.
7. Verification steps and success criteria.

## Effort

Medium

## Notes

Investigate before planning or implementing a fix. If the defect cannot be reproduced or evidence is insufficient, state the limitation and request the missing information rather than guessing.
