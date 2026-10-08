<!--
engineering/templates/AGENTS.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Blank repository agent instructions for project-owned planning and
verification.

Responsibilities
- Provide a blank repository agent instructions template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Repository Agent Instructions Template

Copy into the consuming repository as `AGENTS.md`; replace fields and remove inapplicable guidance.

- [Repository Boundaries](#repository-boundaries)
- [Operating Model](#operating-model)
- [Validation and Documentation](#validation-and-documentation)
- [Project Conventions](#project-conventions)
- [Completion Report](#completion-report)

## Repository Boundaries

- Canonical metadata/configuration: `<paths>`.
- Public contracts and supported platforms: `<interfaces and authority>`.
- Consumer-owned concerns and non-goals: `<boundaries>`.
- Generated/user-owned output to preserve: `<paths>`.

## Operating Model

Read applicable instructions and inspect the working tree before editing. Preserve unrelated and
staged work. Trace claims to current source and tests. Bound the change and its side effects; keep
edits focused. Repository work does not implicitly authorize commits, tags, publication, deployment,
or hosted administration.

## Validation and Documentation

| Changed boundary | Focused checks | Broader gate | Documents to review |
| --- | --- | --- | --- |
| `<boundary>` | `<commands>` | `<command>` | `<paths>` |

Record local versus hosted evidence separately. Report changed files, failed/skipped checks and
reasons, compatibility and migration effects, and unresolved work. Keep confidential diagnostics out
of public prose.

## Project Conventions

`<Language style, deterministic test design, identity/data/resource safeguards, and release rules>`.

## Completion Report

Report the resulting behavior and changed files, intentional differences preserved, exact checks and
results, failures, and skipped checks with reasons. Identify compatibility/migration effects,
remaining limitations, and outstanding work or follow-up ownership. Distinguish current-checkout
results from historical, hosted, and publication evidence. Keep confidential details restricted;
edits alone do not establish successful verification.

`<Project-specific completion evidence and reporting requirements>`.
