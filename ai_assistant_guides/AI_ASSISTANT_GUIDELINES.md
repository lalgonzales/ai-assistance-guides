- For any conventions, restrictions, or workflows that are unique to this repository (not general-purpose), you MUST create a `project_guides/` directory at the root of the repository.
- The main file for project-specific rules is `project_guides/PROJECT_DEVELOPMENT_GUIDE.md`.
- This file MUST be versioned (not in `private/`) and referenced from this main guide.
- Use this file to document:
  - English-only policy for plans (if stricter than the general guide)
  - Plan lifecycle and closure rules specific to the project
  - Any exceptions, additional conventions, or local workflows
- The `PROJECT_DEVELOPMENT_GUIDE.md` MUST include a reference to the repository and be kept in sync with the main guidelines.
- If you start a new project or fork, create or update this file to reflect project-specific needs.
- Always include the repository URL in the header of each project-specific guide for traceability:

  Main repository: https://github.com/lalgonzales/ai-assistance-guides

---
---

# Development & AI Assistant Quick Reference Guide

## Quick-Reference Checklist

- [ ] All documentation, code comments, and scripts MUST be in ENGLISH by default.
- [ ] Planning documents and chat MAY be in SPANISH (user preference).
- [ ] Systematized knowledge and reusable patterns MUST go in `docs/sistematizacion/`.
- [ ] Temporary scripts, logs, and diagnostics MUST remain in `private/` during active work.
- [ ] NEVER move temporary or highly specific artifacts to the main documentation.
- [ ] ALWAYS ask for confirmation before creating documentation outside the systematization area, unless routine, trivial, or plan-driven according to this guide.
- [ ] All plans MUST be formally closed, with learnings transferred and artifacts cleaned up.
- [ ] The assistant MUST always create or update a plan with the next concrete step after any significant change.
- [ ] The assistant MUST use imperative language (MUST, NEVER, ALWAYS) for all critical rules.
- [ ] After each block of work or milestone, the assistant MUST always propose or execute the next concrete step as defined by the plan or guide, or close the plan if all objectives are met. The assistant MUST NEVER leave the process open-ended or ask the user what to do next if the plan or guide already determines the next step.

---

> **LANGUAGE POLICY (MANDATORY):**
> - All documentation, code comments, and scripts MUST be in ENGLISH by default, for normalization and broader accessibility.
> - Planning documents (e.g., plans in `private/planning/`) and general chat/user–AI interactions MAY be in SPANISH.
> - If there is any doubt, ALWAYS prefer ENGLISH for documentation and scripting, but SPANISH is acceptable for planning and interactive chat unless otherwise specified.
> - If the user writes in Spanish in chat or planning, the assistant MAY reply in Spanish unless the user requests English or the context requires it.
> - This rule is IMPERATIVE and OVERRIDES any other ambiguity. The assistant must always check and apply this policy before any output or file creation.
>
> **Examples:**
> - Documentation file (`README.md`, `docs/`, code comments): ENGLISH ONLY
> - Script or code: ENGLISH ONLY
> - Plan in `private/planning/`: SPANISH or ENGLISH (user preference)
> - General chat: SPANISH or ENGLISH (user preference)

---


## File & Directory Naming Policy (MANDATORY)
- All file and directory names MUST be in ENGLISH by default, for normalization, clarity, and cross-team accessibility.
- Names in SPANISH are ONLY permitted for localized documentation or user-facing content, and MUST be explicitly justified in the plan or documentation.
- If in doubt, ALWAYS prefer ENGLISH for naming any file or directory, especially for critical, shared, or long-term artifacts.
- This policy applies to all documentation, scripts, code, plans, and critical files.

## Private Directory Policy (MANDATORY)
- The `private/` directory MUST be created at the root of the repository.
- All temporary scripts, logs, diagnostics, and planning documents MUST be placed inside `private/` during active work.
- The `private/` directory and all its contents MUST be included in the `.gitignore` file to prevent accidental publication.
- Only finalized, systematized, or public documentation may be moved out of `private/` after validation and closure.

---

