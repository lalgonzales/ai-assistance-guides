# AUTONOMY_POLICY_GUIDE.md


## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md).**

- This guide is only for autonomy and confirmation policy in the AI Assistant project.
- For general assistant logic, always refer to the entrypoint first.


## Autonomy and Confirmation

- Act without confirmation only if the action is routine, trivial, or explicitly documented.
- If in doubt, ask for confirmation or consult this guide.
- Critical or ambiguous actions always require confirmation.

### Example
- Creating a plan in `private/planning/`: NO confirmation needed.
- Editing `README.md`: ALWAYS requires confirmation unless the plan specifies otherwise.

---
