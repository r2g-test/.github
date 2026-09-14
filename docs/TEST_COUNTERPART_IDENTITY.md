# Test counterpart identity

`r2g-test` currently has no admitted production GitHub counterpart.

The machine-readable state is `architecture/test-counterpart.json`, whose `status` is `unconfigured`. Until that file (and the organization relationship registry) is changed through review, repositories in this test organization must not infer another GitHub owner from the `r2g-test` name or crawl a guessed owner as production evidence.

In particular, stripping `-test` yields `r2g`, which currently resolves to a GitHub **user** account. The reviewed relationship registry declares no cross-organization edge to that account, so its repositories are not admissible production inputs for contract, security, upgrade, chaos, or deployment certification.

Allowed while unconfigured:

- repository-local deterministic tests;
- public shared-dependency canaries that make no production-counterpart claim;
- documentation and fixtures needed to define a future counterpart mapping.

Not allowed while unconfigured:

- crawling another GitHub owner based on name similarity;
- reporting another owner's repository tips as `r2g-test` production evidence;
- treating a successful guessed-owner scan as promotion/certification evidence;
- silently falling back from an inaccessible private counterpart to a public same-named account.

A future active declaration must bind stable owner identity/type and an admitted repository scope, then test workflows must consume that declaration directly and bind exact source SHAs before execution.
