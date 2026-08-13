# Contributing

Thanks for taking an interest in our work. This guide applies to all public repositories in the Harrison Ward Technology organization.

## Before you start

- **Open an issue first.** For anything beyond a typo fix, describe what you want to change and why before writing code. It saves you from building something we cannot merge
- **Check open issues and pull requests** so you are not duplicating work in progress
- Issues labeled `good first issue` are the easiest place to start

## Reporting a bug

Open an issue and include:

- What you expected to happen
- What actually happened
- Steps to reproduce
- Your environment: operating system, runtime version, and the repo version or commit

## Suggesting a feature

Open an issue describing the problem you are trying to solve, not just the solution you have in mind. Context helps us find the right fix.

## Pull requests

1. Fork the repository and create a branch from `main`
2. Name the branch descriptively: `fix/backup-timeout` or `feat/add-rmm-export`
3. Make your change, and keep it focused. One concern per pull request
4. Add or update tests if the repo has a test suite
5. Update the README or docs if behavior changed
6. Run any linters or formatters the repo uses
7. Open the pull request against `main` and link the related issue

### Commit messages

Use a short imperative subject line under 72 characters.

```
Add retry logic to backup verification job

The verification job failed on transient network errors instead of
retrying. This adds three retries with exponential backoff.

Fixes #42
```

### What we look for in review

- The change does what the issue described
- It does not break existing behavior
- Code matches the style already in the repository
- No secrets, credentials, client names, or client data anywhere in the diff

## Never commit

- API keys, tokens, passwords, or connection strings
- Client names, client IP ranges, hostnames, or any client-identifying data
- Internal network diagrams or infrastructure details
- Customer data of any kind, real or sampled

If you commit a secret by accident, tell us immediately. Do not just delete it in a follow-up commit. The history keeps it.

## Code of conduct

Be direct, be respectful, assume good faith. We remove people who cannot manage that.

## Licensing

By contributing, you agree your contribution is licensed under the same license as the repository.

## Questions

Open a discussion or an issue. For anything sensitive, see [SECURITY.md](SECURITY.md).
