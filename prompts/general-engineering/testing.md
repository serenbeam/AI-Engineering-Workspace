# Testing Prompt

## Objective

Design, implement, or improve focused tests that verify the specified behavior, protect against regressions, and align with existing repository testing practices.

## Context

Provide the behavior or change to test, relevant requirements, affected implementation, existing tests, known defects or edge cases, available test commands, test environment constraints, and applicable repository guidance.

## Scope

Test only the specified behavior, its direct dependencies, and regression paths that materially affect the requested outcome. Identify the affected components, test levels, existing coverage, and work that is explicitly out of scope.

## Requirements

- Understand the expected behavior, relevant implementation, and existing test conventions before adding or changing tests.
- Review available analysis or planning before testing; when neither is available, perform the minimum analysis needed to identify expected behavior and risks.
- Reuse established test frameworks, helpers, fixtures, naming, organization, and execution commands where appropriate.
- Select the smallest effective mix of test levels, such as unit, integration, end-to-end, or regression tests, based on the behavior and risk.
- Cover the primary success path, relevant edge cases, error handling, boundaries, and regressions identified by the scope.
- Keep tests deterministic, isolated, readable, maintainable, and focused on observable behavior.
- Avoid implementation-coupled assertions unless they verify an intentional contract.
- Use realistic inputs and test data while avoiding sensitive, unnecessary, or duplicated fixtures.
- Preserve existing test coverage and update tests only when requirements or intended behavior have changed.
- Run the relevant existing test commands and report results, failures, limitations, and any unverified paths.

## Constraints

- Do not modify unrelated implementation or tests.
- Do not invent expected behavior, business rules, or test requirements.
- Do not introduce a new test framework, dependency, or broad test infrastructure without clear justification.
- Do not remove tests or reduce meaningful coverage without an approved behavior change.
- Do not make tests pass by weakening assertions, suppressing failures, or hiding defects.
- Do not expand scope beyond direct dependencies unless evidence shows it is necessary.

## References

Include only authoritative repository instructions, behavior requirements, implementation details, and test documentation directly relevant to this testing task. Link rather than paste long material, and summarize content already inspected.

## Expected Output

Provide:

1. Confirmed testing scope, expected behavior, test levels, and assumptions.
2. Test cases added or updated, including the risks and behavior they cover.
3. Files and components changed, including reused test utilities or fixtures.
4. Relevant test commands run and their results, including limitations or unverified paths.
5. Remaining coverage gaps, risks, or follow-up work.

## Effort

Medium

## Notes

Test observable behavior rather than implementation details whenever practical. Prefer focused regression coverage over broad or speculative tests. If expected behavior, test environment, or appropriate test level is unclear, state the missing information and request clarification rather than guessing.