> **MANDATORY CONTINUATION POLICY:**
> - After any significant change, review, or clarification, the assistant MUST always create or update a plan in `private/planning/` summarizing the next concrete step(s).
> - The assistant MUST NEVER leave the process open-ended or with multiple possible continuations. There must always be a single, actionable next step, either as a plan or as a direct action.
> - The plan MUST be used as a reference and record of key advances, decisions, blockers, and learnings—not as a log of every micro-action. Updates to the plan SHOULD be made at the end of work blocks, milestones, or when there is relevant progress, not after every minor step.
> - The priority is to focus on development and problem-solving, using the plan for strategic documentation and traceability.
> - After each block of work or milestone, the assistant MUST always propose or execute the next concrete step as defined by the plan or guide, or close the plan if all objectives are met. The assistant MUST NEVER ask the user what to do next if the plan or guide already determines the next step.
> - Example: After completing a block of work or achieving a milestone, update the plan with key outcomes, decisions, and next steps. Avoid interrupting productive flow for minor updates.

---

- All documentation, guides, and plans must be modular, actionable, and kept in sync with the codebase.

---




## Project-Specific Development Guide

For all conventions, restrictions, and workflows that apply only to the development and maintenance of this repository—including the English-only policy for plans and the plan lifecycle—see [`project_guides/PROJECT_DEVELOPMENT_GUIDE.md`](../project_guides/PROJECT_DEVELOPMENT_GUIDE.md) (included in the repository for all contributors).

---

---


## About Tooling, Commits, and Changelog

For details on code quality tools, commit conventions, and changelog generation—including the use of Commitizen with plugins for full commit message extraction—refer to the [Code Quality & Refactoring Subguide](./CODE_QUALITY_SUBGUIDE.md). All technical decisions, justifications, and workflow improvements are documented there to keep this main guide lightweight and focused.
- Use subguides and templates for details, examples, and best practices.
- Always close plans with robust validation, documentation update, and systematization.
- **All code changes MUST pass pre-commit hooks and code quality tools before being considered valid or complete.**
- **If any pre-commit hook or code quality tool fails, the assistant MUST pause, report, and correct before proceeding.**
- **AI Assistant responses and actions must always be guided by the current plan and this guide.**
- **Avoid excessive documentation; prefer systematization and updating guides/templates.**
- **MANDATORY COMMIT WORKFLOW:**
  1. Before staging or committing, ALWAYS run `git status` to review all staged and unstaged changes.
  2. Review and decide how to group changes into atomic, clear, and policy-compliant commits. NEVER use `git add .` to stage everything at once.
  3. Stage and commit only validated, logically grouped changes with clear, descriptive commit messages (title and body), following the conventions in the [Code Quality & Refactoring Subguide](./CODE_QUALITY_SUBGUIDE.md).
  4. If in doubt, consult the plan and guides before committing.
- **Rule:** Before consulting the user, validate the plan and the guide, and end the message with: “Do you confirm the next steps or should we adjust something?”

---

## How to Use This Guide
- Use this guide as a navigation hub.
- For any task, start here and follow the links to detailed subguides and templates.
- Propose improvements as you learn.
- **When in doubt, the assistant will act as follows:**
  1. Review the active plan and this guide.
  2. Propose or execute only the minimum documentation or systematization needed.
  3. Prefer updating subguides or templates over creating new files.
  4. Always ask for confirmation before generating new documentation beyond the systematization area.

---

+# Autonomy Principle (MANDATORY)
+- The assistant has full autonomy to execute routine, trivial, or well-documented actions as defined in this guide, without asking for user confirmation.
+- User confirmation is ONLY required for ambiguous, high-impact, or undocumented actions.
+- When in doubt, the assistant MUST consult the user, but should default to autonomy for all actions explicitly covered by the guide or an active plan.

---

## Confirmation Before File Creation

- The assistant MUST ask for user confirmation before creating or editing files in official documentation or systematization areas (e.g., `docs/`, `docs/sistematizacion/`), unless the action is a direct, routine result of a validated plan or guide.
- For temporary, routine, or cleanup actions in `private/`, the assistant may proceed autonomously without confirmation.
- If there is any ambiguity or the action is critical, ALWAYS ask for confirmation.
+
+> **Note:** For routine, trivial, or well-documented actions (such as renaming files to comply with the naming policy, cleaning up temporary files, or updating checklists), the assistant SHOULD act autonomously and only consult the user if the action is not clearly covered by this guide or an active plan.

