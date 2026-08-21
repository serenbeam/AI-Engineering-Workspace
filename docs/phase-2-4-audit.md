# Phase 2-4 Audit

## 1. Responsibility Map

| File/Asset | Responsibility | Related Phase 5 Task |
|---|---|---|
| `agents/PERSONAL_AGENTS.md` | Durable personal engineering principles and AI collaboration standards. | 1, 6 |
| `instructions/global/copilot_instructions.md` | Default AI behavior, precedence, scope control, exploration, editing, and verification. | 1, 3, 5 |
| `instructions/global/workflow.md` | Reusable workflows for implementation, investigation, review, documentation, dependencies, and exploration. | 1, 6 |
| `instructions/global/prompting-guide.md` | How to write focused, constraint-driven requests with appropriate prompt complexity. | 1, 3, 5 |
| `instructions/global/search-strategy.md` | Incremental, documentation-first repository exploration. | 3, 4, 5 |
| `instructions/global/tool-selection.md` | Tool responsibility and selection guidance. | 5, 7 |
| `instructions/global/rtk-workflow.md` | When RTK helps with large terminal output and context reduction. | 5 |
| `instructions/repository/copilot_instructions-template.md` | Starter structure for project-specific Copilot guidance. | 2, 4, 6 |
| `instructions/repository/copilot_instructions-templete.md` | Exact duplicate of the canonical repository-instructions template. | 2, 3, 6 |
| `prompts/README.md`, `prompts/TEMPLATE.md` | Prompt-library structure, authoring rules, effort selection, and base prompt shape. | 1, 3, 5, 6 |
| `prompts/general-engineering/` | Reusable prompts for analysis, planning, implementation, review, testing, and documentation work. | 1, 3, 6 |
| `prompts/programming-languages/` | JavaScript and TypeScript task considerations. | 1, 3 |
| `prompts/technologies/` | React, React Native, Node.js, and Express task considerations. | 1, 3 |
| `docs/README.md`, `docs/TEMPLATE.md` | Repository-intelligence entry guidance, evidence standards, document boundaries, and maintenance rules. | 2, 4, 6 |
| `docs/repository-overview.md` | High-level repository identity, structure, environment, and component index. | 2, 4 |
| `docs/architecture.md` | Documentation-layer boundaries, relationships, and consultation model. | 1, 2, 4 |
| `docs/feature-map.md` | Capability-to-location map for focused asset discovery. | 3, 4 |
| `docs/decisions.md` | Evidence-supported repository-level decisions and consequences. | 1, 6, 7 |
| `ROADMAP.md` | Authoritative phase plan, completed work, current Phase 5 scope, and future direction. | All |
| `WORKSPACE_STATE.md` | Current milestone, environment, priorities, and non-priorities. | 4, 6, 7 |

## 2. Meaningful Duplication

| Duplication | Where it exists | Why / impact | Source of truth |
|---|---|---|---|
| Exact repository-instructions template | `copilot_instructions-template.md` and misspelled `copilot_instructions-templete.md` have identical SHA-256 hashes. | This is a real maintenance and discovery problem: two equally complete templates can diverge, and only the underscore/`template` path is cited by Phase 4 intelligence. | `instructions/repository/copilot_instructions-template.md` |
| AI behavior and workflow principles | `PERSONAL_AGENTS.md`, global Copilot instructions, workflow, prompting guide, and most prompts repeat "analyse first," "minimal change," "preserve architecture," "avoid assumptions," and documentation expectations. | Intentional reinforcement across different consumption points, but prompt references and long repeated requirements create unnecessary context when used together. | `PERSONAL_AGENTS.md` for durable principles; `copilot_instructions.md` for AI behavior; `workflow.md` for task process; individual prompts only for task-specific constraints. |
| Repository structure and asset locations | `ROADMAP.md`, `WORKSPACE_STATE.md`, `docs/repository-overview.md`, `docs/feature-map.md`, and `docs/architecture.md`. | Some duplication is necessary because these documents answer different questions. It becomes a real problem where Roadmap/State directory trees use hyphenated instruction filenames while current files use underscores, and omit `docs/` from their structure trees. | `docs/repository-overview.md` / `feature-map.md` for current locations; `ROADMAP.md` for phase plan; `WORKSPACE_STATE.md` for current status. |
| Tool-selection and context guidance | Global instructions, search strategy, tool selection, RTK workflow, prompting guide, and prompts. | The documents state distinct intended boundaries, but operational advice is repeated at length. This increases reading cost without adding task-specific decision rules. | `tool-selection.md` for tool choice, `search-strategy.md` for exploration order, `rtk-workflow.md` for RTK thresholds; global instructions should retain only concise defaults. |
| Documentation-maintenance expectations | Personal standards, global instructions, workflow, documentation prompt, docs template, and each Phase 4 document's maintenance section. | Document-level maintenance triggers are correctly local. The broader "update when needed" language does not define a single cross-document impact check. | `docs/TEMPLATE.md` for repository intelligence; `workflow.md` / documentation prompt for task execution; Roadmap and State for phase/status changes. |

