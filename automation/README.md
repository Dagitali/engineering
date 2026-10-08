<!--
engineering/automation/README.md
Dagitali organization documentation

Responsibilities
- Index shared automation adoption and validation guidance.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Shared Automation

Adopt shared automation through explicit, reviewed references. Each consumer owns caller events,
required checks, runtime policy, identity, and delivery. These practices work with any maintained
action or workflow library; executable contracts remain documented with the chosen implementation.

- [Validation and delivery](validation-and-delivery.md)
- [Repository policy checks](repository-policy.md)
- [Workflow trust boundaries](../security/workflow-trust-boundaries.md)
- [Adoption record template](../templates/shared-automation-adoption.md)
- [Automation contract testing](../testing/automation-contracts.md)

Before adoption, identify the library owner, supported interface, released revision, access
requirements, and rollback reference. Review actual inputs, outputs, permissions, runners,
artifacts, and failure behavior. Copying a starter and updating a shared reference are separate
changes; neither automatically enables hosted settings or grants delivery authority.
