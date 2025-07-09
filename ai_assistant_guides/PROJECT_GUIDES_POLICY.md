# Project Guides Policy

## General Principle

- The main AI guide and templates are designed to be general, portable, and must NOT be contaminated with project-specific rules, workflows, or files.
- Any project-specific rule, workflow, or archive policy MUST be documented in a separate `project_guides/` folder, never in the main guide.
- This ensures that the core guide remains clean, portable, and easy to update as a submodule in other repositories.

## How to Use

- If your project requires local rules, exceptions, or workflows not covered by the general guide, document them in `project_guides/`.
- Never modify the main guide or templates for project-specific needs; always extend via `project_guides/`.
- Reference this policy in your project-specific guides as needed.

---

_This file defines the policy for separating general and project-specific logic when using the AI guide as a base or submodule._
