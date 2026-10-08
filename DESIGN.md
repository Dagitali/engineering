<!--
engineering/DESIGN.md
Dagitali organization documentation

Responsibilities
- Explain design and its ownership boundaries.

Maintainer Notes
- Link canonical guidance and preserve purposeful project differences.
-->

# Design

- [Goals and Non-Goals](#goals-and-non-goals)
- [Public Interface](#public-interface)
- [Configuration Strategy](#configuration-strategy)
- [Testing and Change Safety](#testing-and-change-safety)
- [Decision Recording and Evolution](#decision-recording-and-evolution)

## Goals and Non-Goals

Provide reusable guidance with explicit ownership, review scope, and evidence limits. Prefer links
to canonical sources over competing copies. Consumer-specific services, support promises, accounts,
and mandatory toolchains belong with their projects.

## Public Interface

Document paths, linked headings, reference destinations, template fields, and adoption instructions
are compatibility considerations. Preserve existing links and explain replacements and migrations.
Use the [interface checklist] and [release policy] when adoption behavior changes.

## Configuration Strategy

Use [configuration contract guidance] to review inputs, defaults, paths, and migration. This
collection has no universal consumer configuration schema. Templates expose replacement fields;
consumers own installed paths, globs, tool versions, commands, and workflow settings. Keep examples
neutral and copy only what a demonstrated requirement needs. Local hooks describe this checkout, not
a required consumer setup.

## Testing and Change Safety

Follow the [validation procedure] for this checkout. Validate Markdown structure and claims, retain
blank templates, and inspect side effects of formatting hooks. Use [testing guidance] to choose
consumer evidence by boundary; package, device, cloud, and hosted validation remain separate where
applicable.

## Decision Recording and Evolution

Record durable alternatives and consequences through [decision guidance]. Keep reusable diagnosed
failures in [learnings] and recovery procedures in runbooks. Preserve historical evidence and
purposeful local differences. [Architecture] describes this collection’s organization.

[Architecture]: ARCHITECTURE.md
[validation procedure]: CONTRIBUTING.md#validation
[learnings]: LEARNINGS.md
[release policy]: RELEASE-POLICY.md
[decision guidance]: architecture/decision-records.md
[configuration contract guidance]: interfaces/configuration-contracts.md
[interface checklist]: interfaces/evolution-checklist.md
[testing guidance]: testing/README.md
