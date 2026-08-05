# Security policy

## Reporting a vulnerability

Do not disclose vulnerabilities, credentials, exploit details, or sensitive logs in a public issue or pull request.

Use GitHub's private vulnerability reporting feature on the affected repository when available. Otherwise, contact an organization maintainer through a private channel and include:

- the affected repository, version, commit, or environment;
- a concise description of the impact;
- reproducible steps or a minimal proof of concept;
- any known workarounds or mitigations;
- whether the issue is already public.

A maintainer should acknowledge a credible report promptly, coordinate validation and remediation, and publish an advisory when users need to take action. Public disclosure should wait until a fix or practical mitigation is available unless immediate disclosure is necessary to protect users.

## Scope

Security concerns include leaked secrets, unsafe test fixtures, dependency or workflow supply-chain risks, privilege-boundary errors, artifact tampering, and test infrastructure that can affect repositories outside the intended sandbox.

## Supported code

Security fixes generally target maintained default branches and currently supported releases. Archived or explicitly experimental repositories may receive best-effort remediation only; their README should make that status clear.
