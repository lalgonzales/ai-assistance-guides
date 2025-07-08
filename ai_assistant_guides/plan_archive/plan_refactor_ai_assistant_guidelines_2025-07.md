# Plan: Full Consistency Review and Refactor of AI Assistant Guidelines and Subguides

**Date:** 2025-07-07

## Objective
To review and refactor the `AI_ASSISTANT_GUIDELINES.md` (main guide) and all related subguides to ensure all critical policies are imperative, unambiguous, and actionable. The plan is organized in two main sections: Main Guide Refactor and Subguides Refactor. Progress, next steps, and closure criteria are tracked for each section.

---

## Section 1: Main Guide Refactor

### Status: ✅ Complete
- The main guide (`AI_ASSISTANT_GUIDELINES.md`) has been fully reviewed and refactored.
- All critical rules now use imperative language and are actionable.
- The quick-reference checklist is up to date.
- Formatting and consistency have been validated.

---

## Section 2: Subguides Refactor

### Subguides to Review:
- PLAN_STRUCTURE_GUIDE.md
- VALIDATION_LOG_TEMPLATE.md
- PLANNING_TASK_TEMPLATE.md
- ERROR_HANDLING_ENTRY_TEMPLATE.md
- ERROR_HANDLING_ITERATIVO_TEMPLATE.md
- CODE_QUALITY_SUBGUIDE.md
- README_TEMPLATES.md
- Any other referenced subguide

### Next Steps:
1. For each subguide, review for:
   - Imperative, unambiguous language (MUST, NEVER, ALWAYS)
   - Consistency with the main guide
   - Up-to-date references and actionable instructions
   - Formatting and clarity
2. Update this plan with progress and next steps after each subguide is reviewed.
3. If a subguide is complex, create a linked sub-plan and reference it here.
4. When all subguides are complete, proceed to formal plan closure (see Plan Management Instructions).

---

### PLAN_STRUCTURE_GUIDE.md: ✅ Reviewed and complete (2025-07-07)
- Opening note translated to English and made imperative.
- All sections use imperative, actionable language and are consistent with the main guide.
- No further changes needed.

---

### VALIDATION_LOG_TEMPLATE.md: ✅ Reviewed and complete (2025-07-07)
- Made the template imperative (MUST use for all validation events).
- Clarified where to store completed logs.
- No further changes needed.

---

### PLANNING_TASK_TEMPLATE.md: ✅ Reviewed and complete (2025-07-07)
- Made the language policy and template usage imperative (MUST).
- Clarified cleanup requirements.
- Fully aligned with the main guide; no contradictions.
- No further changes needed.

---

### ERROR_HANDLING_ENTRY_TEMPLATE.md: ✅ Reviewed and complete (2025-07-07)
- Made the template imperative (MUST use for all error handling events).
- Clarified usage and storage location.
- Template remains valuable for traceability and is not redundant with validation logs.
- No further changes needed.

---

### Block: Naming Policy, Autonomy, and Strategic Plan Management (2025-07-07)
- Added and formalized the File & Directory Naming Policy (MANDATORY) in the main guide: all file and directory names MUST be in English by default, with Spanish only for justified, localized content.
- Updated and enforced the autonomy principle: the assistant can act autonomously for routine, trivial, or well-documented actions, only consulting the user for ambiguous or high-impact actions.
- Refined the MANDATORY CONTINUATION POLICY: the plan is now a strategic record of key advances, decisions, blockers, and learnings, not a log of every micro-action. Updates are made at the end of work blocks, milestones, or when there is relevant progress.
- Performed a mass renaming of documentation files in `docs/ai_assistant_guides/` to comply with the new naming policy. All references and internal links were validated.
- Reflected on the balance between documentation and productivity: the plan is now used as a reference and for strategic traceability, not as a distraction from development.
- All changes are fully aligned with the updated AI_ASSISTANT_GUIDELINES.md and best practices for maintainability and future centralization.

### Final Block: Subguide Review, Cleanup, and Plan Closure (2025-07-07)
- All remaining subguides in `docs/ai_assistant_guides/` were reviewed:
  - Empty/obsolete files (`COMMIT_RESTRUCTURE_PLAN.md`, `ITERATIVE_DEVELOPMENT.md`, `TECHNICAL_DECISIONS.md`, `UV_UPDATE.md`) were deleted using the API and, when that failed, via terminal with explicit user approval, as required by the File Operation Validation & Terminal Usage Policy.
  - Deletion was validated by direct search; no orphaned files remain.
  - `README.md`, `SYSTEMATIZATION_TEMPLATE.md`, and `UV_COMMANDS_GUIDE.md` were updated to explicitly reference imperative language, naming, validation, and autonomy policies.
  - All other subguides are now fully aligned with the main guide and project policies.
- The process followed the autonomy principle: routine and well-documented actions were executed directly; user approval was requested for terminal actions.
- All actions and validations are traceable and documented in this plan.

---

## Plan Closure Checklist

- [x] All code and logic changes validated with robust tests or direct validation
- [x] All documentation and READMEs reviewed and updated
- [x] New patterns/lessons systematized in templates and guides
- [x] Improvements to guides/templates proposed and applied
- [x] Plan formally closed and summarized
- [x] Plan ready to be archived or deleted from `private/planning/`

### Closure Summary (2025-07-07)
All objectives of the plan have been met:
- The AI Assistant Guidelines and all related subguides are now imperative, unambiguous, actionable, and fully aligned with project best practices.
- File operation, naming, autonomy, and plan management policies are robust and enforced.
- Documentation is traceable, systematized, and free of obsolete artifacts.
- The process is now a model for future documentation and assistant-driven refactors.

No follow-up actions remain. This plan is ready for archival or deletion.
