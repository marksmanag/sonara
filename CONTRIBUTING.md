# Contributing to Sonara

This document explains the recommended workflow and expectations for contributions to the Sonara repository.

Principles

- Document before implement: Research, product requirements, UX, and ADRs must exist before substantial implementation.
- Small, reviewable changes: Keep PRs focused and small.
- Tests and documentation: Changes that affect behavior must include tests and documentation updates.
- Respect creators: Follow the Sonara Constitution when designing features that affect artists or listeners.

Branch strategy

- main: stable documentation & production-ready artifacts.
- docs/*: documentation-focused branches and PRs.
- feat/*: feature work (requires an ADR or design doc if large).
- fix/*: bug fixes.
- ci/*: CI/configuration changes.

Commits and PRs

- Use conventional commit-style messages where practical (e.g., "docs: ...", "feat: ...", "fix: ...").
- Describe why the change is made and link related ADRs, issues, or research.
- Include a changelog entry for user-visible changes.

Code review

- PRs require at least one approving review from a maintainer.
- Reviewers should verify documentation, tests, and that the change follows the Sonara Constitution.

Documentation

- Every subsystem must include a README explaining purpose and maintenance expectations.
- Major decisions must have an ADR in docs/decisions/.

Testing

- Include unit and/or integration tests when applicable.
- Add contract tests for cross-service changes.

Security

- Do not commit secrets. Use secure secret management.
- Report vulnerabilities per SECURITY.md.

Architecture & ADRs

- Significant architectural choices must be captured as ADRs in docs/decisions/.
- ADRs must include context, options considered, and consequences.

Getting help

Open an issue with the "help wanted" label or contact a maintainer listed in repository metadata.
