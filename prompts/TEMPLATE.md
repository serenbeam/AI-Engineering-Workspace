# AI Engineering Prompt Template

Use this template whenever creating prompts for GitHub Copilot CLI, Cursor, or ChatGPT.

---

# Objective

Clearly describe the desired outcome.

---

# Context

Describe the relevant project context.

Include only the information necessary to complete the task.

Reference existing documentation when appropriate.

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

Include relevant documents when applicable.

Examples

- PERSONAL_AGENTS.md
- ROADMAP.md
- WORKSPACE_STATE.md
- AGENTS.md
- Architecture documentation
- ADRs
- Feature documentation

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

Select one:

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