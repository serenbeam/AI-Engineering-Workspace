# TypeScript Engineering Prompt

## Objective

Implement, analyse, review, or improve the specified TypeScript behavior while preserving project conventions, type safety, runtime compatibility, correctness, readability, and maintainability.

## Context

Provide the task objective, affected TypeScript files or modules, compiler configuration, runtime and ECMAScript targets, module system, relevant framework or tooling, existing types and patterns, tests, requirements, and applicable repository guidance.

## Scope

Work only within the specified TypeScript areas and their direct dependencies. Identify the affected modules, public interfaces, type boundaries, runtime environments, validation paths, and work that is explicitly out of scope.

## Requirements

- Understand the requested behavior, current implementation, TypeScript configuration, and repository conventions before making changes or recommendations.
- Reuse existing module structure, shared types, utilities, error-handling patterns, and dependencies where appropriate.
- Preserve compiler settings, runtime compatibility, module-system conventions, public interfaces, and established API behavior unless a change is explicitly required.
- Model domain concepts and public contracts with clear, accurate types that express valid states and required constraints.
- Prefer type inference when it is clear; add explicit annotations at module boundaries, public APIs, complex values, and places where they improve understanding.
- Prefer reusable generic types when they improve correctness and readability without introducing unnecessary complexity.
- Reuse existing utility types before introducing new ones, such as `Partial`, `Pick`, `Omit`, `Record`, and `Readonly`.
- Prefer discriminated unions over boolean flags or loosely related optional properties when modelling multiple valid states.
- Prefer explicit narrowing through control flow and type guards instead of unsafe assertions.
- Avoid unsafe casts, `any`, non-null assertions, and overly broad types unless they are necessary and justified by an existing boundary.
- Narrow unknown or external data through validation and type guards before relying on its structure; TypeScript types do not replace runtime validation.
- Prefer repository-specific type patterns over generic TypeScript recommendations when they intentionally differ.
- Handle asynchronous behavior, promises, errors, resource cleanup, cancellation, and concurrency intentionally when relevant.
- Use modern TypeScript and JavaScript features only when they are supported by the configured compiler, runtime, transpilation, and repository conventions.
- Preserve or improve test coverage using existing test tools and patterns, and verify both type checking and relevant runtime behavior.

## Constraints

- Do not modify unrelated files, behavior, compiler settings, or public interfaces.
- Do not weaken type safety by adding broad casts, `any`, suppressions, or non-null assertions to bypass errors.
- Do not introduce dependencies, build tools, transpilation, type systems, or architectural patterns without clear justification.
- Do not assume browser, server, Node.js, bundler, ECMAScript, or TypeScript support without confirming the project environment and configuration.
- Do not use deprecated APIs, unsupported language features, or environment-specific globals without compatibility evidence.
- Do not perform unrelated refactoring or broad formatting changes.
- Do not invent requirements, API contracts, or business rules.

## References

Review applicable guidance and task context:

- `agents/PERSONAL_AGENTS.md`
- `ROADMAP.md`
- `WORKSPACE_STATE.md`
- `prompts/README.md`
- `prompts/TEMPLATE.md`
- `prompts/programming-languages/javascript.md`
- `prompts/general-engineering/analysis.md`
- `prompts/general-engineering/planning.md`
- `prompts/general-engineering/code-review.md`
- `prompts/general-engineering/refactoring.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide:

1. Confirmed scope, compiler and runtime compatibility assumptions, and affected type boundaries.
2. A concise summary of the implementation, analysis, review findings, or refactoring performed.
3. TypeScript-specific considerations addressed, including type safety, external-data validation, and asynchronous behavior where relevant.
4. Files changed and relevant type checks, tests, or runtime validation performed.
5. Remaining risks, limitations, or follow-up work.

## Effort

Medium

## Notes

Use repository-specific TypeScript configuration and conventions as the source of truth for compiler options, style, module resolution, tooling, and tests. If the task, expected behavior, type contracts, runtime compatibility, or configuration is unclear, state the missing information and request clarification rather than guessing.
