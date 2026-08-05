# Governance

## Decision model

The organization uses maintainer-led, review-driven governance. Changes should be decided as close as practical to the repository that owns the behavior while preserving organization-wide security, compatibility, and documentation standards.

## Roles

- **Contributors** propose changes, provide tests and documentation, and participate in review.
- **Maintainers** triage work, review and merge changes, manage releases, and uphold repository boundaries.
- **Organization owners** manage access, shared policy, cross-repository architecture, and exceptional risk decisions.

Roles are based on demonstrated responsibility and current need, not title alone. Access should follow least privilege and be reviewed periodically.

## Significant changes

Cross-repository interfaces, breaking changes, security-sensitive behavior, data formats, release policy, and repository transfers should have a written proposal or decision record. The record should state context, options, decision, consequences, migration, and rollback.

## Resolving disagreement

Prefer evidence, prototypes, compatibility analysis, and reversible experiments. If consensus is not possible, the maintainers responsible for the affected boundary decide and document the rationale. Organization owners arbitrate disputes that span repositories or involve security, access, or policy.

## Deprecation and archival

Do not silently delete history or abandon consumers. Mark deprecated repositories clearly, provide migration guidance when practical, preserve releases and decision records, and archive only after active replacements and ownership boundaries are documented.
