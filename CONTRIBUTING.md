# Contributing to Sonara

Thank you for contributing to Sonara. This document explains how to contribute, branch naming, and the project's PR quality gate.

Branch naming
- feature/<short-description>
- fix/<short-description>
- chore/<short-description>
- Use kebab-case and keep branch names short and descriptive.

Workflow
1. Understand the task and write a short plan in the PR description.
2. Create a branch (do not work directly on main).
3. Make minimal, well-tested changes.
4. Run local validation (see "Validation" below).
5. Open a Pull Request (use the template). Include the Quality Gate checklist.
6. Address review feedback. Do not merge until CI and reviews pass.

Validation
- This repository currently contains documentation and minimal source files. No build or test toolchain was detected automatically.
- If you add code that requires a build, update this file with instructions to run the appropriate build/test commands (Gradle/Maven/NPM/etc.).

Pull Requests
- Use the provided PR template. The PR must describe the problem, the plan, files changed, and include the Quality Gate checklist.

Agent guidance
- Project-local skills live under .agent/skills/. Follow the SKILL.md skeletons when adding project-specific skills.

License
- By contributing, you agree that your contributions will be licensed under the repository's license (see LICENSE).
