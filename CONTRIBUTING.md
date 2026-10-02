# Contributing to Fors Corp projects

Default guidelines for every Fors Corp repository. A repository's own `CONTRIBUTING.md` overrides anything here.

## Before you start

- For anything larger than a small fix, open an issue first so the approach is agreed before the work is done.
- Read the repository's `README.md` and, where present, `CLAUDE.md` or `AGENTS.md`: they hold the standing rules the code is held to.

## Pull requests

- Default branches only move through pull requests. There is no direct push and no bypass, for anyone.
- History is linear: merge by squash or rebase. Merge commits are rejected.
- Every status check must be green. A failing check is a reason to fix the change, not to retry the check.
- Resolve every review thread before merging.
- Keep a PR to one concern. Split unrelated changes.
- Write the PR title as the changelog line you would want to read later. Several repositories enforce Conventional Commits on titles.
- Do not force-push a PR branch once review has started. Push fixup commits and let squash flatten them.

## Dependencies

- Do not add a dependency a PR does not need. If you add one, say why in the PR.
- Dependabot keeps versions current. Do not hand-bump versions in an unrelated PR.

## Workflows

- Every workflow declares an explicit `permissions:` block.
- Prefer pinning actions to a commit SHA with the version in a trailing comment.
- Only GitHub-owned, Marketplace-verified, and explicitly allow-listed actions run in this organization. If a new action is blocked, ask before adding it to the allow-list.

## Security issues

See [SECURITY.md](SECURITY.md). Never report a vulnerability in a public issue.
