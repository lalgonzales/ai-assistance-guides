# ARTIFACT_LOCATION_GUIDE.md


## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md).**

- This guide is only for artifact location and organization policy in the AI Assistant project.
- For general assistant logic, always refer to the entrypoint first.


## Artifact Location

- Generalizable knowledge and reusable patterns → `docs/sistematizacion/`
- Temporary scripts, logs, and diagnostics → `private/` (this folder is excluded from git via `.gitignore` and is for local, non-versioned work only; do NOT synchronize or commit files from `private/`)
- Finalized plans → summarize in systematization and archive/delete from `private/`

### Example
- A one-time troubleshooting script: `private/`
- An onboarding checklist: `docs/sistematizacion/`

---
