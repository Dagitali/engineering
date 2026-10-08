<!--
engineering/templates/pull-request-infrastructure.md
Dagitali organization documentation

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

- [ ] Focused diff and affected behavior reviewed.
- [ ] Applicable tests and documentation updated.
- [ ] Security, lifecycle, replacement, and cost effects reviewed.
- [ ] Artifact and clean-install checks recorded where relevant.
- [ ] Recovery and outstanding work assigned.

Leave inapplicable items unchecked with N/A and a reason. This template does not authorize
deployment.
