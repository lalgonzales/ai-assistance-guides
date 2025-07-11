## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md).**

- This guide is only for the registry and protection of critical files in the AI Assistant project.
- For general assistant logic, always refer to the entrypoint first.

# Critical Files Registry (ARCHIVOS_CRITICOS.md)

This file IMPERATIVELY lists all files and directories that MUST NEVER be deleted, emptied, or modified without explicit justification, validation, and plan update. The AI Assistant and all collaborators MUST consult this registry before any destructive or high-impact file operation.

> **Naming Policy:**
> All naming rules for files and directories are defined in the main guide (see: File & Directory Naming Policy in AI_ASSISTANT_GUIDELINES.md). This registry inherits and enforces those rules for all critical files.

## Quick-Reference Checklist
- [ ] ALWAYS check this registry before deleting, moving, or modifying any file.
- [ ] Files listed here MUST NOT be deleted, emptied, or overwritten without explicit plan, user approval, and backup.
- [ ] Any change to this registry MUST be documented in the main plan and validated.
- [ ] If in doubt, ALWAYS ask the user before proceeding with any operation on these files.

## Protected Files/Directories
- `docs/ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md`
- `docs/ai_assistant_guides/PLAN_STRUCTURE_GUIDE.md`
- `docs/ai_assistant_guides/CRITICAL_FILES.md` (this file)
- `docs/sistematizacion/` (entire directory)
- Any file explicitly marked as critical in an active plan

## Usage
- Update this file whenever a new critical file or directory is identified.
- Reference this registry in all file operation policies and plan closure checklists.
- If a file must be removed or modified for a justified reason, document the rationale and obtain explicit approval in the plan before proceeding.

---

> **Warning:**
> The AI Assistant MUST always validate against this registry before any destructive operation. Violating this policy is considered a critical error and MUST be logged and reported in the plan.
