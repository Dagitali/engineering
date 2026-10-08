<!--
engineering/automation/repository-policy.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Repository Policy Checks

Select repository validators by the actual policy and files they inspect. Consumers own expected values,
installation, integration, and remediation. A validator's development settings are not consumer policy.

## Select and Configure

Define each check's inputs, discovery scope, configuration, expected diagnostics, exit behavior, and
side effects. Prefer read-only checks when validation alone is required. Do not create irrelevant package
metadata or copy language/cloud assumptions merely to satisfy a tool. Install a reviewed immutable tool
revision through the consuming project's reproducible environment.

## Migrate Existing Checks

Compare old and replacement commands against the same repository revision. Use successful, deliberately
failing, and boundary fixtures. Verify reporting, exit behavior, read-only guarantees, and intentional
exceptions before replacing local scripts. Keep regression cases for purposeful consumer differences.

## Integrate and Verify

Use the same documented invocation locally and in CI. Distinguish tool-format validation from the safety
of inspected code, and declared policy from hosted enforcement. Keep authenticated hosted audits opt-in
and separate from ordinary offline checks. Record owner, tool revision, configuration, commands, evidence,
and previous known-good behavior for recovery. Use [change management](../playbooks/change-management.md)
and the [hosted audit runbook](../runbooks/hosted-settings-audit.md) where applicable.
