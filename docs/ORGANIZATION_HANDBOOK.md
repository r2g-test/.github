# r2g-test organization handbook

> Organization-wide defaults for repositories maintained under **r2g-test**. A repository may strengthen these rules locally, but should not silently weaken them.

## Purpose

`r2g-test` provides isolated repositories and fixtures for validating r2g packaging, release, installation, and compatibility workflows without risking production projects.

The `.github` repository is the canonical home for the organization profile, contribution policy, security guidance, support expectations, shared issue forms, pull-request guidance, and planning links.

## Repository expectations

Every active repository should make the following easy to discover:

- its purpose, ownership boundary, supported environments, and maturity level;
- a reproducible local-development and test command;
- the source of truth for interfaces, fixtures, and generated artifacts;
- release, rollback, deprecation, and compatibility expectations;
- links to the relevant GitHub Project and Linear project or issue.

Test repositories must clearly distinguish deterministic fixtures from generated, ephemeral, or destructive test data.

## Change workflow

1. Start from an issue, Linear item, or clearly documented maintenance objective.
2. Use a focused branch and keep unrelated work out of the pull request.
3. Explain the change, motivation, risk, validation, compatibility impact, and rollback path.
4. Run the narrowest relevant checks plus any organization-level conformance checks.
5. Resolve conflicts semantically: preserve the intent of both sides where compatible and document deliberate trade-offs.
6. Prefer squash merges for focused changes unless preserving commit structure materially helps review or auditability.

## Testing and evidence

A change is not complete merely because code was pushed. Pull requests should include enough evidence for another maintainer to reproduce the result, such as:

- exact commands and environments used;
- expected and observed outcomes;
- negative or failure-path coverage;
- artifact, fixture, or snapshot updates;
- relevant GitHub Actions runs or local-equivalent logs.

Tests in this organization should avoid hidden dependencies on personal credentials, mutable external state, or unversioned services.

## Security and data handling

Never commit credentials, tokens, private keys, production data, or sensitive logs. Use synthetic or irreversibly sanitized fixtures. Report vulnerabilities privately according to `SECURITY.md`; do not open a public issue containing exploit details.

Dependencies, actions, containers, and external fixtures should be pinned where reproducibility or supply-chain integrity matters.

## Documentation quality

Documentation is part of the deliverable. Keep examples executable, links current, headings descriptive, and assumptions explicit. Prefer short decision records for architectural or compatibility choices that future maintainers may otherwise have to rediscover.

## Planning and status

GitHub is the source of truth for code, reviews, checks, releases, and delivery evidence. Linear is the source of truth for prioritization, dependencies, sequencing, and cross-project planning. The organization GitHub Project provides the cross-repository execution view. See `PROJECTS.md` for the current routing contract.

## Organization health checklist

Review periodically:

- [ ] Organization profile accurately describes the project and its boundaries.
- [ ] Contribution, security, support, governance, issue, and PR guidance is present.
- [ ] Active repositories have owners, descriptions, topics, and maintained READMEs.
- [ ] Default branches and required checks reflect current risk.
- [ ] Stale repositories are archived or carry an explicit status notice.
- [ ] Project links resolve and completed work is reflected in both GitHub and Linear.
- [ ] Shared workflows and templates are versioned, tested, and backwards compatible.
