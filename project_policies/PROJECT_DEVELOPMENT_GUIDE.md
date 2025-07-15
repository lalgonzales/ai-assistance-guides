# Project-Specific Development Guide

This file documents rules, conventions, and workflows that apply ONLY to this repository and are complementary to the main AI guide.

## Archive Policy
- All improvement or development plans created in this repository, according to their relevance, must be stored in `ai_assistant_guides/plan_archive/`.

## Documentation Versioning & Commit Policy
- In this repository, all commits (except those with type `ci`) must trigger a version bump in the project. This applies to documentation, normative guides, and code changes.
- Use commit types such as `feat`, `fix`, or `BREAKING CHANGE` for all changes that should be reflected in the project version.
- Only commits with type `ci` (continuous integration or automation) are exempt from triggering a version bump.
- Each commit represents a new version or revision of the documentation, ensuring traceability and historical record.
- The `pyproject.toml` version may be updated to reflect major documentation milestones or significant changes in project structure, not just code.
- All project-specific guides and registries must follow this logic, using commit history as the primary versioning mechanism for documentation.
- For code releases, synchronize documentation versioning with the project version in `pyproject.toml` when appropriate.
- Always document the commit plan and messages in the plan or logs before executing the commit.
- Review the [Conventional Commits Guide](../ai_assistant_guides/CONVENTIONAL_COMMITS.md) for message format and workflow.

## Plan Archiving and Cleanup Workflow
1. Evaluate if the plan deserves to be archived (relevance, learning, or historical value).
2. If it should be archived:
   - Move the plan from `private/planning/` to `ai_assistant_guides/plan_archive/`.
   - Delete all temporary files created during the plan (logs, scripts, etc.).
   - Commit with a clear message, e.g.: `archive(plan): move and archive completed plan <name>`
3. If it should NOT be archived:
   - Delete the plan and all related temporary files.
   - Commit with a cleanup message, e.g.: `chore(cleanup): remove temporary plan and artifacts <name>`

This ensures traceability, cleanliness, and compliance with the archive and temporary file policy.
