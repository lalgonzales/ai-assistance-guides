######################################################################
######################################################################
# AI_ASSISTANT_GUIDELINES.md — MANDATORY ENTRYPOINT
######################################################################

## 🚦 EntryPoint: Critical Rules Checklist

**This guide is the mandatory entrypoint and central reference for all documentation. It must not contain operational instructions or workflows. All actionable content is in the subguides listed below.**

### 1. Critical Rules Checklist
- [ ] Language: All documentation, code, and scripts in ENGLISH. Plans and chat may be in SPANISH (user preference).
- [ ] Validation: All critical operations (delete, move, plan closure) must be validated and evidenced.
- [ ] Autonomy: Only act without confirmation if the action is routine, trivial, or explicitly documented. If in doubt, consult subguide or ask for confirmation.
- [ ] Confirmation: Before creating/editing outside `private/` or `docs/sistematizacion/`, ask for confirmation unless the plan specifies.
- [ ] Cleanup: Archive or delete temporary artifacts after plan closure. If you can't, document the pending item.
- [ ] Plan closure: Every plan must be formally closed and its learnings systematized.

### 2. Usage Flow
1. Read this entrypoint and apply the checklist.
2. Is the action routine, trivial, and safe? → Act.
3. If not → Consult the relevant subguide (see below) or ask for confirmation.
4. If ambiguity arises, document and resolve in the plan before acting.

### 3. Subguides and References
- [Language Policy](./LANGUAGE_POLICY_GUIDE.md)
- [Critical Operation Validation](./VALIDATION_POLICY_GUIDE.md)
- [Autonomy & Confirmation](./AUTONOMY_POLICY_GUIDE.md)
- [Plan Closure & Validation](./PLAN_CLOSURE_GUIDE.md)
- [Artifact Location](./ARTIFACT_LOCATION_GUIDE.md)
- [Plan Structure](./PLAN_STRUCTURE_GUIDE.md)
- [Commit Conventions](./CONVENTIONAL_COMMITS.md)
- [Code Quality](./CODE_QUALITY_SUBGUIDE.md)
- [Error Handling](./ERROR_HANDLING_ENTRY_TEMPLATE.md)
- [Project Guides Policy](./PROJECT_GUIDES_POLICY.md)
  _Policy for separating general and project-specific rules and guides._
- [UV Commands Guide](./UV_COMMANDS_GUIDE.md)

---

## ⚠️ Policy: No Operational Instructions
> This main guide (AI_ASSISTANT_GUIDELINES.md) must not contain operational instructions, workflows, or detailed examples. Its sole purpose is to serve as the mandatory entrypoint and reference. All actionable content must be placed in the appropriate subguides.

### Validation Rule
- Any edit to this guide must be justified in the plan and linked to a documented improvement or refactor. Unjustified edits should be flagged and reverted.

## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md).**

> **Edit registry:** See [registry/entrypoint/edits_registry.md](../registry/entrypoint/edits_registry.md) for a complete log of all changes to this guide.
