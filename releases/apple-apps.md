<!--
engineering/releases/apple-apps.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide signed app evidence and beta versus public-release readiness.

Responsibilities
- Guide signed app evidence and beta versus public-release readiness.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Apple App Releases

Keep app metadata and evergreen release procedure separate from candidate records. Each candidate
records version/build, schema, platforms, exact signed artifact, privacy behavior, blockers, and
evidence.

- [Compatibility and Product Readiness](#compatibility-and-product-readiness)
- [Signed Artifact Validation](#signed-artifact-validation)
- [Beta Acceptance and Public Release](#beta-acceptance-and-public-release)

## Compatibility and Product Readiness

Review product behavior, permissions, external data flows, persistence/migration, asset licensing,
accessibility, and supported platforms. Synchronize privacy policy, nutrition labels, product copy,
screenshots, and tester instructions with actual behavior. Do not turn product-specific privacy
promises into organization-wide guarantees.

## Signed Artifact Validation

Verify developer identity, entitlements, signing, App Store Connect configuration, metadata/URLs,
screenshots, privacy answers, uploaded build, tester access, and review state. Automated Debug tests
do not prove the exact signed Release binary. Retain archive inspection and actual device/TestFlight
evidence. Persistence and private sync need relevant account/device/migration checks alongside
automated tests.

## Beta Acceptance and Public Release

Separate invited-beta acceptance from public-release readiness. Record deferred checks with decision
date, owner, accepted risk, tester guidance, and completion milestone; a waiver is not a pass. Use
the [release checklist], [TestFlight checklist], and [metadata template]. Follow the app's local
release policy for delivery.

[metadata template]: ../templates/app-store-metadata.md
[release checklist]: ../templates/apple-app-release-checklist.md
[TestFlight checklist]: ../templates/testflight-beta-checklist.md
