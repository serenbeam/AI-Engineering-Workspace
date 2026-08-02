# JavaScript Engineering Prompt

## Objective

Implement, analyse, review, or improve the specified JavaScript behavior while preserving project conventions, runtime compatibility, correctness, readability, and maintainability.

## Context

Provide the task objective, affected JavaScript files or modules, runtime and ECMAScript targets, module system, relevant framework or tooling, existing patterns, tests, requirements, and applicable repository guidance.

## Scope

Work only within the specified JavaScript areas and their direct dependencies. Identify the affected modules, public interfaces, runtime environments, validation paths, and work that is explicitly out of scope.

## Requirements

- Understand the requested behavior, current implementation, and repository conventions before making changes or recommendations.
- Reuse existing module structure, utilities, error-handling patterns, and dependencies where appropriate.
- Preserve runtime compatibility, module-system conventions, public interfaces, and established API behavior unless a change is explicitly required.
- Write clear, idiomatic JavaScript using descriptive names, focused functions, and explicit control flow.
- Use modern JavaScript features only when they are supported by the configured runtime, transpilation, and repository conventions.
- Handle asynchronous behavior, promises, errors, resource cleanup, cancellation, and concurrency intentionally when relevant.
- Validate external inputs and preserve expected handling for nullish, missing, malformed, and boundary values.
- Avoid implicit coercion, shared mutable state, hidden side effects, and unnecessary dynamic behavior when clearer alternatives exist.
- Consider performance characteristics only when they are relevant to the requested task, and avoid premature optimization.
- Preserve secure handling of external inputs and avoid introducing common JavaScript security issues where applicable.
- Follow existing repository naming, formatting, and organizational conventions.
- Preserve or improve test coverage using existing test tools and patterns.
- Use the smallest maintainable change that satisfies the confirmed requirements and update documentation only when needed.

## Constraints

- Do not modify unrelated files, behavior, or public interfaces.
- Do not introduce dependencies, build tools, transpilation, type systems, or architectural patterns without clear justification.
- Do not assume browser, server, Node.js, bundler, or ECMAScript support without confirming the project environment.
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
- `prompts/general-engineering/analysis.md`
- `prompts/general-engineering/planning.md`
- `prompts/general-engineering/code-review.md`
- `prompts/general-engineering/refactoring.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide:

1. Confirmed scope, runtime and module compatibility assumptions, and affected areas.
2. A concise summary of the implementation, analysis, review findings, or refactoring performed.
3. JavaScript-specific considerations addressed, including asynchronous behavior, errors, input handling, and compatibility where relevant.
4. Files changed and relevant tests or validation performed.
5. Remaining risks, limitations, or follow-up work.

## Effort

Medium

## Notes

Use repository-specific configuration and conventions as the source of truth for JavaScript style, runtime support, modules, tooling, and tests. Prefer existing repository conventions over generic JavaScript best practices when they intentionally differ. If the task, runtime, compatibility requirements, or expected behavior is unclear, state the missing information and request clarification rather than guessing.
