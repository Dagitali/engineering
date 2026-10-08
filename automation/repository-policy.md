<!--
engineering/automation/repository-policy.md
Dagitali organization documentation

Responsibilities
- Guide selection and verification of consumer-owned repository checks.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Repository Policy Checks

Select repository validators by the actual policy and files they inspect. Consumers own expected
values, installation, integration, and remediation. A validator's development settings are not
consumer policy.

- [Select and Configure](#select-and-configure)
- [Migrate Existing Checks](#migrate-existing-checks)
- [Integrate and Verify](#integrate-and-verify)

## Select and Configure

Use [configuration contracts] to review defaults, precedence, path resolution, and unknown keys.
Define each check's inputs, discovery scope, configuration, expected diagnostics, exit behavior, and
side effects. Prefer read-only checks when validation alone is required. Do not create irrelevant
package metadata or copy language/cloud assumptions merely to satisfy a tool. Install a reviewed
immutable tool revision through the consuming project's reproducible environment.

## Migrate Existing Checks

Compare old and replacement commands against the same repository revision. Use successful,
deliberately failing, and boundary fixtures. Verify reporting, exit behavior, read-only guarantees,
and intentional exceptions before replacing local scripts. Keep regression cases for purposeful
consumer differences.

Classify each difference as configuration drift, an intentional policy change, unsupported
replacement behavior, or a defect. Separate tool adoption from policy changes where possible. Retain
existing checks for requirements the replacement does not cover, and review every caller before
retiring a script. A successful replacement run does not establish equivalent coverage; confirm both
accepted and deliberately rejected cases and document residual gaps.

## Integrate and Verify

Use the same documented invocation locally and in CI. Distinguish tool-format validation from the
safety of inspected code, and declared policy from hosted enforcement. Keep authenticated hosted
audits opt-in and separate from ordinary offline checks. Record owner, tool revision, configuration,
commands, evidence, and previous known-good behavior for recovery. Use [change management] and the
[hosted audit runbook] where applicable.

[configuration contracts]: ../interfaces/configuration-contracts.md
[change management]: ../playbooks/change-management.md
[hosted audit runbook]: ../runbooks/hosted-settings-audit.md
