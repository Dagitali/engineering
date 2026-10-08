<!--
engineering/templates/pull-request-infrastructure.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Blank infrastructure pull request for project-owned planning and verification.

Responsibilities
- Provide a blank infrastructure pull request template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Infrastructure Pull Request Template

Copy to the consuming project's supported PR template location and replace instructions with local
checks.

- [Summary and Scope](#summary-and-scope)
- [Compatibility and Infrastructure](#compatibility-and-infrastructure)
- [Validation](#validation)
- [Documentation and Delivery](#documentation-and-delivery)
- [Deployment and Rollback](#deployment-and-rollback)
- [Checklist](#checklist)

## Summary and Scope

`<Problem, resulting behavior, affected interfaces, related issue, target branch>`.

## Compatibility and Infrastructure

`<Defaults, resources, logical identity/replacement, IAM/public access, retention, TLS/DNS,
availability, cost, consumer ownership, migration, and rollback>`.

## Validation

`<Exact revision, commands/results, synthesis inspection, packaging/install checks, local versus
hosted, failed/skipped checks and reasons>`.

## Documentation and Delivery

`<Updated contracts/examples/decisions/changelog, delivery effect, approved operational steps>`.

## Deployment and Rollback

`<Deployment/publication effect or explicit none, configuration changes, resource replacements, data
migrations, expected interruption, separately approved operations, prior safe revision/state,
rollback or forward-fix steps, recovery owner, and verification>`. Cross-reference compatibility
impacts above. Identify irreversible effects and retained-state requirements; restoring code alone
may not restore replaced resources or migrated data. Keep private account and operational details in
restricted records.

## Checklist

- [ ] Focused diff and affected behavior reviewed.
- [ ] Applicable tests and documentation updated.
- [ ] Security, lifecycle, replacement, and cost effects reviewed.
- [ ] Artifact and clean-install checks recorded where relevant.
- [ ] Recovery and outstanding work assigned.

Leave inapplicable items unchecked with N/A and a reason. This template does not authorize
deployment.
