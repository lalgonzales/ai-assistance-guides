---

# Plan Structure Guide

> **Note:** Whenever possible, update guides, templates, or systematization instead of creating new documentation. The assistant MUST always act according to the active plan and this guide, and should only propose new documentation if it is strictly necessary for traceability or team learning.

This guide defines the minimum structure, best practices, and actionable examples for all planning documents in this project. All plans MUST be written in English and follow these standards to ensure clarity, traceability, and robust closure.

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


## Example Plan Template

```
# [Short Title]: [Objective]

## Objective
Briefly describe the goal and scope.

## Progress & Checklist
- [x] Step 1 completed
- [ ] Step 2 in progress
- [ ] Step 3 pending
- [ ] Validate with robust tests (CLI, flows, suite)
- [ ] Update documentation and READMEs
- [ ] Register new patterns/lessons
- [ ] Propose improvements to guides/templates
- [ ] Clean up and formally close the plan

## Validation
- [ ] Run CLI: `python scripts/smart_sync.py --dry-run`
- [ ] Run test suite: `pytest`
- [ ] Confirm expected output and no errors

## Documentation
- [ ] Update `README.md` and affected guides

## Systematization
- [ ] Add new patterns to `docs/sistematizacion/`

## Closure Criteria
- [ ] All checklist items complete
- [ ] Evidence of validation attached
- [ ] Plan formally closed and referenced in changelog

## Traceability
- Files modified: ...
- Error logs: ...
```

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

## Relationship to Other Templates
- Use this guide together with `PLANNING_TASK_TEMPLATE.md` for new plans.
- Reference `VALIDATION_LOG_TEMPLATE.md` for documenting validation results.
- For error handling, use `ERROR_HANDLING_ENTRY_TEMPLATE.md` and link logs in your plan.

---

> For questions or improvements, propose changes directly in this guide or via the main AI Assistant Guidelines.
