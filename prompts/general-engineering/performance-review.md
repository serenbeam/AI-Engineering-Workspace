# Performance Review Prompt

## Objective

Evaluate the specified system, feature, change, or workload for performance risks and optimization opportunities. Identify evidence-based improvements that preserve correctness, maintainability, and established architecture.

## Context

Provide the performance concern or goal, affected behavior, expected workload, available metrics or profiling data, relevant implementation, known constraints, current baselines, target thresholds, and applicable repository guidance.

## Scope

Review only the specified performance area, its direct execution path, and dependencies that materially affect the measured or reported behavior. Identify the workload, metrics, environment, affected components, and work that is explicitly out of scope.

## Requirements

- Understand the expected behavior, workload, and relevant performance objective before drawing conclusions.
- Establish or review a baseline using available measurements, profiling data, logs, traces, benchmarks, or reproducible observations.
- Trace the relevant execution path and identify bottlenecks, unnecessary work, resource contention, inefficient data access, allocation pressure, latency, throughput, and scalability constraints where relevant.
- Distinguish measured facts from hypotheses, assumptions, and unknowns.
- Evaluate the impact of the issue on users, systems, resources, and operational cost when evidence is available.
- Review existing architecture, patterns, and utilities before recommending changes.
- Prioritize correctness, reliability, maintainability, and readability before optimization.
- Recommend the smallest change likely to produce a measurable improvement and explain the expected benefit.
- Identify trade-offs, compatibility risks, failure modes, and regression considerations for each material recommendation.
- Define validation steps, comparable measurements, and success criteria for confirming an improvement.

## Constraints

- Do not modify files or implement changes.
- Do not recommend optimization without a performance objective, evidence, or a clearly stated hypothesis to validate.
- Do not make unsupported assumptions about workload, environment, scale, or bottlenecks.
- Do not sacrifice correctness, security, reliability, readability, or maintainability for speculative gains.
- Do not introduce dependencies, caching layers, concurrency, or architectural changes without clear justification.
- Do not perform unrelated refactoring or expand the review beyond the specified scope unless evidence requires it.

## References

Include only authoritative repository instructions, performance objectives, measurements, profiling evidence, and architecture documentation directly relevant to this review. Link rather than paste long material, and summarize content already inspected.

## Expected Output

Provide a concise review containing:

1. Confirmed scope, workload, environment, performance objective, and evidence reviewed.
2. Current baseline and relevant metrics, including measurement limitations.
3. Bottlenecks or risks ordered by priority, each with evidence, impact, and likely cause.
4. Recommended focused improvements, expected benefit, trade-offs, and affected areas.
5. Assumptions, unknowns, and additional data needed to validate conclusions.
6. Verification steps, comparable success criteria, and regression considerations.

## Effort

Medium

## Notes

Measure before optimizing whenever practical. Focus on material bottlenecks and user- or system-visible impact rather than theoretical micro-optimizations. If a baseline, workload, or performance target is unavailable, state the limitation and request the missing information rather than guessing.
