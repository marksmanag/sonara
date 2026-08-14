# The Great Academy Engineering Workflow (Canonical)

This document is the canonical Great Academy engineering workflow for Sonara. It is intended to be the repository's source-of-truth for how we plan, build, verify, and release software.

Foundational Principle
"Study the Past. Understand the Present. Build the Future."

Engineering Principle
"The agent may create. The tools must verify."

Beginner Principle
"Understand what we are building before asking the machine to build it."

1. What We Are Building
We are building a repeatable software engineering system that takes ideas through:

Idea → Plan → Architecture → Implementation → Testing → Security → Release → Maintenance

The AI is an assistant and, when properly configured, an agent. It is not the source of truth. The source of truth is the project's repository, architecture, documentation, tests, configuration, and verified behavior.

2. Core Tenets (Summary)
- GitHub is the project's memory.
- Agents work in an agent workspace (Antigravity) and must not bypass repository truth.
- Build proves compile; tests prove behavior; journeys prove user flows.
- Security is architecture, not an afterthought.

3. The Complete Architecture (Overview)
A clear separation of responsibilities exists between documentation, source, agent workspace, Android CLI (when applicable), build, tests, and release. See the repository docs and .agent/skills for project-local details.

4. Golden Development Loop
Understand → Plan → Verify → Implement → Build → Test → Inspect → Fix → Review → Merge → Release → Learn

5. Step-by-step guidance
- Step 1 — UNDERSTAND: clarify problem, users, actions, failure modes, and success criteria.
- Step 2 — PLAN: list files to change, architecture, dependencies, testing, security implications, migrations, and rollback.
- Step 3 — VERIFY THE ENVIRONMENT: inspect repository structure, tooling, SDKs (if applicable), and CI.
- Step 4 — SELECT SKILLS: install project-local or official skills needed for the task.
- Step 5 — IMPLEMENT: make the smallest safe change, reuse components, preserve behavior, and explain decisions.
- Step 6 — BUILD: run the build, observe failures, fix with minimal change, and iterate.
- Step 7 — TEST: unit, integration, UI, and Journey tests as appropriate.
- Step 8 — INSPECT: architecture, accessibility, performance, error handling, logging, dependencies, and UX.
- Step 9 — SECURITY REVIEW: identity, auth, secrets, data, transport, audit, recovery.
- Step 10 — GIT WORKFLOW: use feature/fix/chore branches, open PRs, enforce CI and reviews.
- Step 11 — QUALITY GATE: verify the checklist before merging (see PR template).
- Step 12 — MERGE & RELEASE: merge only after gates pass; prepare release notes, artifacts, signing, distribution, and monitoring.

6. Project-local knowledge
Place project-specific skills under .agent/skills/ to teach agents project rules and conventions.

7. Beginner's mental model and daily workflow
Follow the daily workflow: start by reading this document and README, plan, implement small changes, build, test, inspect, and open PRs.

8. What NOT to do
- Do not perform random AI coding without a plan.
- Do not store important decisions only in chat — preserve them in docs, ADRs, or skills.
- Do not upgrade dependencies without review and testing.

9. Documentation & Skills
- Maintain docs/ENGINEERING_WORKFLOW.md as the canonical source.
- Keep WORKFLOW_SUMMARY.md as the quick entry point for new contributors.
- Use AGENTS.md for concise agent guidance.
- Create SKILL.md files under .agent/skills/ for project-local agent instructions.

10. Unknowns and project-specific notes
- This repository currently contains documentation and a minimal set of files. The Sonara architecture, build, and test toolchain were not detected automatically — do not assume a specific build system.
- If you add code that requires a build tool, update this file and CONTRIBUTING.md with explicit commands.

11. Change management
- Make the smallest change necessary to implement a feature or fix.
- Include tests and documentation for all non-trivial changes.
- Review diffs carefully before merging.

Appendix: Quality Gate (summary)
- Problem & acceptance criteria described
- Branch named correctly
- Branch builds and CI passes
- Unit/integration tests added and passing
- Journey(s) for main flow pass
- Security considerations documented
- Documentation updated

For full context and examples, follow the Great Academy practices in this repository and consult project-local skills under .agent/skills/.
