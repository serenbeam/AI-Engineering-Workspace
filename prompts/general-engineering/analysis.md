# Engineering Analysis Prompt

## Objective

Analyse the specified problem, behavior, implementation, or design area and provide an evidence-based understanding before proposing implementation changes.

## Context

Provide only the documentation, files, modules, observed behavior, and requirements relevant to the analysis.

## Scope

Analyse only the specified areas and their direct dependencies. Expand the scope only when evidence shows that it is necessary.

## Requirements

- Understand the current implementation before drawing conclusions.
- Trace relevant behavior and relationships using available evidence.
- Distinguish confirmed facts, assumptions, and unknowns.
- Identify existing patterns, constraints, and reusable solutions where relevant.
- Explain cause-and-effect relationships clearly.
- Prefer the minimum necessary analysis and avoid unrelated exploration.

## Constraints

- Do not implement changes.
- Do not modify files.
- Do not make unsupported assumptions.
- Do not recommend architectural changes unless the evidence requires them.
- Do not analyse unrelated areas.

## References

Include only authoritative repository instructions, requirements, issue reports, architecture documentation, and implementation details directly relevant to this analysis. Link rather than paste long material, and summarize content already inspected.

## Expected Output

Provide a concise analysis containing:

1. Scope and relevant context reviewed.
2. Evidence-based findings, with affected files or components where applicable.
3. Confirmed root cause or explanation of the current behavior.
4. Assumptions, unknowns, and questions that require clarification.
5. Recommended next step, including the minimum change to investigate or implement when appropriate.

## Effort

Medium

## Notes

Analyse before proposing implementation. If the available evidence is insufficient, state what is missing and request clarification rather than guessing.
