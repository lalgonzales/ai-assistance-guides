# Project-Specific Development Guide

This file documents rules, conventions, and workflows that apply ONLY to this repository and are complementary to the main AI guide.

## Archive Policy
- All improvement or development plans created in this repository, according to their relevance, must be stored in `ai_assistant_guides/plan_archive/`.

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
