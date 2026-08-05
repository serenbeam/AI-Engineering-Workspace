# Node.js Engineering Prompt

## Objective

Implement, analyse, review, or improve the specified Node.js behavior while preserving project conventions, runtime compatibility, correctness, security, reliability, readability, maintainability, and operational behavior.

## Context

Provide the task objective, affected Node.js files or modules, Node.js version, package manager, module system, runtime and deployment environment, relevant framework or tooling, external services, existing patterns, tests, requirements, and applicable repository guidance.

## Scope

Work only within the specified Node.js areas and their direct dependencies. Identify the affected modules, public interfaces, request or command paths, asynchronous boundaries, external integrations, runtime environments, validation paths, operational concerns, and work that is explicitly out of scope.

## Requirements

- Understand the requested behavior, current implementation, Node.js version, package manager, module system, runtime environment, and repository conventions before making changes or recommendations.
- Reuse existing module structure, utilities, configuration, error-handling patterns, logging, dependency-injection patterns, and dependencies where appropriate.
- Preserve runtime compatibility, module-system conventions, public interfaces, command-line behavior, service contracts, configuration behavior, and established API behavior unless a change is explicitly required.
- Write clear, idiomatic JavaScript or TypeScript using descriptive names, focused functions, explicit control flow, and predictable module boundaries.
- Use Node.js and language features only when they are supported by the configured runtime, transpilation, and repository conventions.
- Handle asynchronous behavior, promises, streams, errors, resource cleanup, cancellation, timeouts, and concurrency intentionally when relevant.
- Validate and normalize external input at system boundaries, including request data, environment variables, command-line arguments, files, messages, and third-party responses.
- Preserve secure handling of credentials, secrets, file paths, network input, serialization, authentication, authorization, and untrusted data where relevant.
- Use environment configuration through existing repository patterns. Validate required configuration early and do not hard-code secrets or environment-specific values.
- Keep error handling intentional and actionable. Preserve established error contracts, status codes, logging, and observability behavior without exposing sensitive details.
- Manage resources explicitly where relevant, including file handles, network connections, database clients, streams, timers, child processes, event listeners, and graceful shutdown.
- Avoid blocking the event loop with CPU-intensive or synchronous work on request paths. Use existing project patterns for background work, queues, workers, or streaming when needed.
- Consider performance, memory use, backpressure, retries, idempotency, and failure modes when they materially affect the requested task.
- Preserve or improve test coverage using existing test tools and patterns. Test observable behavior, error paths, and boundary conditions where practical.
- Use the smallest maintainable change that satisfies the confirmed requirements and update documentation only when needed.

## Constraints

- Do not modify unrelated files, behavior, public interfaces, API contracts, configuration, deployment behavior, or runtime support.
- Do not introduce dependencies, frameworks, build tools, transpilation, module systems, background-processing systems, or architectural patterns without clear justification.
- Do not assume Node.js version, package manager, module system, operating-system behavior, serverless or long-running-process model, container support, or deployment environment without confirming the project configuration.
- Do not use deprecated APIs, unsupported language features, environment-specific globals, blocking work, or synchronous I/O on latency-sensitive paths without compatibility and performance evidence.
- Do not weaken input validation, error handling, authentication, authorization, secret handling, logging, security, type safety, or test coverage.
- Do not modify lockfiles, generated files, environment templates, deployment configuration, or production runtime settings unless the approved scope requires it.
- Do not perform unrelated refactoring, broad formatting changes, or architecture changes.
- Do not invent requirements, API contracts, configuration values, infrastructure behavior, or business rules.

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
- `prompts/programming-languages/javascript.md`
- `prompts/programming-languages/typescript.md`
- `instructions/global/workflow.md`
- `instructions/global/prompting-guide.md`

## Expected Output

Provide:

1. Confirmed scope, Node.js runtime and module compatibility assumptions, and affected modules, interfaces, asynchronous boundaries, and integrations.
2. A concise summary of the implementation, analysis, review findings, or refactoring performed.
3. Node.js-specific considerations addressed, including asynchronous behavior, input validation, error handling, resources, security, configuration, and operational behavior where relevant.
4. Files changed and relevant tests or validation performed.
5. Remaining risks, limitations, or follow-up work.

## Effort

Medium

## Notes

Use the repository's Node.js version, package manager, module system, runtime model, framework, configuration, observability, deployment environment, and test tooling as the source of truth. Prefer established repository patterns over generic Node.js recommendations when they intentionally differ. If the task, expected behavior, runtime compatibility, external interfaces, configuration, security requirements, or operational constraints are unclear, state the missing information and request clarification rather than guessing.
