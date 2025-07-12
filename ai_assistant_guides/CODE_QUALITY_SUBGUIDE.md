## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md).**

This guide is only for code quality and refactoring rules for the AI Assistant project.
For general assistant logic, always refer to the entrypoint first.

# Code Quality & Refactoring Subguide for AI Assistant

> **Purpose:**
> This subguide provides IMPERATIVE rules and best practices for code quality and refactoring. All critical rules use MUST, NEVER, or ALWAYS. The AI Assistant and collaborators MUST follow these to maintain a clean, modular, and maintainable codebase.

---

## Quick-Reference Checklist

- [ ] All code, comments, documentation, workflow step names, and commit messages MUST be in ENGLISH by default.
- [ ] Functions/classes MUST have a single, well-defined responsibility.
- [ ] Code MUST be modular, readable, and simple.
- [ ] Repeated logic MUST be extracted into reusable functions/modules.
- [ ] All critical logic MUST be covered by tests.
- [ ] Code quality tools (linters, formatters, etc.) MUST be used before commit.
- [ ] Documentation and docstrings MUST be updated as needed.
- [ ] After any significant change, the plan MUST be updated with the next step.

---

## Key Principles (Imperative)

- **Modularity:**
  - Functions and classes MUST have a single, well-defined responsibility.
  - Large, monolithic functions MUST be avoided—ALWAYS prefer small, composable units.

- **Readability:**
  - Names for functions, variables, and classes MUST be descriptive.
  - Concise comments MUST be added where logic is non-obvious.
  - Code and documentation MUST be in ENGLISH by default.

- **Simplicity:**
  - Logic MUST be simple and clear; NEVER use clever or overly abstract solutions.
  - Dead code and unnecessary complexity MUST be removed.

- **Reusability:**
  - Repeated logic MUST be extracted into reusable functions or modules.
  - Code duplication MUST be avoided.

- **Testing:**
  - All critical logic MUST be covered by tests.
  - Tests MUST be added or updated when refactoring.


- **Pre-commit & Tooling:**
  - Pre-commit hooks and code quality tools (e.g., linters, formatters) MUST be used to enforce standards automatically.
  - Commitizen MUST be configured with a plugin (e.g., cz_changeup) that supports extracting both the commit title and description for changelogs, to ensure complete traceability and context in release notes.
  - The [tool.commitizen.changeup] section in `pyproject.toml` MUST define all commit types and bump rules explicitly, to guarantee consistent versioning and changelog generation.
  - All contributors MUST write commit messages with a clear title and an informative description, as both will be included in the changelog.
  - Additional tools (e.g., black, flake8, isort, mypy) MUST be integrated as needed.
  - For CI/CD jobs, ALWAYS install critical tools (e.g., Commitizen, cz plugins) explicitly in the workflow, not only from `pyproject.toml`, to ensure reproducibility and control.
  - **ALWAYS run `git status` before staging or committing to review all changes and confirm only relevant files are included. This applies to both plan-based and autonomous actions.**

- **Documentation:**
  - Docstrings and README sections MUST be updated or added as needed.
  - The intent and usage of complex functions or modules MUST be documented.

- **Incremental Improvement:**
  - Refactor opportunistically—ALWAYS improve code quality as you touch related areas.
  - Large, risky rewrites MUST be avoided unless necessary.
  - Update or add docstrings and README sections as needed.

- **Incremental Improvement:**
  - Refactor opportunistically—improve code quality as you touch related areas.
  - Avoid large, risky rewrites unless necessary.

---



## Workflow for Code Quality Jobs (Imperative)

1. Review the relevant plan and this subguide before any code quality or refactor job.
2. Identify and document areas of high complexity, duplication, or unclear logic.
3. Propose or execute targeted refactors, ALWAYS following the principles above.
4. Validate all changes with tests and code quality tools before reporting completion.
5. Update documentation and systematize new patterns if needed.
6. The plan MUST be updated after each significant change; use sub-plans for large refactors.
7. **MANDATORY COMMIT WORKFLOW:**
   - ALWAYS run `git status` before staging or committing to review all changes.
   - Decide how to group changes into atomic, clear, and policy-compliant commits. NEVER use `git add .` to stage everything at once.
   - Stage and commit only validated, logically grouped changes with clear, descriptive commit messages (title and body), following the conventions in this subguide.
   - Example:
       - `chore(ci): add GitHub Actions workflow for version bump`
       - `docs(project): add project-specific development guide`
   - Reference the main guide for further details and rationale.

## Commit Workflow and Grouping
- Before executing any commit, review changes with `git status` and group only relevant files.
- Document the file groups and proposed commit messages in the plan and corresponding log.
- This ensures traceability, auditability, and compliance with project standards.

## Bidirectional Traceability Policy
- Any log or artifact generated during a code quality job must link back to the originating plan/log, and the plan/log must register the link to the artifact.
- This guarantees traceability, reviewability, and compliance with project standards.

**Example:**
- In the log: “This log is linked to the plan step X. Artifact generated: [artifact.md](../path/artifact.md)”)

