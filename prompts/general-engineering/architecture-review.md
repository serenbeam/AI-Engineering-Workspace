# Architecture Review Prompt

## Objective

Evaluate the specified system architecture, design area, or proposed architectural change for correctness, maintainability, consistency, scalability, and alignment with established project principles.

## Context

Provide the architecture or design area to review, relevant requirements, diagrams or documentation, affected components, existing implementation patterns, constraints, known concerns, and applicable repository guidance.

## Scope

Review only the specified architecture, its direct dependencies, and the boundaries that materially affect the requested evaluation. Identify the current architecture, intended outcome, affected components, and work that is explicitly out of scope.

## Requirements

- Understand the system objective, current architecture, and relevant requirements before forming conclusions.
- Trace responsibilities, component boundaries, dependencies, data flow, integration points, and ownership where relevant.
- Evaluate alignment with established architecture, separation of concerns, maintainability, readability, testability, reliability, and operational needs.
- Identify coupling, duplication, unclear responsibilities, dependency direction, scaling constraints, and failure boundaries when they materially affect the scope.
- Consider compatibility, security, performance, and resilience only where relevant to the architecture under review.
- Assess whether existing patterns, components, and abstractions can satisfy the objective before recommending new ones.
- Distinguish confirmed findings from assumptions, risks, and unresolved questions.
- Prioritize findings and recommendations by impact, likelihood, and implementation cost.
- Recommend the smallest maintainable architectural change that addresses confirmed concerns.
- Describe trade-offs for multiple reasonable approaches and identify verification needs.

## Constraints

- Do not modify files or implement changes.
- Do not perform a repository-wide audit unless the requested scope requires it.
- Do not recommend architectural changes without evidence and clear benefits.
- Do not introduce patterns, services, dependencies, or abstractions solely for theoretical flexibility.
- Do not recommend unrelated refactoring or scope expansion.
- Do not make unsupported assumptions about requirements, scale, security, performance, or operational constraints.

## References

Review applicable guidance and task context:

- `agents/PERSONAL_AGENTS.md`
- `ROADMAP.md`
- `WORKSPACE_STATE.md`
- `prompts/README.md`
- `prompts/TEMPLATE.md`
- `prompts/general-engineering/analysis.md`
- `prompts/general-engineering/planning.md`
- `prompts/general-engineering/code-review.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide a concise review containing:

1. Confirmed scope, architecture context, and evidence reviewed.
2. Current responsibilities, boundaries, dependencies, and relevant data or control flow.
3. Findings ordered by priority, each with evidence, impact, and recommended correction.
4. Viable options and trade-offs when more than one solution is reasonable.
5. Compatibility, reliability, security, performance, and scalability considerations relevant to the scope.
6. Assumptions, unresolved questions, and information required to validate conclusions.
7. Recommended next steps, including focused implementation or planning work and verification criteria.

## Effort

Medium

## Notes

Review the existing architecture before recommending changes. Focus on material design risks and maintainable improvements rather than style preferences or speculative future needs. If requirements, system boundaries, or operational constraints are unclear, state the limitation and request clarification rather than guessing.
