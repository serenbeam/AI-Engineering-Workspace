# AI Engineering Workflow

Version: 1.0

Status: Stable

---

# Purpose

This document defines the standard engineering workflows used when collaborating with AI.

The objective is to provide consistent, repeatable, and technology-agnostic processes for common software engineering tasks.

These workflows describe *how work should be approached*, not *how code should be written*.

---

# Scope

These workflows apply to all software projects unless a repository defines its own workflow.

Project-specific workflows may extend or replace individual sections where appropriate.

---

# Workflow Selection Guide

Use the workflow that best matches the current task.

| Task | Workflow |
|------|----------|
| Implement a new feature | Feature Implementation |
| Fix a bug | Bug Investigation |
| Improve existing code | Refactoring |
| Review changes | Code Review |
| Update documentation | Documentation Update |
| Upgrade dependencies | Dependency Update |
| Understand a repository | Repository Exploration |

---

# Common Workflow Principles

The following principles apply to every workflow.

1. Understand the objective.
2. Analyse the current implementation.
3. Identify constraints.
4. Plan the minimum required changes.
5. Implement carefully.
6. Verify correctness.
7. Update documentation when necessary.

Avoid skipping analysis unless explicitly requested.

---

# Feature Implementation

## Objective

Implement new functionality while preserving the existing architecture.

## Standard Workflow

1. Understand requirements.
2. Locate affected components.
3. Review existing implementation.
4. Identify reusable code.
5. Plan the implementation.
6. Implement the minimum required changes.
7. Verify functionality.
8. Update documentation if required.

## Expected Outcome

A feature that integrates naturally with the existing project while minimising unnecessary changes.

---

# Bug Investigation

## Objective

Resolve defects by identifying and fixing the root cause rather than treating symptoms.

## Standard Workflow

1. Understand the reported behaviour.
2. Reproduce the issue.
3. Locate the affected implementation.
4. Identify the root cause.
5. Confirm the diagnosis with evidence.
6. Implement the smallest effective fix.
7. Perform regression checks.
8. Verify the solution.

## Expected Outcome

A verified fix that resolves the issue without introducing new regressions.

---

# Refactoring

## Objective

Improve maintainability without changing observable behaviour.

## Standard Workflow

1. Understand the current implementation.
2. Identify maintainability issues.
3. Evaluate expected benefits.
4. Refactor incrementally.
5. Preserve behaviour.
6. Verify correctness.
7. Update documentation if required.

## Expected Outcome

Cleaner code with improved readability or maintainability while preserving functionality.

---

# Code Review

## Objective

Evaluate implementation quality and identify opportunities for improvement.

## Standard Workflow

1. Understand the scope.
2. Review correctness.
3. Review architecture.
4. Review maintainability.
5. Review readability.
6. Review performance when relevant.
7. Provide objective recommendations.

## Expected Outcome

Clear, evidence-based feedback prioritised by impact.

---

# Documentation Update

## Objective

Keep documentation aligned with implementation.

## Standard Workflow

1. Identify implementation changes.
2. Locate affected documentation.
3. Update relevant sections.
4. Remove outdated information.
5. Verify consistency.

## Expected Outcome

Documentation accurately reflects the current implementation.

## Documentation Impact Check

Before completing a change that affects repository guidance, confirm whether it
changes:

1. a responsibility, location, or capability in `docs/`;
2. a repository-level decision in `docs/decisions.md`;
3. phase status, deliverables, or direction in `ROADMAP.md`; or
4. current objective, environment, or priorities in `WORKSPACE_STATE.md`.

Update only the applicable source-of-truth document and its direct references.
Do not update every document by default.

---

# Dependency Update

## Objective

Introduce or update dependencies responsibly.

## Standard Workflow

1. Understand the purpose.
2. Verify necessity.
3. Review compatibility.
4. Evaluate alternatives.
5. Implement changes.
6. Verify build.
7. Verify runtime behaviour.

## Expected Outcome

Dependencies remain minimal, compatible, and maintainable.

---

# Repository Exploration

## Objective

Understand only the repository context required for the current task.

## Standard Workflow

1. Review repository documentation.
2. Locate relevant files.
3. Inspect only the necessary implementation.
4. Expand exploration only when required.
5. Avoid repeatedly reading the same files.
6. Stop exploration when sufficient context has been gathered.

## Expected Outcome

Efficient repository understanding with minimal unnecessary context.

---

# Verification

Before considering any task complete, verify:

- requirements have been satisfied,
- architecture remains consistent,
- existing patterns have been preserved,
- imports and references are valid,
- naming remains consistent,
- unnecessary changes have not been introduced,
- documentation has been updated when required.

---

# Guiding Principle

Follow structured engineering workflows that maximise correctness, maintainability, and consistency while minimising unnecessary changes and context usage.

---

# End of Document