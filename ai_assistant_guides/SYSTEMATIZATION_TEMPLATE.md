## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md).**

- This template is only for documenting systematization in development projects for the AI Assistant.
- For general assistant logic, always refer to the entrypoint first.

# Systematization Template for Development Projects

This template MUST be used to document and systematize processes, decisions, patterns, and lessons learned in any development project. All documentation MUST follow the AI Assistant Guidelines:
- Use imperative, unambiguous language (MUST, NEVER, ALWAYS).
- Name files and directories in English by default, following the naming policy.
- Validate and document all file operations and changes.
- Ensure autonomy in routine documentation and cleanup actions.
- Archive or delete obsolete files after robust validation.

---

## 1. Key Decisions
- List here the most important technical decisions made during the project.
- Example: "Removed the --all option from the CLI to avoid overload and facilitate quick testing."

## 2. Testing and Validation Patterns
- Describe patterns and best practices for testing, validation, and automation.
- Example: "Automated runner to execute main commands and collect logs."

## 3. Validation Log Template
```
Date: YYYY-MM-DD
Responsible: <name>

### Command executed
<example command>

### Result
- Finished successfully?: Yes/No
- Files generated: <list files>
- Relevant logs:
  <key log fragments>
- Issues found:
  <describe bugs, errors, improvements>
- Observations:
  <additional notes>
```

## 4. Lessons Learned
- Centralize relevant learnings for the team and future projects here.
- Example: "Centralizing active planning and cleaning obsolete files improves traceability."

## 5. Iterative Development
- Explain the iterative approach and how improvement cycles are documented.
- Example: "Each important change is documented in a private plan and consolidated in technical documentation."

## 6. References and Key Files
- List critical files, main scripts, and documentation paths.
- Example: `scripts/smart_sync.py`, `private/planning/`, `docs/ai_assistant_guides/`

---

## 🚨 MANDATORY ACTION
Upon completing a systematization log:
1. Save the completed log in `private/systematization_logs/`.
2. Add a link to the log in the corresponding plan or log document.

These steps are required for traceability and compliance with project standards.


> Adapt and expand this template as needed for your project, but DO NOT remove the imperative language or the autonomy, naming, and validation policies. Use it as a base to systematize and transfer knowledge in development teams.
