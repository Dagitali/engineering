<!--
engineering/README.md
Dagitali organization documentation

Responsibilities
- Index shared engineering guidance and clarify adoption boundaries.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Dagitali Engineering

Shared development practices, review procedures, and reusable documentation templates for Dagitali
projects. Each project retains its own executable configuration, licensing, support commitments,
release policy, and hosted settings.

- [Start Here](#start-here)
- [Goals and Non-Goals](#goals-and-non-goals)
- [Adoption](#adoption)
- [Topic Guides](#topic-guides)
- [Repository Map](#repository-map)
- [Contributing](#contributing)
- [Support and Community](#support-and-community)
- [License](#license)
- [Validation and Scope](#validation-and-scope)

## Start Here

- [Developer onboarding]
- [Development workflow]
- [Documentation maintenance]
- [Change management]
- [Branch protection]
- [Automation]
- [Templates]
- [Source notices]
- [Reference library]

## Goals and Non-Goals

Provide reusable engineering practices, review guidance, and blank templates. Keep guidance grounded
in evidence and leave executable configuration, product policy, and operational authority with each
consuming project. This repository does not deploy products or enforce hosted settings.

## Adoption

Use shared guidance alongside the project's local instructions. Replace template fields before
installing a template in a consuming repository. Local commands, supported versions, branch routes,
permissions, and product guarantees remain authoritative in that project.

This repository contains reusable practice and blank templates. Project catalogs, migration
inventories, completed operational records, and product-specific contracts belong to their owners.
See the [license](#license) and [retained notices][Source notices] for applicable material terms.

## Topic Guides

Browse the [development index], [testing index], and [release index] for guidance grouped by task.
Use the [adoption tutorial] to try a local Markdown check with disposable files. Use [consumer
scaffolding] to plan a minimal project baseline and its readiness review.

- [Python](languages/python.md) and [Swift](languages/swift.md)
- [Python testing](testing/python.md), [infrastructure testing](testing/infrastructure.md),
  and [disposable cloud tests](testing/disposable-cloud-tests.md)
- [Interface evolution](interfaces/evolution-checklist.md)
- [Architecture decisions](architecture/decision-records.md)
- [GitFlow option](git/gitflow.md)
- [Ownership and exceptions](governance/ownership-and-exceptions.md)
- [Release evidence](releases/evidence-and-history.md), [Python releases](releases/python-packages.md),
  [Apple app releases](releases/apple-apps.md), and [shared automation releases](releases/shared-automation.md)
- [Repository incident response](runbooks/repository-ci-incident.md),
  [required check transitions](runbooks/update-required-checks.md),
  [hosted settings audits](runbooks/hosted-settings-audit.md), and
  [shared automation incidents](runbooks/shared-automation-incident.md)
- [Automation contract testing](testing/automation-contracts.md)
- [Workflow trust boundaries](security/workflow-trust-boundaries.md)
- [CDK change safety](infrastructure/cdk-change-safety.md)
- [Tooling lessons](learnings/python-and-repository-tooling.md)

Read [Architecture] for ownership and adoption flow, [Design] for content constraints, and
[Learnings] for reusable diagnosed failures.

## Repository Map

| Area | Purpose |
| --- | --- |
| [Documentation index] | Maintenance and adoption procedures |
| [Architecture index] | Decision recording and impact planning |
| [Templates] | Blank forms and instruction templates |
| [development index] and [testing index] | Planning and verification |
| [release index] | Consumer release guidance |
| [Repository release policy] and [Changelog] | This collection’s versioning and history |
| [Automation], [runbook index], and [playbook index] | Adoption, diagnosis, and change planning |

## Contributing

Read the [contributor guide] and [repository instructions] before editing. Keep reusable guidance
separate from project-owned contracts, and keep source templates blank.

## Support and Community

Use the [Support guide] for help and maintenance boundaries, the [Security policy] for sensitive
findings, and the [Code of Conduct] for participation standards and conduct concerns.

## License

This repository's documentation and templates are licensed under the [MIT License]. See [NOTICE]
for attribution and [Source notices] for the licensing transition. Adopting this guidance does not
change a consuming project's license or other project-owned contracts.

## Validation and Scope

Use the contributor guide's [validation procedure] for this checkout. Review local destinations,
heading anchors, reference labels, and template placeholders alongside source accuracy. Local checks
do not establish external availability, hosted enforcement, or publication. Browse the [runbook
index] for bounded operational procedures and the [playbook index] for change planning.

[repository instructions]: AGENTS.md
[Architecture]: ARCHITECTURE.md
[Changelog]: CHANGELOG.md
[Code of Conduct]: CODE_OF_CONDUCT.md
[contributor guide]: CONTRIBUTING.md
[validation procedure]: CONTRIBUTING.md#validation
[Design]: DESIGN.md
[Learnings]: LEARNINGS.md
[MIT License]: LICENSE
[NOTICE]: NOTICE
[Source notices]: NOTICES.md
[Reference library]: REFERENCES.md
[Repository release policy]: RELEASE-POLICY.md
[Security policy]: SECURITY.md
[Support guide]: SUPPORT.md
[Architecture index]: architecture/README.md
[Automation]: automation/README.md
[development index]: development/README.md
[Development workflow]: development/agent-assisted-workflow.md
[Developer onboarding]: development/onboarding.md
[Documentation index]: documentation/README.md
[adoption tutorial]: documentation/adopt-markdown-check.md
[Documentation maintenance]: documentation/maintenance.md
[Branch protection]: governance/branch-protection.md
[playbook index]: playbooks/README.md
[Change management]: playbooks/change-management.md
[consumer scaffolding]: playbooks/scaffold-consumer-project.md
[release index]: releases/README.md
[runbook index]: runbooks/README.md
[Templates]: templates/README.md
[testing index]: testing/README.md
