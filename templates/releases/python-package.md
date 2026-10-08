<!--
engineering/templates/releases/python-package.md
Dagitali organization documentation

Responsibilities
- Provide a blank python package release notes template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Python Package Release Notes

Replace fields with actual outcomes. Retain completed records in the released project's archive.

- [Candidate and Highlights](#candidate-and-highlights)
- [Change Scope](#change-scope)
- [Compatibility and Support](#compatibility-and-support)
- [Validation and Artifacts](#validation-and-artifacts)
- [Publication and Rollback](#publication-and-rollback)
- [Follow Up](#follow-up)

## Candidate and Highlights

`<Project, version/build, status, verified event date/timezone, evidence identifying candidate,
changelog link>`.

## Change Scope

`<User-visible changes, fixes, relevant decisions, and material unchanged boundaries>`.

## Compatibility and Support

`<Breaking changes, deprecations, defaults, support/runtime changes, migration, or explicit none>`.
Commands, flags, configuration, outputs, exit codes, exports, typing; wheel/sdist identity and clean
installation; optional synthesized-resource impact.

## Validation and Artifacts

`<Exact revision/artifacts, environment, commands, dates, results, integrity evidence, hosted versus
local, failed/skipped checks and reasons, manual verification, and limitations>`.

## Publication and Rollback

`<Actual publication/distribution state, approved operations, protected environment, prior
known-good revision, staged adoption, migration/rollback, or not published>`.

## Follow Up

`<Remaining blockers, owner, next verification, public issue links where appropriate>`.

Do not infer publication from a build, overwrite historical results, retarget immutable tags, or
include confidential evidence. Use N/A with a reason for inapplicable items.