**Example:**
- Creating a new plan in `private/planning/` as part of a workflow: NO confirmation needed.
- Generating a temporary script for diagnostics in `private/`: NO confirmation needed.
- Editing `README.md` or adding a new guide in `docs/`: ALWAYS ask for confirmation unless it’s a direct result of a validated plan.
- Performing a cleanup of old logs in `private/`: NO confirmation needed if the objective is clear and routine.

## Key Topics & Subguides
- **Plan Structure & Best Practices:**
  - See [PLAN_STRUCTURE_GUIDE.md](./PLAN_STRUCTURE_GUIDE.md) for plan structure, checklists, and closure criteria.
- **Commit Conventions:**
  - [CONVENTIONAL_COMMITS.md](./CONVENTIONAL_COMMITS.md)
- **Validation & Testing:**
  - [VALIDATION_LOG_TEMPLATE.md](./VALIDATION_LOG_TEMPLATE.md)
- **Planning & Task Management:**
  - [PLANNING_TASK_TEMPLATE.md](./PLANNING_TASK_TEMPLATE.md)
- **Systematization & Project-Specific Knowledge:**
  - [../sistematizacion/](../sistematizacion/)
- **Error Handling:**
  - [ERROR_HANDLING_ENTRY_TEMPLATE.md](./ERROR_HANDLING_ENTRY_TEMPLATE.md)
  - [ERROR_HANDLING_ITERATIVO_TEMPLATE.md](./ERROR_HANDLING_ITERATIVO_TEMPLATE.md)
- **Code Quality & Refactoring:**
  - [CODE_QUALITY_SUBGUIDE.md](./CODE_QUALITY_SUBGUIDE.md)
- **Other Templates & Guides:**
  - [README_TEMPLATES.md](./README_TEMPLATES.md)
- **Spanish Documentation:**
  - [docs/es/](../../docs/es/)

---

## Plan Closure and Validation

- All plans MUST be formally closed when their objectives are met.
- Upon closure, the assistant MUST:
  1. Validate that all code and logic changes are tested and documented.
  2. Review and update all relevant documentation and READMEs.
  3. Systematize new patterns or lessons in `docs/sistematizacion/` if generalizable.
  4. Propose improvements to guides/templates if needed.
  5. Summarize the closure in the plan, noting any follow-up actions.
  6. Archive or delete the plan from `private/planning/` once no longer needed.
- Use this checklist for every plan closure:
  - [ ] All code and logic changes validated with robust tests
  - [ ] All documentation and READMEs reviewed and updated
  - [ ] New patterns/lessons systematized
  - [ ] Improvements to guides/templates proposed if needed
  - [ ] Plan formally closed and summarized
  - [ ] Plan archived or deleted from `private/planning/`

**Example:**
- After completing a refactor, update the plan with a summary, ensure all learnings are systematized, and archive/delete the plan from `private/planning/`.

---

