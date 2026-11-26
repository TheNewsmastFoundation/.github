# Contributing

This is the default contribution guide for repositories in
TheNewsmastFoundation. A repository's own `CONTRIBUTING.md` takes precedence
and covers its setup, test and release steps.

## Workflow

1. Branch from the default branch using a short prefix:
   `feat/…`, `fix/…`, `chore/…`, `docs/…`.
2. Keep each pull request focused on one change.
3. Open a pull request and fill in the template. Link the issue it closes
   (for example `Closes #123`).
4. At least one approving review is required before merge. Reviewers are
   assigned automatically from `CODEOWNERS`.
5. All required checks must pass. Do not merge on red CI.
6. Use **Squash and merge**. The head branch is deleted automatically.

## Commit messages

Use [Conventional Commits](https://www.conventionalcommits.org/):
`feat: …`, `fix: …`, `chore: …`, `docs: …`, `refactor: …`, `test: …`.

## Dependencies

Dependabot opens grouped update PRs weekly. Review and merge them within two
weeks; security updates take priority over feature work.

## Secrets

Never commit credentials, API keys, `.env` files or signing keys. Use GitHub
Actions secrets or environment secrets. If a secret is committed, rotate it
immediately and tell a maintainer; removing it from history is not enough.

## Security

Report vulnerabilities privately as described in
[SECURITY.md](https://github.com/TheNewsmastFoundation/.github/blob/main/SECURITY.md).
