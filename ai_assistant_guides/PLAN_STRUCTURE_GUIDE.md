---

# Plan Structure Guide

> **Note:** Whenever possible, update guides, templates, or systematization instead of creating new documentation. The assistant MUST always act according to the active plan and this guide, and should only propose new documentation if it is strictly necessary for traceability or team learning.


This guide defines the minimum structure, best practices, and actionable examples for all planning documents in this project. All plans MUST be written in English and follow these standards to ensure clarity, traceability, and robust closure.

> **For critical or long-lived plans:**
> Always use or adapt the [PLAN_HANDOVER_TEMPLATE.md](./PLAN_HANDOVER_TEMPLATE.md) to ensure the plan is self-sufficient, recoverable, and ready for handover or asynchronous continuation.

> ⚠️ All plans MUST be created from the official [PLAN_HANDOVER_TEMPLATE.md](./PLAN_HANDOVER_TEMPLATE.md). It is FORBIDDEN to create plans without this structure. Any plan not following this template is INVALID and must be regularized immediately.

---

## Minimum Plan Structure

1. **Title and Objective**
   - Clearly state the goal, scope, and context of the plan.
2. **Checklist & Progress**
   - List all actionable steps as checkboxes in a single unified section at the top of the plan. Each step should be specific, verifiable, and reflect both progress and validation criteria.
   - Avoid duplicating checklists or progress sections; keep a single, up-to-date list.
3. **Validation & Testing**
   - Define how results will be validated (e.g., CLI commands, test suite, integration flows).
   - Include expected outputs or acceptance criteria.
4. **Documentation Update**
   - Specify which READMEs, guides, or user docs must be updated.
5. **Systematization**
   - Register new patterns, lessons, or reusable solutions in `docs/sistematizacion/` if applicable.
6. **Closure Criteria**
   - List explicit criteria for plan completion (e.g., all tests pass, docs updated, evidence attached).
7. **Traceability**
   - Reference all files created/modified. Link to error logs or validation evidence as needed.

---



## Plan Template (Single Source of Truth)

> **All plans MUST use the [PLAN_HANDOVER_TEMPLATE.md](./PLAN_HANDOVER_TEMPLATE.md) as the canonical template.**
> For simple plans, fill only the required sections; for critical/long-lived plans, complete all sections for robust handover and recovery.

This ensures every plan is self-sufficient, traceable, and easy to continue or close by any contributor. Do not create or use alternative templates.

---

## Logging & Plan Structure Standard (2025-07-06)

- All detailed logs of debugging/testing cycles (commands, outputs, errors, análisis) must go in a dedicated log file (e.g., `plan_X_log.md`) linked from the main plan.
- The main plan should only contain the checklist, key conclusions, decisions, and links to logs and relevant files.
- Summarize only the most important results and next steps in the plan; keep the log file as the full trace of actions and evidence.
- This ensures plans remain clear, auditable, and easy to review, while logs provide full traceability for debugging and validation.

---

## Actionable Steps Principle

All steps in a plan must be clear, concrete, and directly executable by any contributor, without requiring further clarification. Avoid ambiguity and open-ended instructions.

**Guidelines:**
- Each step should specify exactly what to do (e.g., command to run, file to edit, output to check).
- If there are options, list them explicitly and describe how to choose.
- Avoid vague language like "analyze", "review", or "as needed" unless followed by a concrete action.
- Use checklists for all actionable items.

**Examples:**
- Good: `Run python3 scripts/smart_sync.py --endpoints events`
- Good: `Update README.md to document the new --endpoints flag`
- Good: `If error X occurs, create an error log using ERROR_HANDLING_ENTRY_TEMPLATE.md and link it here.`
- Bad: `Test the sync` (too vague)
- Bad: `Review the output` (what is the expected output? what to do if it fails?)

Plans should be as independent and self-contained as possible, so any team member can execute them without extra context.

---


## Best Practices
- Keep steps actionable and verifiable.
- Update the plan as you learn or as requirements change.
- Use error logs and validation evidence for traceability.
- Always close the plan with a summary and links to evidence.
- Propose improvements to this guide or templates as needed.

---

## Plan Closure

All plans must be formally closed following these steps:
- Ensure all checklist items are complete and validated.
- Attach or link all evidence (logs, outputs, screenshots, etc.).
- Summarize key learnings and decisions.
- Archive the plan if it has long-term value, or delete if not needed (see archiving policy).
- Remove all temporary/intermediate files unless needed for traceability.
- If minor tasks remain, create a mini-plan and close the main one.
- Reference the [PLAN_HANDOVER_TEMPLATE.md](./PLAN_HANDOVER_TEMPLATE.md) for closure instructions and required sections.

This ensures every plan is auditable, recoverable, and easy to continue or review by any contributor.

---


## Relationship to Other Templates
- Use this guide together with `PLANNING_TASK_TEMPLATE.md` for new plans.
- Reference `VALIDATION_LOG_TEMPLATE.md` for documenting validation results.
- For error handling, use `ERROR_HANDLING_ENTRY_TEMPLATE.md` and link logs in your plan.
- For critical/long-lived plans or when handover is likely, use [PLAN_HANDOVER_TEMPLATE.md](./PLAN_HANDOVER_TEMPLATE.md) to ensure robust continuity and recovery.

---

> For questions or improvements, propose changes directly in this guide or via the main AI Assistant Guidelines.
