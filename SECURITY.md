# Security Policy

This is the default security policy for every Fors Corp repository that does not ship its own `SECURITY.md`. Where a repository has one, that file wins.

## Reporting a vulnerability

Do not open a public issue for a security problem.

1. Preferred: open a private security advisory on the affected repository ("Security" tab, then "Report a vulnerability"). Private vulnerability reporting is enabled on every public Fors Corp repository.
2. Otherwise: email developer@marcfors.com with the repository name, a description, and reproduction steps.

You will get an acknowledgement, and a note when a fix ships or when we conclude the report is not a vulnerability. Please give us reasonable time to fix before disclosing publicly.

## What is enforced organization-wide

These controls are set at the organization level and enforced by GitHub, not by convention:

| Control | Scope |
|---|---|
| Default branch is pull-request only: no direct pushes, no force-pushes, no deletion, linear history, review threads resolved before merge | Every repository, with no bypass for anyone, owners included |
| Dependabot alerts and security updates, dependency graph | Every repository (enforced configuration) |
| Secret scanning with push protection, private vulnerability reporting | Every public repository |
| Actions allow-list: GitHub-owned actions, Marketplace-verified creators, and an explicit list of other action owners | Every repository |
| Fork pull requests from external contributors need approval before workflows run | Every repository |
| `GITHUB_TOKEN` defaults to read-only; workflows must request write permissions explicitly | Every repository |

Repository-specific controls (required status checks, CodeQL, dependency audits) are documented in each repository's own `SECURITY.md` or `CONTRIBUTING.md`.