## 3. Phase 5 Gap Analysis

| Phase 5 Task | Already Covered | Partially Covered | Missing | Existing File(s) | Gap |
|---|---|---|---|---|---|
| Improve AI instructions | Yes | Yes | No | Personal standards; global instructions; workflow | Clear boundaries exist, but repeated rules and inconsistent `PERSONAL_AGENTS.md` path references weaken the instruction hierarchy. |
| Optimize repository guidance | Yes | Yes | No | Repository template; Phase 4 docs | The template says repository knowledge should be centralized there, while Phase 4 explicitly assigns repository knowledge to `docs/`. Reconcile this boundary and cross-reference. |
| Reduce unnecessary AI context | Yes | Yes | No | Global instructions; prompting guide; search strategy; prompt README/template; docs README | The principle exists, but prompts commonly prescribe many references and Medium effort by default without a compact context-selection rule. |
| Improve repository understanding | Yes | Yes | No | Docs README; overview; architecture; feature map; decisions | Core intelligence is complete. Improve discovery accuracy by correcting stale structure paths and making the entry/read order consistent across workspace governance documents. |
| Improve token efficiency | Yes | Yes | No | Prompting guide; search strategy; tool selection; RTK workflow | Guidance is qualitative. There is no concise decision rule for when to use a short prompt, reference versus paste content, summarize inspected material, or use RTK based on output size. |
| Standardize documentation maintenance | Yes | Yes | No | Docs template; docs README; workflow; documentation prompt | Per-document triggers exist, but there is no shared change-impact convention for deciding whether Roadmap, State, overview, architecture, feature map, or decisions require synchronized updates. |
| Evaluate additional AI tooling when beneficial | No | Yes | No | Tool-selection guide; RTK guide; decisions; Roadmap; State | Tool Selection mentions future expansion but lacks evidence-based evaluation criteria, adoption threshold, and decision-recording path. Phase 6 deferral remains appropriate for tooling that is not yet justified. |

## 4. Existing Documents to Improve

1. `instructions/repository/copilot_instructions-template.md`: clarify that repository-specific operational rules belong here while repository intelligence belongs in `docs/`; reference rather than centralize duplicated facts.
2. `instructions/global/copilot_instructions.md`, `workflow.md`, and `prompting-guide.md`: reduce repeated defaults and establish concise progressive-disclosure/context-selection guidance.
3. `prompts/README.md` and `prompts/TEMPLATE.md`: define minimal reference selection by task and avoid treating every listed reference as required context.
4. Prompt files: retain only genuinely task- or technology-specific rules; rely on the library and global guidance for shared principles.
5. `ROADMAP.md` and `WORKSPACE_STATE.md`: correct current instruction-template filenames and include the completed `docs/` capability in their structure descriptions.
6. `docs/README.md` and `docs/TEMPLATE.md`: define a lightweight documentation impact check and link to the authoritative phase/status documents.
7. `instructions/global/tool-selection.md`: add a bounded evaluation path for beneficial AI tooling, including evidence, cost, compatibility, context impact, and a decision record.

## 5. New Documents That May Actually Be Necessary

None. Existing templates and ownership boundaries can support all identified improvements.

A separate Phase 5 template is not currently justified. New tooling evaluations can be recorded in `docs/decisions.md` after evaluation, while reusable selection criteria belong in `instructions/global/tool-selection.md`.

## 6. Recommended Order for the Seven Phase 5 Tasks

1. Improve AI instructions
2. Optimize repository guidance
3. Reduce unnecessary AI context
4. Improve repository understanding
5. Improve token efficiency
6. Standardize documentation maintenance
7. Evaluate additional AI tooling when beneficial

This order first resolves source-of-truth and instruction-boundary conflicts, then reduces context and discovery cost, standardizes upkeep, and finally evaluates tools against the improved baseline.

## 7. Conclusion

**Remain unchanged:** the Phase 2-4 responsibility-layer model, the Phase 4 core repository-intelligence set, the seven fixed Phase 5 tasks, and the principle that documents should reference authoritative sources rather than duplicate them.

**Improve:** duplicated instruction content, prompt reference breadth, the repository-template/docs boundary, stale filename references in governance documents, and documentation-impact guidance.

**Missing:** a concise progressive-disclosure/context-selection convention, a cross-document maintenance impact check, and evidence-based tooling evaluation criteria.

**Phase 5 template:** it does not appear necessary; the existing prompt, repository-instructions, and repository-intelligence templates are sufficient.

Audit complete. Phase 5 implementation has not started.
