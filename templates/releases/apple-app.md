<!--
engineering/templates/releases/apple-app.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Blank apple app release notes for project-owned planning and verification.

Responsibilities
- Provide a blank apple app release notes template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Apple App Release Notes

Replace fields with actual outcomes. Retain completed records in the released project's archive.
Use the [release evidence guide] and [platform release guide] while preparing the record. When
copying this template, adapt these links to destinations available in the consuming project.

- [Candidate and Highlights](#candidate-and-highlights)
- [Change Scope](#change-scope)
- [Compatibility and Support](#compatibility-and-support)
  - [Breaking Changes](#breaking-changes)
  - [Deprecations](#deprecations)
  - [Support Boundary](#support-boundary)
- [Validation and Artifacts](#validation-and-artifacts)
  - [Artifact Contracts](#artifact-contracts)
- [Publication and Rollback](#publication-and-rollback)
- [Follow Up](#follow-up)

## Candidate and Highlights

`<Project, version/build, status, verified event date/timezone, evidence identifying candidate,
changelog link>`.

## Change Scope

`<User-visible changes, fixes, relevant decisions, and material unchanged boundaries>`.

## Compatibility and Support

`<Breaking changes, deprecations, defaults, support/runtime changes, migration, or explicit none>`.
User-facing improvements, supported platforms, permissions, data migrations, sync, external service
disclosures, signed build/channel identity, and tester guidance.

### Breaking Changes

`<Affected behavior, prior and new contract, required consumer action, migration, or explicit none>`.

### Deprecations

`<Deprecated interface, replacement, migration owner/steps, removal policy, or explicit none>`.

### Support Boundary

`<Supported runtimes/platforms/interfaces, verified combinations and evidence, configurable but
unverified alternatives, exclusions, or explicit no changes>`.

## Validation and Artifacts

`<Exact revision/artifacts, environment, commands, dates, results, integrity evidence, hosted versus
local, failed/skipped checks and reasons, manual verification, and limitations>`.

### Artifact Contracts

`<Artifact names, formats, contents, retention, download/installation expectations, changed
contracts and consumer migration, or explicit no changes>`. Keep release artifacts distinct from
diagnostics; record applicable upload behavior on success, failure, and cancellation, and link
validation evidence for missing or unverified outcomes.

## Publication and Rollback

`<Actual publication/distribution state, approved operations, protected environment, prior
known-good revision, staged adoption, migration/rollback, or not published>`.

## Follow Up

`<Remaining blockers, owner, next verification, public issue links where appropriate>`.

Do not infer publication from a build, overwrite historical results, retarget immutable tags, or
include confidential evidence. Use N/A with a reason for inapplicable items.

[platform release guide]: ../../releases/apple-apps.md
[release evidence guide]: ../../releases/evidence-and-history.md