> **Logging Standard:** All detailed logs of debugging/testing cycles must go in a dedicated log file linked from the main plan. The main plan should only contain the checklist, conclusions, and links. See [PLAN_STRUCTURE_GUIDE.md](./PLAN_STRUCTURE_GUIDE.md#logging--plan-structure-standard-2025-07-06).
>
> For detailed examples, templates, and best practices, always refer to the linked subguides.

---

## Documentation and Artifact Location

- Systematized knowledge and reusable patterns MUST go in `docs/sistematizacion/`.
- Temporary scripts, logs, and diagnostics MUST remain in `private/` during active work.
- NEVER move temporary or highly specific artifacts to the main documentation.
- Use the following checklist to determine file location:
  - [ ] Is it generalizable, reusable, or onboarding value? → `docs/sistematizacion/`
  - [ ] Is it a temporary script, log, or diagnostic? → `private/`
  - [ ] Is it a finalized plan or learning? → Summarize in systematization, archive or delete from `private/`.

---

## Systematization vs. Temporary Artifacts

- Systematization refers to knowledge, patterns, or documentation that is generalizable, reusable, or valuable for onboarding and long-term reference.
- Temporary artifacts are scripts, logs, diagnostics, or notes created for short-term, specific, or experimental purposes.
- The assistant MUST always:
  - Move systematized knowledge and reusable patterns to `docs/sistematizacion/`.
  - Keep temporary artifacts in `private/` during active work.
  - Summarize finalized plans or learnings in systematization, then archive or delete from `private/`.
- Use the following decision flow:
  1. Is the artifact generalizable, reusable, or valuable for onboarding? → Systematize in `docs/sistematizacion/`.
  2. Is it a temporary script, log, or diagnostic for a specific task? → Keep in `private/`.
  3. Is it a finalized plan or learning? → Summarize in systematization, archive/delete from `private/`.
- If in doubt, ask the user for clarification before moving or deleting artifacts.

**Example:**
- A troubleshooting script for a one-time bug: keep in `private/`.
- A reusable SQL template or onboarding checklist: move to `docs/sistematizacion/`.
- A completed plan with valuable lessons: summarize in systematization, then archive/delete the original plan.

---

## Execution and Output Tracking

- The assistant MUST always track the output of scripts, tests, or commands it executes.
- Outputs and results MUST be reviewed and, if relevant, summarized or logged for traceability.
- The assistant MUST always provide actionable feedback or next steps based on execution results.
- This ensures continuous progress and clear follow-up on all actions.

**Example:**
- After running a test suite, summarize the results and propose fixes or next steps if failures are found.
- When executing a script, log the output in a dedicated file if it is relevant for debugging or traceability.

---


## File Operation Validation & Terminal Usage Policy (REINFORCED)



> **MANDATORY & REINFORCED:**
> - All file deletions, moves, or other critical file operations MUST be validated immediately after execution.
> - The assistant MUST NEVER report success unless the operation is confirmed complete by showing explicit evidence (e.g., output of `ls`, `find`, or search result showing the file is gone).
> - If the API fails, the assistant MUST use terminal commands (with explicit user approval) and MUST show the output as evidence.
> - If the file still exists after all attempts, the assistant MUST notify the user, document the file for manual cleanup, and NEVER claim success.
> - It is STRICTLY FORBIDDEN to report success based only on intent or command execution without validation.
> - This rule is IMPERATIVE and OVERRIDES any ambiguity or shortcut.

- If a file cannot be deleted or moved via the standard API, the assistant MAY propose or execute the required operation using a terminal command (e.g., `rm`, `mv`) **with explicit user approval**. This is permitted only for safe, project-related actions.
- The assistant MUST NEVER use the terminal for any destructive, malicious, or system-damaging actions, and MUST always act in good faith and within the project’s scope.
- If a file still cannot be deleted or moved (e.g., due to editor locks or system restrictions), the assistant MUST notify the user, propose alternative actions (such as manual removal or closing the file in the editor), and document the unresolved file in the plan's cleanup section.
- After plan closure, all temporary or intermediate files MUST be validated as removed or archived. Any that remain MUST be listed for manual follow-up in the plan's cleanup checklist.

**Quick Checklist (REINFORCED):**
- [ ] Validate every file operation (list/search to confirm result)
- [ ] Use terminal commands only with user approval if API fails
- [ ] NEVER perform destructive/system-damaging actions
- [ ] Notify user and document in plan if operation cannot be completed
- [ ] After plan closure, confirm all cleanup; list unresolved files for follow-up

**Example (REINFORCED):**
> After deleting a file, the assistant MUST show the result of listing or searching the directory to confirm it is gone. If the file is still present, the assistant MUST notify the user and document it for manual removal. Only when the file is demonstrably absent may the assistant report success.
> After deleting a file, list the directory to confirm it is gone. If still present, notify the user and suggest closing the file in the editor or removing it manually. After plan closure, check that all files marked for cleanup are actually gone; if not, document them for follow-up in the plan. If a file cannot be deleted via the API, propose or execute a safe terminal command (with user approval) to complete the operation.

**See also:** Use the main plan's cleanup checklist to track and document any unresolved file operations for traceability.
