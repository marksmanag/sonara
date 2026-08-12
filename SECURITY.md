# Security

Sonara treats security and user protection as first-class concerns. This document outlines reporting and core security principles for the repository and project.

Core principles

- Least privilege: Grant minimal permissions required.
- Secure defaults: Opt-in features are explicit; defaults are conservative.
- Defense in depth: Multiple layers of protection where appropriate.
- Auditability: Log significant events and keep immutable audit trails when required.
- Privacy by design: Minimize data collection and default to private.

Reporting vulnerabilities

If you discover a security vulnerability affecting Sonara, please report it responsibly:

1. Open a private, confidential issue (or use the GitHub security advisory flow) and mark it as a security report.
2. If you prefer email, send details to security@sonara.invalid (replace with official address when available).
3. Provide steps to reproduce, impact assessment, and any suggested mitigations.

Secrets management

- Never commit API keys, private keys, passwords, or tokens.
- Use environment variables and approved secret stores for CI and deployments.

Dependencies

- Track third-party dependency provenance and license information before adoption.
- Use automated dependency scanning in CI where practical.

Disclosure policy

- Sonara will acknowledge reporters and coordinate a responsible disclosure timeline.
- Do not publicly disclose vulnerabilities until a coordinated release or mitigation is available.
