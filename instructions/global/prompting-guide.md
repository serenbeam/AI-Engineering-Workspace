# AI Prompting Guide

Version: 1.0

Status: Stable

---

# Purpose

This document defines recommended practices for communicating with AI during software development.

The objective is to create clear, consistent, and efficient prompts that minimise ambiguity, reduce unnecessary context usage, and produce predictable results.

These guidelines are technology-agnostic and apply across software engineering tasks regardless of programming language, framework, or AI coding assistant.

---

# Scope

These guidelines apply when interacting with AI during software development.

Examples include:

- GitHub Copilot
- Cursor
- ChatGPT
- Claude
- Gemini
- Other AI coding assistants

Repository-specific instructions may extend these guidelines where appropriate.

---

# Prompting Principles

A good prompt should:

- Clearly define the objective.
- Provide only the necessary context.
- Describe relevant constraints.
- Specify the expected output.
- Minimise assumptions.
- Encourage evidence-based reasoning.

Avoid vague, broad, or open-ended requests whenever practical.

---

# Prompt Structure

Whenever practical, structure prompts using the following order:

1. Objective
2. Relevant Context
3. Constraints
4. Expected Output
5. Verification Requirements

Not every prompt requires every section, but this structure should be preferred for medium and high-complexity tasks.

---

# Prompt Complexity Guide

Not every task requires the same level of detail.

Choose the prompt structure based on the complexity and expected impact of the task.

| Prompt Type | Typical Effort | Typical Use Cases |
|-------------|----------------|-------------------|
| Quick Prompt | Low | Questions, explanations, small fixes, focused analysis |
| Structured Prompt | Medium | Bug analysis, code review, refactoring, feature planning |
| Comprehensive Prompt | High | Major features, complex implementation, multi-module work, architectural planning |

---

## Quick Prompt

Use for small, focused requests where little context is required.

### Recommended Structure

- Objective
- Optional Context
- Optional Constraints

### Example

Objective

Explain the purpose of this function.

Context

Only analyse `validation.ts`.

Constraint

Do not suggest implementation changes.

---

## Structured Prompt

Use for most day-to-day software engineering tasks.

### Recommended Structure

Objective

<Describe the goal>

Context

<Relevant files, modules, or documentation>

Constraints

<List important limitations>

Expected Output

<Describe the desired response>

### Example

Objective

Review the authentication flow.

Context

Only analyse:

- authentication service
- related controllers

Constraints

- Preserve the current architecture.
- Do not propose new dependencies.

Expected Output

- Maintainability observations
- Potential issues
- Improvement recommendations

---

## Comprehensive Prompt

Use for large or high-impact tasks that require planning before implementation.

### Recommended Structure

Objective

<Describe the overall goal>

Context

<Relevant modules, documentation, business requirements>

Constraints

<List technical and business constraints>

Expected Output

<Planning, implementation, documentation, etc.>

Verification

<Describe how success should be evaluated>

### Example

Objective

Implement a new authentication provider.

Context

Relevant modules:

- authentication
- user management

Existing architecture:

Layered Architecture

Constraints

- Preserve the existing architecture.
- Maintain backwards compatibility.
- Avoid introducing unnecessary dependencies.

Expected Output

1. Implementation plan.
2. Required changes.
3. Potential risks.
4. Final implementation.

Verification

- Existing authentication continues to work.
- New provider integrates successfully.
- No regression in existing functionality.

---

## Choosing the Appropriate Prompt

Use the simplest prompt that provides sufficient context.

General guidance:

- Start with a **Quick Prompt** for simple questions or focused tasks.
- Use a **Structured Prompt** for most software engineering activities.
- Use a **Comprehensive Prompt** when planning or implementing complex changes.

Providing more context than necessary can reduce efficiency, while providing too little context may lead to incomplete or inaccurate responses.

Prefer clarity over length.

---

# Provide Clear Objectives

State the primary goal first.

Good examples:

