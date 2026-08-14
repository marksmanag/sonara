# AGENTS

This file describes operational guidance for project-local agents.

Purpose
- Provide concise, actionable instructions for automated agents used in this repository.

Principles
- The agent may create. The tools must verify.
- Keep human oversight: do not merge PRs automatically.

Roles
- lead-agent: plans and coordinates (human review required).
- builder-agent: implements small, well-defined changes.
- reviewer-agent: checks diffs, tests, and quality gates.

How to use
1. Read docs/ENGINEERING_WORKFLOW.md before making changes.
2. Use .agent/skills/* for project-specific guidance.
3. Always create a branch and open a PR for human review.

Unknowns / notes
- This file is intentionally short. For full workflow, see docs/ENGINEERING_WORKFLOW.md.
