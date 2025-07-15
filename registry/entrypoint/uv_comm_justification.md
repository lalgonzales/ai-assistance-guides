# uv_comm Integration Reference

**Related guide:** [AI_ASSISTANT_GUIDELINES.md](../../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md)

## Analysis of Main Entry Guide and UV Commands Guide

### AI_ASSISTANT_GUIDELINES.md
- This is the mandatory entrypoint and central reference for all documentation.
- It must not contain operational instructions or detailed workflows; all actionable content is in subguides.
- Validation, autonomy, and confirmation are key principles.
- For any non-trivial action, consult the relevant subguide.
- It does not explicitly mention environment management or UV commands, but directs to subguides for such topics.

### UV_COMMANDS_GUIDE.md
- This is the official subguide for dependency and environment management with UV.
- Provides basic commands (`uv sync`, `uv add`, `uv run`) and workflow examples.
- Requires imperative language and validation of operations.
- Recommends keeping `uv.lock` under version control and using `uv run` for environment commands.
- Links to the main guide and official UV documentation.

### Recommendation
- Any action related to environment and dependencies should reference `UV_COMMANDS_GUIDE.md` from the plan, log, or operational guide.
- The main entrypoint delegates environment management to this subguide, following the principle of not mixing operational instructions in the entrypoint.
- For better traceability, plans and logs should include a direct link to `UV_COMMANDS_GUIDE.md` when describing environment setup steps.

---

**Conclusion:**
- The normative flow is well structured: the entrypoint points to subguides, and the UV subguide covers all environment management needs.
- This is not a weakness, but an intentional separation of responsibilities.
- If greater visibility is needed, a note can be added to the entrypoint reminding users to consult `UV_COMMANDS_GUIDE.md` for environment topics.

## Next Steps: Improving EntryPoint Visibility

### What will be done:
1. Add a brief note in the subguides section of the entrypoint (`AI_ASSISTANT_GUIDELINES.md`) to remind that all actions related to environment and dependencies should consult `UV_COMMANDS_GUIDE.md`.
2. This improvement reinforces traceability and ensures collaborators and assistants do not overlook the UV commands guide.
3. No operational instructions will be added to the entrypoint, only a visible and normative reference.
4. Synchronize changes and document the improvement in the commit and in this reference file.

---

**Purpose:**
- Improve visibility and normative compliance regarding environment management.
- Facilitate workflow and consultation of relevant guides.
