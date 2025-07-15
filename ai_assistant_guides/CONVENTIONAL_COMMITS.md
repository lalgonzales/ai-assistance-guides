## 🚦 MANDATORY ENTRYPOINT
**All planning, logic, and critical rules start from [AI_ASSISTANT_GUIDELINES.md](../ai_assistant_guides/AI_ASSISTANT_GUIDELINES.md).**

> **Edit registry:** See [registry/policies/conventional_commits_edits.md](../registry/policies/conventional_commits_edits.md) for a complete log of all changes to this guide.

# Conventional Commits Guide

This guide is only for commit message standards and strategy for the AI Assistant project.
For general assistant logic, always refer to the entrypoint first.

## Commit Strategy & Documentation Requirement (Best Practice)

- **Document the file groups and proposed commit messages in the plan and related logs before executing the commit.** This step is mandatory for traceability and review.
- **ALWAYS run `git status` before staging or committing to review all changes and confirm only relevant files are included. This applies to both plan-based and autonomous actions.**
- **Commits should group logical blocks of work:** Avoid committing every micro-action. Instead, commit after completing a meaningful unit of work, such as a feature, fix, refactor, or documentation update.
- **Group by type of modification:** If possible, separate unrelated changes (e.g., refactor vs. docs) into different commits.
- **Commit at milestones or after relevant progress:** Update the plan and commit when you reach a milestone, finish a block of work, or complete a cleanup/archive.
- **Use clear, conventional messages:** Always follow the format and types below for clarity and automation.

This approach improves traceability, code review, and recovery, and is required for all contributors.

---

This document describes the Conventional Commits standard for commit messages. Use this guide to ensure clear, consistent, and automatable commit history in any project.

## Commit Message Format
```
type(scope?): subject

body (optional)

footer (optional)
```

### Types
- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, etc)
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **test**: Adding or correcting tests
- **chore**: Maintenance, build, or auxiliary tool changes

### Examples
```
feat: add user authentication module
fix: correct typo in error message
chore: update dependencies
```

## Why Use Conventional Commits?
- Enables automated changelogs
- Improves collaboration and code review
- Makes project history easier to understand

> For more details, see https://www.conventionalcommits.org/en/v1.0.0/
