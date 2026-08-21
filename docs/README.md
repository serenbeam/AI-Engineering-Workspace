# Repository Intelligence Documents

`docs/` contains concise, evidence-based repository knowledge for AI-assisted development. It complements repository instructions and prompts; it does not duplicate their operational rules or task procedures.

| File | Purpose |
| --- | --- |
| `TEMPLATE.md` | Shared structure and maintenance standard for repository-intelligence documents. |
| `repository-overview.md` | Repository identity, major structure, environment, and component index. |
| `architecture.md` | Responsibility layers, boundaries, relationships, and information flows. |
| `feature-map.md` | Locations of the workspace's major reusable capabilities. |
| `decisions.md` | Significant repository-level decisions, supporting evidence, and known uncertainty. |

Use the most specific document first, then follow its repository-relative references for authoritative detail. Update the relevant document when its covered repository knowledge or source of truth changes.

For a workspace change, perform a focused documentation impact check: update
the relevant intelligence document for changed facts, `decisions.md` for a
material decision, `ROADMAP.md` for phase direction or deliverables, and
`WORKSPACE_STATE.md` for current status or priorities. Do not update
unaffected documents.
