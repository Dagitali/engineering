<!--
engineering/templates/README.md
Dagitali organization documentation

Responsibilities
- Index blank templates and explain copying and verification.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Engineering Templates

- [Using Templates](#using-templates)
- [Updating Adopted Templates](#updating-adopted-templates)
- [Repository Instructions](#repository-instructions)
- [Development and Review](#development-and-review)
- [Verification Records](#verification-records)
- [Adoption and Ownership](#adoption-and-ownership)
- [Release Templates](#release-templates)

## Using Templates

Choose a blank form, replace project-specific fields, and retain completed records with their owner.
Installing a Copilot template requires the consuming repository's supported local path and actual
globs. Templates do not change a project's license, support commitments, branching model, or
operational authority.

Copy the selected template into the consuming project, replace explicit fields, and remove
inapplicable guidance. Verify local destinations, installed instruction paths/globs, and the
project's actual commands before use. Keep source templates blank in this checkout and store
completed records with their owner.

## Updating Adopted Templates

Record the source path and copied commit or tag in the consuming project. Compare that revision with
the proposed update, review compatibility and replacement fields, and preserve intentional local
adaptations. Updating this collection does not update existing copies.

Apply the smallest reviewed change, verify local links, installed paths and globs, and actual
commands, then run the consuming project’s relevant checks. Record the resulting source revision,
validation, and recovery reference with that project. Keep completed adoption records outside this
checkout.

## Repository Instructions

- [Repository Agent Instructions Template](AGENTS.md)
- [Repository Copilot Instructions Template](copilot/copilot-instructions.md)
- [Mermaid Diagram Instructions](copilot/mermaid.instructions.md)
- [Swift Testing Instructions Template](copilot/swift-testing.instructions.md)
- [Swift Source Instructions Template](copilot/swift.instructions.md)

## Development and Review

- [Developer Onboarding Template](developer-onboarding.md)
- [Development Task Templates](development-task.md)
- [Architecture Decision Template](architecture-decision.md)
- [Change Impact Map Template](change-impact-map.md)
- [Apple App Pull Request Template](pull-request-apple-app.md)
- [Infrastructure Pull Request Template](pull-request-infrastructure.md)

## Verification Records

- [Evidence Inventory Template](evidence-inventory.md)
- [Feature Verification](feature-verification.md)
- [Apple Platform Graphics](apple-platform-graphics.md)
- [CloudKit Sync Verification](cloudkit-sync-verification.md)
- [External Service Data Handling](external-service-data-handling.md)
- [External Service Operations](external-service-operations.md)

## Adoption and Ownership

- [Consumer Inventory Template](consumer-inventory.md)
- [Shared Automation Adoption Template](shared-automation-adoption.md)

## Release Templates

- [App Store Metadata](app-store-metadata.md)
- [Apple App Release Checklist](apple-app-release-checklist.md)
- [Python Release Checklist Template](python-release-checklist.md)
- [TestFlight Beta Checklist](testflight-beta-checklist.md)
- [Apple App Release Notes](releases/apple-app.md)
- [Python Package Release Notes](releases/python-package.md)
- [Shared Automation Release Notes](releases/shared-automation.md)
