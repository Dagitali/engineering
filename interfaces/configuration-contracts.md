<!--
engineering/interfaces/configuration-contracts.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Explain configuration contracts and verification boundaries.

Responsibilities
- Explain configuration contracts and verification boundaries.

Maintainer Notes
- Preserve consumer-owned commands, configuration, and policy.
-->

# Configuration Contracts

- [Ownership and Sources of Truth](#ownership-and-sources-of-truth)
- [Inputs and Defaults](#inputs-and-defaults)
- [Paths and Discovery](#paths-and-discovery)
- [Validation and Failure Behavior](#validation-and-failure-behavior)
- [Compatibility and Migration](#compatibility-and-migration)
- [Sensitive Values](#sensitive-values)

## Ownership and Sources of Truth

Each component owns its accepted configuration and supported versions. Consumers own values and
integration. Keep the schema, implementation, examples, and validation aligned; this guide defines a
review method, not a universal configuration format. Use the [interface checklist] for evolution.

## Inputs and Defaults

Document locations, accepted keys and types, required fields, defaults, precedence, environment
overrides, and unknown-key behavior. Distinguish absence from an empty or invalid value. Verify that
examples use supported inputs rather than borrowing another component’s settings.

## Paths and Discovery

State the base for each relative path, discovery rules, exclusions, encoding expectations, and
symlink behavior. Explain missing-file and out-of-root handling. Do not assume every command uses
the same working directory or resolution rule. Separate local destinations from remote resources.

## Validation and Failure Behavior

Define when validation occurs, diagnostics, exit or error behavior, partial-result handling, and
side effects. Cover valid, malformed, missing, and boundary inputs where meaningful. Schema
validation does not establish that referenced code is safe or that hosted settings are enforced.

## Compatibility and Migration

Review stricter validation, changed defaults, removed keys, and discovery changes as potential
consumer migrations. Keep intentional differences explicit, retain regression evidence, and document
recovery. Use [policy-check guidance] when replacing validators and the component’s own release
policy for classification.

## Sensitive Values

Keep credentials and private identifiers out of examples, fixtures, and reports. Document safe
redaction and diagnostic behavior in the owning component. Verify access and execution boundaries
through [workflow trust guidance]; configuration review does not authorize secret retrieval.

[policy-check guidance]: ../automation/repository-policy.md
[workflow trust guidance]: ../security/workflow-trust-boundaries.md
[interface checklist]: evolution-checklist.md
