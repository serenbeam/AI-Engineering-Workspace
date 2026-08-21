# React Engineering Prompt

## Objective

Implement, analyse, review, or improve the specified React behavior while preserving project conventions, component boundaries, accessibility, correctness, readability, maintainability, and user experience.

## Context

Provide the task objective, affected React components, hooks, routes, state-management approach, rendering environment, relevant JavaScript or TypeScript configuration, styling system, existing patterns, tests, requirements, and applicable repository guidance.

## Scope

Work only within the specified React areas and their direct dependencies. Identify the affected components, props, state and data-flow boundaries, user interactions, rendering environment, accessibility requirements, validation paths, and work that is explicitly out of scope.

## Requirements

- Understand the requested behavior, current implementation, React version, rendering environment, and repository conventions before making changes or recommendations.
- Reuse existing component structure, hooks, shared UI elements, state-management patterns, utilities, styling conventions, and dependencies where appropriate.
- Preserve public component APIs, routing behavior, and rendering boundaries (including server-rendered and client-rendered components where applicable), unless a change is explicitly required.
- For React 19.x work, consider Actions, form actions, `useActionState`, `useOptimistic`, and Server Components only when they are relevant to the confirmed architecture and task.
- Keep components focused on a clear responsibility; extract a component, hook, or utility only when it improves reuse, readability, or testability.
- Model UI state explicitly, including loading, empty, error, success, disabled, and pending states when relevant.
- Keep state at the lowest common owner that requires it. Avoid duplicated, derived, stale, or unnecessary state when it can be calculated from props, existing state, or data.
- Use effects only to synchronize with external systems. Avoid effects for derived values, event-driven behavior, or control flow that can be expressed during rendering or in event handlers.
- Define complete, stable hook dependency arrays. Prevent stale closures, unintended repeated work, and race conditions in asynchronous effects.
- Handle asynchronous data, errors, cancellation, cleanup, and unmounting intentionally when relevant.
- Preserve predictable rendering by using stable keys for collections and avoiding mutation of props, state, context values, and shared objects.
- Apply memoization only when supported by a demonstrated render or computation concern; do not add `memo`, `useMemo`, or `useCallback` by default.
- Keep forms, validation, controlled or uncontrolled inputs, and submission behavior consistent with existing repository patterns.
- Build accessible interfaces with semantic HTML, keyboard support, visible focus behavior, appropriate labels, and meaningful feedback for loading, errors, and validation.
- Preserve responsive behavior, styling conventions, and visual consistency with the existing application where relevant.
- Preserve or improve test coverage using existing test tools and patterns. Test observable user behavior rather than implementation details where practical.
- Use the smallest maintainable change that satisfies the confirmed requirements and update documentation only when needed.

## Constraints

- Do not modify unrelated files, behavior, public component interfaces, routes, or rendering boundaries.
- Do not introduce dependencies, state-management libraries, styling systems, build tools, or architectural patterns without clear justification.
- Do not assume React version, browser support, server rendering, client rendering, framework behavior, or JavaScript or TypeScript support without confirming the project environment.
- Do not add effects, context, global state, memoization, or component abstraction unless the confirmed problem requires them.
- Do not mutate props, state, context, or other values used by React rendering.
- Do not rely on array indexes as keys when collection order can change, or on effects to compensate for incorrect data flow.
- Do not weaken accessibility, error handling, validation, type safety, or test coverage.
- Do not perform unrelated refactoring, broad formatting changes, or visual redesigns.
- Do not invent requirements, UI behavior, API contracts, or business rules.

## References

Include only authoritative repository instructions, UI and accessibility requirements, rendering configuration, and implementation or test context directly relevant to this React task. Link rather than paste long material, and summarize content already inspected.

## Expected Output

Provide:

1. Confirmed scope, React and rendering-environment assumptions, and affected component, state, and data-flow boundaries.
2. A concise summary of the implementation, analysis, review findings, or refactoring performed.
3. React-specific considerations addressed, including state ownership, effects, asynchronous behavior, accessibility, rendering, and user-facing states where relevant.
4. Files changed and relevant tests or validation performed.
5. Remaining risks, limitations, or follow-up work.

## Effort

Medium

## Notes

Use the repository's React version, framework, and rendering model (client rendering, server rendering, or hybrid rendering) as the source of truth. This prompt applies to React 19.x and earlier supported versions; use React 19.x capabilities, including Actions, form actions, `useActionState`, `useOptimistic`, and Server Components, only when the repository and task support them. Prefer established repository patterns over generic React recommendations when they intentionally differ. If the task, expected behavior, rendering environment, accessibility requirements, state ownership, or compatibility requirements are unclear, state the missing information and request clarification rather than guessing.
