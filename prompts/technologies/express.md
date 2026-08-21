# Express Engineering Prompt

## Objective

Implement, analyse, review, or improve the specified Express behavior while preserving project conventions, HTTP API contracts, middleware flow, correctness, security, reliability, readability, maintainability, and operational behavior.

## Context

Provide the task objective, affected Express application, routers, middleware, controllers, services, request and response contracts, Express and Node.js versions, authentication and authorization approach, external services, deployment environment, existing patterns, tests, requirements, and applicable repository guidance.

## Scope

Work only within the specified Express areas and their direct dependencies. Identify the affected routes, middleware order, request and response boundaries, validation paths, error paths, authorization rules, external integrations, runtime environments, and work that is explicitly out of scope.

## Requirements

- Understand the requested behavior, current implementation, Express and Node.js versions, middleware order, deployment environment, and repository conventions before making changes or recommendations.
- Reuse existing router structure, middleware, controllers, services, validation, authentication, authorization, error handling, logging, configuration, and dependencies where appropriate.
- Preserve established HTTP methods, route paths, request and response schemas, status codes, headers, cookies, pagination, error contracts, and API behavior unless a change is explicitly required.
- Keep routing, middleware, request handling, domain logic, persistence, and response formatting separated according to existing repository patterns.
- Register middleware in the required order and ensure route-specific middleware, fallbacks, and error-handling middleware remain reachable.
- Validate and normalize request parameters, query values, headers, cookies, body data, files, and other untrusted input at the HTTP boundary before relying on them.
- Handle asynchronous route and middleware errors according to the installed Express version and existing repository pattern. Route errors through the established error handler and avoid sending more than one response.
- Return intentional status codes and response shapes. Preserve consistent handling for success, validation failures, authentication and authorization failures, missing resources, conflicts, rate limits, and unexpected errors where relevant.
- Preserve secure HTTP behavior, including authentication, authorization, session or cookie handling, CORS, CSRF protection, security headers, rate limiting, body and upload limits, proxy trust, and sensitive-data handling when relevant.
- Use configuration through existing repository patterns. Validate required configuration early and do not hard-code secrets, origins, hosts, ports, paths, or environment-specific values.
- Keep logging, correlation identifiers, error reporting, and observability consistent with existing patterns without exposing sensitive information to clients or logs.
- Handle request cancellation, timeouts, streaming, uploads, response completion, resource cleanup, and graceful shutdown intentionally when relevant.
- Avoid blocking the event loop with CPU-intensive or synchronous work on request paths. Use existing project patterns for background work, queues, workers, or streaming when needed.
- Consider performance, caching, backpressure, retries, idempotency, concurrency, and failure modes when they materially affect the requested task.
- Preserve or improve test coverage using existing test tools and patterns. Test observable HTTP behavior, middleware order, error paths, authorization boundaries, and validation failures where practical.
- Use the smallest maintainable change that satisfies the confirmed requirements and update documentation only when needed.

## Constraints

- Do not modify unrelated files, behavior, route paths, public API contracts, middleware order, authentication behavior, configuration, deployment behavior, or runtime support.
- Do not introduce dependencies, middleware, frameworks, authentication systems, validation libraries, build tools, or architectural patterns without clear justification.
- Do not assume Express version, Node.js version, module system, proxy configuration, session model, authentication approach, deployment topology, or serverless or long-running-process model without confirming the project configuration.
- Do not weaken input validation, error handling, authentication, authorization, cookie security, CSRF protection, CORS policy, rate limiting, logging, security, privacy, type safety, or test coverage.
- Do not send error details, stack traces, credentials, tokens, personal data, or internal implementation details to clients unless the established contract explicitly requires it.
- Do not modify lockfiles, generated files, environment templates, reverse-proxy configuration, deployment configuration, or production runtime settings unless the approved scope requires it.
- Do not perform unrelated refactoring, broad formatting changes, or architecture changes.
- Do not invent requirements, API contracts, authorization rules, configuration values, infrastructure behavior, or business rules.

## References

Include only authoritative repository instructions, API contracts, runtime configuration, security requirements, and implementation or test context directly relevant to this Express task. Link rather than paste long material, and summarize content already inspected.

## Expected Output

Provide:

1. Confirmed scope, Express and Node.js compatibility assumptions, and affected routes, middleware, request and response contracts, error paths, and integrations.
2. A concise summary of the implementation, analysis, review findings, or refactoring performed.
3. Express-specific considerations addressed, including middleware order, validation, error propagation, HTTP contracts, security, configuration, and operational behavior where relevant.
4. Files changed and relevant tests or validation performed.
5. Remaining risks, limitations, or follow-up work.

## Effort

Medium

## Notes

Use the repository's Express and Node.js versions, router and middleware conventions, API contracts, authentication and authorization model, validation, error handling, configuration, observability, deployment environment, and test tooling as the source of truth. Prefer established repository patterns over generic Express recommendations when they intentionally differ. If the task, expected behavior, API contract, middleware order, security requirements, external interfaces, configuration, or operational constraints are unclear, state the missing information and request clarification rather than guessing.
