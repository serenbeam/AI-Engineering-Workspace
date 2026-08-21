# Prompt Library

## Purpose

The Prompt Library provides reusable, structured prompts for common AI-assisted software engineering tasks. It promotes clear objectives, focused context, explicit constraints, and consistent expected outputs across repositories and AI tools.

Use these prompts as adaptable starting points rather than fixed instructions. Tailor each prompt to the repository, task, and applicable project guidance while keeping the request concise and evidence-based.

## Philosophy

The Prompt Library supports AI collaboration that prioritizes correctness, maintainability, readability, consistency, and simplicity. Prompts should guide AI tools to understand the relevant context, preserve established patterns, and make the minimum change necessary to meet the objective.

Prompts are not a substitute for repository-specific instructions, architecture, or business requirements. When guidance conflicts, follow the repository's applicable rules.

## AI Compatibility

The prompts are technology- and tool-agnostic. They can be used with GitHub Copilot, Cursor, ChatGPT, or other AI assistants that support structured instructions.

Adapt formatting or tool-specific syntax when required, but retain the prompt's objective, context, scope, constraints, expected output, and effort level. This preserves a consistent engineering workflow across AI tools and repositories.

## Recommended Workflow

Use the following workflow for non-trivial engineering tasks:

1. Select the prompt category and effort level that match the task.
2. Copy `TEMPLATE.md` and replace its guidance with task-specific information.
3. Provide only the authoritative repository instructions, documentation, requirements, and files directly relevant to the task.
4. Ask the AI to analyse the existing implementation before proposing a change when the task is not straightforward.
5. Review the proposed approach, risks, and trade-offs before implementation.
6. Implement the smallest maintainable change that satisfies the objective.
7. Verify the expected behavior and update relevant documentation when necessary.

For small, focused tasks, use only the applicable steps. For large or high-impact work, separate analysis, planning, implementation, and verification into distinct requests when practical.

## Progressive Disclosure

Start with the minimum context needed to complete the task safely. Add repository instructions, files, requirements, or documentation only when they directly govern the task or become necessary during investigation.

- Link or reference authoritative material instead of pasting long content.
- Summarize previously inspected files, findings, and decisions; provide exact paths only when the AI needs to inspect them.
- Select task-specific references rather than automatically including generic global documents.
- Choose the smallest effort level that provides a reliable result, and increase it only when scope, risk, or evidence requires it.

## Structure

The library is organized by prompt purpose so it can grow without changing its overall structure.

```text
prompts/
├── README.md
├── TEMPLATE.md
├── general-engineering/
├── programming-languages/
└── technologies/
```

| Location | Purpose |
| --- | --- |
| `README.md` | Describes the library, its conventions, and how to select prompts. |
| `TEMPLATE.md` | Provides the base structure for new prompts. |
| `general-engineering/` | Technology-agnostic engineering prompts. |
| `programming-languages/` | Prompts with language-specific considerations. |
| `technologies/` | Prompts for frameworks, platforms, or other technologies. |

Create a category directory only when it contains a reusable prompt. Keep names descriptive and task-focused, such as `bug-investigation.md` or `code-review.md`.

## Using the Template

Start each new library prompt from `TEMPLATE.md`. Preserve its sections unless a section is not relevant to the task:

1. **Objective** states the outcome to achieve.
2. **Context** supplies only the information needed for the task.
3. **Scope** identifies the included files, modules, or areas.
4. **Requirements** defines expected quality and behavior.
5. **Constraints** protects unaffected behavior and limits unnecessary changes.
6. **References** links only authoritative repository guidance or documentation directly relevant to the task.
7. **Expected Output** defines the required deliverable.
8. **Effort** selects the appropriate task size.

Replace placeholders with task-specific information. Remove examples and instructions intended only for the prompt author before using a prompt with an AI tool.

For example:

```markdown
# Objective

Identify the root cause of a reproducible defect and recommend the smallest safe correction.

# Scope

Analyse only the affected feature and its direct dependencies.

# Constraints

- Do not modify unrelated behavior.
- Do not introduce dependencies.

# Expected Output

- Root cause with supporting evidence.
- Recommended correction and affected areas.
- Verification considerations.

# Effort

Medium
```

## Prompt Categories

### General Engineering

Use `general-engineering/` for workflows that apply regardless of language or technology. Typical prompts include:

- Analysis
- Planning
- Bug investigation
- Code review
- Refactoring
- Feature implementation
- Documentation
- Architecture review
- Performance review
- Testing

### Programming Languages

Use `programming-languages/` when a task requires language-specific conventions, tooling, or design considerations. Keep the underlying engineering workflow reusable; add only details that are genuinely specific to the language.

### Technologies

Use `technologies/` when a task depends on a framework, platform, library, or other technology. Include only technology-specific context that changes how the task should be approached.

## Selecting Effort

Choose the smallest effort level that provides enough context and process for a reliable result.

| Effort | Use When | Typical Prompt Shape |
| --- | --- | --- |
| **Small** | The task is focused, low risk, and limited to a single concern or file. | Objective, focused context, and constraints. |
| **Medium** | The task affects multiple related areas or needs limited repository analysis. | Full template with scope, requirements, and expected output. |
| **Large** | The task is feature-level, cross-cutting, high impact, or requires broad repository understanding. | Full template plus explicit planning, risks, dependencies, and verification. |

Use **Small** for a narrowly scoped explanation, correction, or review. Use **Medium** for most day-to-day engineering tasks, such as investigating a defect or reviewing a related set of changes. Use **Large** for work that should be analysed and planned before implementation, such as an architectural change or a multi-module capability.

## Authoring Guidelines

- Keep each prompt focused on one engineering outcome.
- State the objective before providing context.
- Use progressive disclosure: provide minimal context first and add task-specific authoritative references only as needed.
- Link to long material instead of pasting it, and summarize content already inspected.
- Prefer explicit constraints over implied assumptions.
- Request evidence for analysis and review tasks.
- Define a verifiable expected output for implementation tasks.
- Keep prompts technology-agnostic unless the category requires specialization.
- Update a prompt when its workflow changes; avoid duplicating the same guidance in multiple prompts.

When repository-specific instructions conflict with a library prompt, follow the repository-specific instructions. The library standardizes the task request; it does not replace project requirements.

## Extending the Library

Add a new prompt when a workflow is repeated often enough to benefit from a shared, reusable starting point. Begin from the template, place the prompt in the narrowest appropriate category, and keep its title and filename aligned with the task it supports.

Avoid creating prompts for one-off requests or copying project-specific rules into the library. Link to applicable project guidance at use time instead.
