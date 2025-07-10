# Plan Structure Guide (v2 — Table-Based)

## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](./AI_ASSISTANT_GUIDELINES.md).**

- This guide is only for plan structure and template logic.
- For general assistant logic, always refer to the entrypoint first.

## ⚠️ OBLIGATORY PLAN TEMPLATE
**All plans MUST use the [PLAN_HANDOVER_TEMPLATE_v2.md](./PLAN_HANDOVER_TEMPLATE_v2.md) as the only valid structure.**

- Any plan not following this template is INVALID and must be regularized immediately.
- The table structure is defined in the template, not here. This guide only explains the logic, numbering, and best practices for using the template.
- For the actual table, see the template: [PLAN_HANDOVER_TEMPLATE_v2.md](./PLAN_HANDOVER_TEMPLATE_v2.md).

## Minimum Plan Structure

- Steps are numbered for the main flow; incidentals or transversal findings use letters (A, B, C, ...).
- All evidence, discussions, or detailed logs must be kept in external files and linked from the table in the plan.
- The plan must remain clean, with only the table and essential context.

## Actionable Steps Principle

All steps in a plan must be clear, concrete, and directly executable by any contributor, without requiring further clarification. Avoid ambiguity and open-ended instructions.

**Guidelines:**
- Each step should specify exactly what to do (e.g., command to run, file to edit, output to check).
- If there are options, list them explicitly and describe how to choose.
- Avoid vague language like "analyze", "review", or "as needed" unless followed by a concrete action.
- Use the table for all actionable items (see template).

**Examples:**
- Good: `Edit the configuration file to set the required parameter.`
- Good: `Update the documentation to include the new process step.`
- Good: `If an error occurs, create a log file and link it in the table.`
- Bad: `Test the process` (too vague)
- Bad: `Review the output` (what is the expected output? what to do if it fails?)

## Best Practices
- Keep steps actionable and verifiable.
- Update the plan as you learn or as requirements change.
- Use error logs and validation evidence for traceability (always linked from the table).
- Always close the plan with a summary and links to evidence.
- Propose improvements to this guide or templates as needed.

## Plan Closure

All plans must be formally closed following these steps:
- Ensure all table steps are complete and validated.
- Attach or link all evidence (logs, outputs, screenshots, etc.) in the Related column.
- Summarize key learnings and decisions.
- Archive the plan if it has long-term value, or delete if not needed (see archiving policy).
- Remove all temporary/intermediate files unless needed for traceability.
- If minor tasks remain, create a mini-plan and close the main one.
- Reference the [PLAN_HANDOVER_TEMPLATE_v2.md](./PLAN_HANDOVER_TEMPLATE_v2.md) for closure instructions and required sections.

## Relationship to Other Templates
- [AI_ASSISTANT_GUIDELINES.md](./AI_ASSISTANT_GUIDELINES.md) — **MANDATORY ENTRYPOINT**
- [PLAN_HANDOVER_TEMPLATE_v2.md](./PLAN_HANDOVER_TEMPLATE_v2.md) — **MANDATORY PLAN TEMPLATE**
- [VALIDATION_LOG_TEMPLATE.md](./VALIDATION_LOG_TEMPLATE.md) — Optional, for documenting validation results.
- [ERROR_HANDLING_ENTRY_TEMPLATE.md](./ERROR_HANDLING_ENTRY_TEMPLATE.md) — Optional, for error handling logs.

> For questions or improvements, propose changes directly in this guide or via the main AI Assistant Guidelines.
