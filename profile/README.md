<div align="center">

# r2g-test

**Isolated, reproducible validation for r2g packaging and release workflows.**

[Repositories](https://github.com/orgs/r2g-test/repositories) · [Organization handbook](../docs/ORGANIZATION_HANDBOOK.md) · [Contributing](../CONTRIBUTING.md) · [Security](../SECURITY.md)

</div>

## What belongs here

This organization hosts test repositories, fixtures, and compatibility scenarios used to verify r2g behavior without placing production projects at risk. Repositories should make their test boundary, prerequisites, cleanup behavior, and expected outcomes explicit.

## Engineering principles

- Prefer deterministic, isolated tests over hidden dependencies on mutable services.
- Use synthetic or irreversibly sanitized fixtures; never commit production data or credentials.
- Pin dependencies and actions where reproducibility or supply-chain integrity matters.
- Treat failure paths, cleanup, compatibility, and rollback as first-class behavior.
- Keep changes reviewable and resolve conflicts semantically rather than selecting one side mechanically.
- Preserve evidence: commands, environments, expected results, observed results, and relevant CI runs.

## Start contributing

Read the [organization handbook](../docs/ORGANIZATION_HANDBOOK.md) and [contribution guide](../CONTRIBUTING.md), then open a focused issue or pull request in the repository that owns the behavior. Use the shared issue forms so maintainers receive a reproducible report.

For vulnerabilities, follow the [security policy](../SECURITY.md) and report privately.

<!-- org-project-routing:start -->
## Planning and delivery

- [GitHub Project: r2g-test-project](https://github.com/orgs/r2g-test/projects/1)
- [Linear planning project](https://linear.app/denman/project/githubcomr2g-test-22027d260a34)
- [Detailed project-routing contract](../docs/PROJECTS.md)

GitHub owns code and delivery evidence; Linear owns planning and dependencies. The linked organization Project provides the cross-repository execution view.
<!-- org-project-routing:end -->
