# Contributing to r2g-test

Thank you for helping improve the r2g test ecosystem. Contributions should make packaging and release behavior easier to reproduce, diagnose, and trust.

## Before starting

- Search existing issues and pull requests for related work.
- For behavior changes, open or reference an issue that describes the expected outcome and compatibility impact.
- Keep production credentials and private data out of test repositories.

## Development workflow

1. Fork or branch from the default branch.
2. Make one coherent change per pull request.
3. Add or update deterministic tests and fixtures.
4. Run the repository's documented formatter, linter, unit tests, and relevant integration tests.
5. Update documentation when commands, fixtures, APIs, or expected behavior change.
6. Open a pull request using the shared template and include reproducible validation evidence.

## Test design

Prefer tests that are deterministic, isolated, and explicit about prerequisites. When testing external services, provide a local substitute, recorded fixture, or clearly marked opt-in integration path. Clean up temporary resources and avoid relying on mutable global state.

## Commits and pull requests

Use clear, imperative commit messages. The pull request description should cover motivation, scope, risk, compatibility, validation, and rollback. Small reviewable changes are preferred over broad refactors that mix unrelated concerns.

## Reviews and merges

Address review feedback with code or a documented rationale. Resolve conflicts by understanding both branches' intent rather than choosing one side mechanically. Maintainers may squash-merge focused pull requests after required checks pass.

By contributing, you agree to follow the organization Code of Conduct and security policy.
