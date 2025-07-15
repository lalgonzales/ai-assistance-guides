# [Plan Title]: [Objective]

> **Edit history:** All normative changes to this template are documented in its [Plan Handover Template Edits Registry](../registry/plan_handover_template/edits_registry_plan_handover.md).

**Plan metadata:**
- **Title:** [Plan Title]
- **Created:** [YYYY-MM-DD]
- **Last updated:** [YYYY-MM-DD]
- **Status:** [draft/in progress/completed]

## 🚦 MANDATORY ENTRYPOINT
All plans and actions must follow [AI_ASSISTANT_GUIDELINES.md](./AI_ASSISTANT_GUIDELINES.md).

## ⚠️ PLAN STRUCTURE
For structure and logic, see [PLAN_STRUCTURE_GUIDE.md](./PLAN_STRUCTURE_GUIDE.md).

---

## 🚦 PRINCIPLES FOR ALL PLANS
- Every plan MUST:
  - Follow a clear, structured route using the official template.
  - Remain clean: only the table and essential context, all evidence/logs linked from the table.
  - Be aligned with defined objectives and actionable steps.
  - Be updated as work progresses or requirements change.
  - Ensure full traceability: all outputs, logs, and decisions must be accessible and referenced.
  - Be formally closed with summary and links to evidence.
  - Use safe commit practices: review changes with `git status`, stage only relevant files, and use descriptive commit messages. See [CODE_QUALITY_SUBGUIDE.md](./CODE_QUALITY_SUBGUIDE.md#mandatory-commit-workflow) for details.

## Objective & Context
Briefly describe the goal, scope, and any relevant background.

## Checklist & Progress (Table-Based)

### Status legend (recommended values):
- ⏳ Pending: Not started yet
- 🔄 In progress: Being worked on
- 🟡 Action required: Needs a decision or integration, but does not block the rest of the plan
- ✅ Completed: Finished and validated
- 🛑 Blocked: Cannot proceed until an external issue is resolved
- ❌ Cancelled: Step was discarded or is no longer relevant
- 📝 Observation: For incidentals or findings that do not require direct action

Use the status that best reflects the situation. Prefer "🟡 Action required" for steps that need a decision or integration but do not block the rest of the plan. Use "🛑 Blocked" only for steps that truly prevent further progress.

| Step | Description | Status | Notes | Related |
|------|-------------|--------|-------|---------|
| 1 | Define objective and scope |  |  |  |
| 2 | List main actions |  |  |  |
| 3 | Validate results and document evidence |  |  |  |
| A | Additional findings |  | For discoveries outside the main flow |  |

- Number main steps (1, 2, 3, ...). Use letters (A, B, ...) for incidentals or transversal findings.
- All evidence, discussions, or detailed logs MUST be saved in the appropriate folder (e.g., `private/plan_logs/`, `private/error_logs/`, etc.) and linked from the table for traceability.
- This is a **MANDATORY ACTION** for plan compliance.
- Keep the plan clean and focused.

## References
- [AI_ASSISTANT_GUIDELINES.md](./AI_ASSISTANT_GUIDELINES.md) — **MANDATORY ENTRYPOINT**
- [PLAN_STRUCTURE_GUIDE.md](./PLAN_STRUCTURE_GUIDE.md) — **PLAN STRUCTURE & LOGIC**
- [VALIDATION_LOG_TEMPLATE.md](./VALIDATION_LOG_TEMPLATE.md) — Optional, for validation logs.
- [ERROR_HANDLING_ENTRY_TEMPLATE.md](./ERROR_HANDLING_ENTRY_TEMPLATE.md) — Optional, for error handling logs.
- [Related files, plans, or artifacts]

## How to Continue if You Are New to This Plan
- What is the current status?
- What are the next steps?
- What should be validated before proceeding?
- Where is the evidence or context?
- Who to contact if blocked?

## Closure & Archiving Instructions
- How to validate closure?
- Where to archive the plan if relevant?
- What temporary files/artifacts must be deleted?
- **Mandatory: Before archiving, verify that all permanent documentation and artifacts are written in ENGLISH, as required by LANGUAGE_POLICY_GUIDE.md. Translate any Spanish content before final closure.**
- **Mandatory: Before any commit (closure, archive, or autonomous action), ALWAYS run `git status` to review and confirm only relevant files are staged.**
- **Mandatory: After deleting all temporary files, also remove any empty folders associated with closed plans in `private/`, leaving only `planning/` and other active folders as needed.**

## Status
- [ ] In progress
- [ ] Blocked
- [ ] Ready to archive
- [ ] Closed

---

_This template ensures every plan is self-sufficient, traceable, and easy to continue or close by any contributor._
