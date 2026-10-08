<!--
engineering/CHANGELOG.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Public history of user-visible changes and compatibility corrections.

Responsibilities
- Maintain changelog for this repository.

Maintainer Notes
- Preserve released entries and group pending changes under Unreleased.
- Keep local links and documented behavior consistent with repository sources.
- Keep shared guidance independent of any originating project.
-->

# Changelog

This file records concise, user-visible changes to shared guidance and templates. The [release notes
archive] indexes detailed scope, compatibility, validation evidence, and release status. The
[release policy] owns version classification and compatibility review. The [reading guide] explains
candidate identity and historical evidence boundaries.

The format is based on [Keep a Changelog]. Version classification is informed by [Semantic
Versioning] and adapted to documentation and template compatibility by the local release policy.

Entries summarize local Git evidence. Dates for existing versions are annotated-tag creation dates
in America/New_York, not verified publication dates. Changes after the latest tag remain under
Unreleased until assigned to a reviewed release.

- [Unreleased](#unreleased)
- [0.1.0 - 2026-10-08](#010---2026-10-08)
  - [Initial Customization](#initial-customization)
- [0.0.0 - 2026-10-08](#000---2026-10-08)
  - [Initial Collection](#initial-collection)

## Unreleased

- Added repository-wide MIT licensing and project attribution after `v0.1.0`.
- Added support, security, conduct, and release policies, with evidence-bounded historical records.
- Added architecture, design, and learnings overviews, generic adoption and release playbooks,
  contributor onboarding, and configuration-contract guidance.
- Expanded testing-layer, dependency-boundary, workflow-responsibility, and hosted-audit guidance.
- Improved repository navigation and guidance for updating adopted templates while preserving
  consumer-owned contracts, blank source templates, and historical evidence.

Entries describe integrated changes since the latest tag; unreviewed working-tree proposals are not
evidence of a release.

## [0.1.0] - 2026-10-08

### Initial Customization

- Normalized Markdown structure and reference links.
- Added topic indexes, an adoption tutorial, consumer scaffolding guidance, and a reference library.
- Updated local hook configuration and documentation conventions.

See the [0.1.0 record] for evidence boundaries.

## [0.0.0] - 2026-10-08

### Initial Collection

- Initial engineering guidance and blank-template collection.

See the [0.0.0 record] for evidence boundaries.

[release policy]: RELEASE-POLICY.md
[Keep a Changelog]: https://keepachangelog.com/en/1.1.0/
[Semantic Versioning]: https://semver.org/spec/v2.0.0.html
[reading guide]: releases/evidence-and-history.md
[release notes archive]: releases/history/README.md
[0.0.0]: releases/history/v0.0.0.md
[0.0.0 record]: releases/history/v0.0.0.md
[0.1.0]: releases/history/v0.1.0.md
[0.1.0 record]: releases/history/v0.1.0.md
