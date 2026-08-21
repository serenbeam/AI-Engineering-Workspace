# React Native Engineering Prompt

## Objective

Implement, analyse, review, or improve the specified React Native behavior while preserving project conventions, component boundaries, platform compatibility, accessibility, correctness, readability, maintainability, performance, and mobile user experience.

## Context

Provide the task objective, affected React Native components, hooks, screens, navigation flows, state-management approach, Android and iOS support requirements, React Native and React versions, Expo or React Native CLI configuration, native modules, permissions, styling system, existing patterns, tests, requirements, and applicable repository guidance.

## Scope

Work only within the specified React Native areas and their direct dependencies. Identify the affected components, screens, props, state and data-flow boundaries, navigation paths, platform-specific behavior, native integrations, permissions, accessibility requirements, validation paths, and work that is explicitly out of scope.

## Requirements

- Understand the requested behavior, current implementation, React Native and React versions, development workflow, supported platforms, and repository conventions before making changes or recommendations.
- Reuse existing component structure, hooks, shared UI elements, navigation patterns, state-management patterns, utilities, native modules, styling conventions, and dependencies where appropriate.
- Preserve public component APIs, navigation behavior, deep links, platform-specific behavior, native configuration, and established user-visible behavior unless a change is explicitly required.
- Keep components focused on a clear responsibility; extract a component, hook, or utility only when it improves reuse, readability, or testability.
- Model UI state explicitly, including loading, empty, error, success, disabled, offline, and pending states when relevant.
- Keep state at the lowest common owner that requires it. Avoid duplicated, derived, stale, or unnecessary state when it can be calculated from props, existing state, or data.
- Use effects only to synchronize with external systems. Define complete, stable hook dependency arrays and handle asynchronous work, cancellation, cleanup, app lifecycle changes, and race conditions intentionally when relevant.
- Preserve predictable rendering by using stable keys for collections and avoiding mutation of props, state, context values, and shared objects.
- Use performant list components and virtualization patterns for large or dynamic collections. Apply memoization only when supported by a demonstrated render or computation concern; do not add `memo`, `useMemo`, or `useCallback` by default.
- Design layouts for varying screen sizes, orientations, densities, safe areas, text scaling, keyboard behavior, and platform conventions where relevant.
- Keep navigation, back behavior, gestures, focus behavior, deep links, and screen lifecycle handling consistent with existing repository patterns.
- Use React Native accessibility props and semantic equivalents to provide meaningful labels, roles, states, hints, focus order, and feedback for assistive technologies.
- Handle native capabilities, permissions, secure storage, device data, network availability, and platform privacy requirements intentionally when relevant.
- Isolate Android- or iOS-specific behavior using established project patterns, and preserve equivalent behavior across supported platforms unless a difference is required.
- Follow the existing Expo or native build workflow. For React Native New Architecture work, consider Fabric, TurboModules, or code generation only when the confirmed project configuration and task require them.
- Preserve or improve test coverage using existing test tools and patterns. Test observable user behavior and relevant platform differences rather than implementation details where practical.
- Use the smallest maintainable change that satisfies the confirmed requirements and update documentation only when needed.

## Constraints

- Do not modify unrelated files, behavior, public component interfaces, navigation paths, native configuration, or platform support.
- Do not introduce dependencies, native modules, state-management libraries, navigation systems, styling systems, build tools, or architectural patterns without clear justification.
- Do not assume React Native, React, Expo, Android, iOS, device, emulator, simulator, JavaScript, TypeScript, or New Architecture support without confirming the project environment and configuration.
- Do not add effects, context, global state, memoization, platform-specific code, or component abstraction unless the confirmed problem requires them.
- Do not mutate props, state, context, or other values used by React rendering.
- Do not rely on array indexes as keys when collection order can change, or on effects to compensate for incorrect data flow.
- Do not weaken accessibility, error handling, permission handling, security, privacy, type safety, platform compatibility, or test coverage.
- Do not alter native build files, generated files, permissions, signing, deployment configuration, or app-store metadata unless the approved scope requires it.
- Do not perform unrelated refactoring, broad formatting changes, or visual redesigns.
- Do not invent requirements, UI behavior, API contracts, platform behavior, or business rules.

## References

Include only authoritative repository instructions, platform and accessibility requirements, native configuration, and implementation or test context directly relevant to this React Native task. Link rather than paste long material, and summarize content already inspected.

## Expected Output

Provide:

1. Confirmed scope, React Native and platform compatibility assumptions, and affected components, screens, navigation, native integrations, and data-flow boundaries.
2. A concise summary of the implementation, analysis, review findings, or refactoring performed.
3. React Native-specific considerations addressed, including platform differences, lifecycle, navigation, permissions, accessibility, responsive layout, performance, and user-facing states where relevant.
4. Files changed and relevant tests or validation performed.
5. Remaining risks, limitations, or follow-up work.

## Effort

Medium

## Notes

Use the repository's React Native and React versions, Expo or native workflow, Android and iOS support policy, architecture, navigation, component conventions, state-management approach, styling system, and test tooling as the source of truth. Use platform APIs, native modules, and New Architecture capabilities only when the repository and task support them. Prefer established repository patterns over generic React Native recommendations when they intentionally differ. If the task, expected behavior, supported platforms, native configuration, accessibility requirements, navigation behavior, state ownership, or compatibility requirements are unclear, state the missing information and request clarification rather than guessing.
