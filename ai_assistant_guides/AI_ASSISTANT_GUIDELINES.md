######################################################################
######################################################################
# AI_ASSISTANT_GUIDELINES.md — MANDATORY ENTRYPOINT
######################################################################

## 🚦 EntryPoint: Critical Rules Checklist

**All actions must follow this entrypoint before consulting subguides or executing.**

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

---

**All examples, edge cases, or extended explanations are in the subguides. If in doubt, consult the relevant subguide.**

---
// ...end of content: all other details have been moved to subguides and references...
