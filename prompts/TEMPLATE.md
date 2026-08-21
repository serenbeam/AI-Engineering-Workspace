# AI Engineering Prompt Template

Use this template whenever creating prompts for GitHub Copilot CLI, Cursor, or ChatGPT.

---

# Objective

Clearly describe the desired outcome.

---

# Context

Describe the relevant project context.

Include only the information necessary to complete the task.

Use progressive disclosure: link to authoritative material instead of pasting long content, and summarize files or findings that were already inspected.

---

# Scope

Clearly define what should be included.

Specify affected modules, files, or directories.

---

# Requirements

List the functional and non-functional requirements.

Examples:

- Follow existing project architecture.
- Reuse existing implementations whenever possible.
- Keep changes minimal.
- Maintain consistency.
- Preserve coding style.
- Prefer readability and maintainability.

---

# Constraints

Describe what must NOT be changed.

Examples:

- Do not modify unrelated files.
- Do not introduce new dependencies.
- Do not change architecture.
- Do not rename files.
- Do not perform unrelated refactoring.

---

# References

Reference only authoritative repository instructions, requirements, or documentation that directly govern this task. Do not automatically include generic global documents.

Use repository-relative paths when retained, for example `agents/PERSONAL_AGENTS.md`.

---

# Expected Output

Clearly define the expected deliverable.

Examples

- Analysis report
- Markdown document
- Code implementation
- Refactoring proposal
- Bug investigation
- Review summary

---

# Effort

Choose the smallest sufficient effort level. Increase effort only when the task's scope, risk, or required investigation makes it necessary.

## Small

Single file

Small implementation

Minimal context

---

## Medium

Multiple related files

Limited repository analysis

---

## Large

Feature-level work

Requires broader repository understanding

May require planning before implementation.

---

# Notes

If requirements are ambiguous:

- Explain assumptions.
- Ask clarifying questions.
- Avoid guessing business rules.

Prefer incremental improvements over large rewrites.

Keep responses concise and actionable.