- Analyse the authentication flow.
- Review the implementation.
- Refactor duplicated logic.
- Explain the existing architecture.

Avoid combining multiple unrelated objectives into a single request.

---

# Provide Relevant Context

Only provide information directly related to the task.

Examples include:

- affected files,
- relevant modules,
- related documentation,
- business requirements,
- existing implementation details.

Avoid providing the entire repository when only a few files are required.

---

# Define Constraints

Describe important limitations before implementation.

Examples:

- preserve the existing architecture,
- minimise code changes,
- avoid adding dependencies,
- maintain backwards compatibility,
- reuse existing utilities,
- do not rename files unless required.

Constraints help AI produce predictable and consistent results.

---

# Specify Expected Output

Clearly describe what should be returned.

Examples:

- implementation plan,
- root cause analysis,
- code review,
- refactoring recommendations,
- documentation updates,
- implementation.

The more specific the expected output, the more consistent the response.

---

# Request Analysis Before Implementation

For non-trivial tasks, prefer requesting analysis before requesting implementation.

Recommended sequence:

1. Analyse
2. Plan
3. Implement

This approach reduces unnecessary implementation and encourages better engineering decisions.

---

# Keep Context Focused

Provide only the information required for the current task.

Prefer:

- relevant files,
- relevant functions,
- relevant modules,
- related documentation,
- specific features.

Avoid requesting repository-wide analysis unless genuinely necessary.

---

# Separate Large Tasks

Break large requests into smaller steps whenever practical.

Preferred sequence:

1. Analysis
2. Planning
3. Implementation
4. Verification

Avoid combining multiple complex tasks into a single request.

---

# Request Evidence

When requesting analysis or review, encourage evidence-based conclusions.

Examples:

- reference affected files,
- explain the execution flow,
- identify observable behaviour,
- distinguish facts from assumptions.

Avoid accepting unsupported conclusions.

---

# Encourage Minimal Changes

When requesting implementation, explicitly encourage small, focused modifications.

Examples:

- preserve existing architecture,
- reuse existing implementations,
- minimise changes,
- avoid unrelated refactoring.

Small, focused changes improve maintainability and simplify code review.

---

# Ask for Trade-offs

When multiple solutions are possible, request an explanation of the trade-offs.

Examples include:

- advantages,
- disadvantages,
- complexity,
- maintainability,
- long-term impact.

Avoid asking AI to choose arbitrarily without justification.

---

# Verification

When implementation is requested, specify how success should be evaluated.

Examples:

- expected behaviour,
- affected components,
- possible side effects,
- regression risks,
- documentation updates.

Verification improves confidence in the final result.

---

# Prompt Examples

## Good Request

Objective

Review the authentication flow.

Context

Only analyse the authentication module and related services.

Constraints

Do not propose architectural changes.

Expected Output

Identify maintainability issues and provide improvement recommendations.

---

## Less Effective Request

Review the whole project and improve everything.

### Reason

The request is too broad, lacks constraints, and does not define the expected outcome.

---

# Common Mistakes

Avoid:

- combining multiple unrelated objectives,
- providing excessive repository context,
- omitting important constraints,
- leaving the expected output undefined,
- requesting implementation before understanding the problem,
- asking AI to make unsupported assumptions.

---

# Relationship with Other AI Workspace Documents

This guide complements the other documents in the AI Engineering Workspace.

| Document | Primary Responsibility |
|----------|------------------------|
| PERSONAL_AGENTS.md | Engineering principles and collaboration standards |
| copilot-instructions.md | Global AI behaviour |
| workflow.md | Standard engineering workflows |
| prompting-guide.md | Effective communication with AI |
| Repository Copilot Instructions | Repository-specific knowledge |
| AGENTS.md | Project-specific rules and business context |

Each document has a distinct responsibility and should avoid duplicating information from the others.

---

# Guiding Principle

Effective prompting begins with a clear objective, sufficient context, explicit constraints, and well-defined expectations.

Better prompts produce better engineering outcomes.

---

# End of Document