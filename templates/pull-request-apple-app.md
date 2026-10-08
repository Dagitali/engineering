<!--
engineering/templates/pull-request-apple-app.md
Dagitali organization documentation

Responsibilities
- Provide a blank apple app pull request template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Apple App Pull Request Template

Copy into the consuming project's PR template location and retain its own policy and release gates.

- [Summary and Review Focus](#summary-and-review-focus)
- [Validation and UI Evidence](#validation-and-ui-evidence)
- [Privacy and Persistence](#privacy-and-persistence)
- [Distribution and Documentation](#distribution-and-documentation)

## Summary and Review Focus

`<User-visible problem, behavior, affected platforms/features, target release, risky files, related
issue>`.

## Validation and UI Evidence

`<Build/tests, local versus hosted status, device/manual checks, accessibility/localization,
sanitized screenshots, skipped checks and reasons>`.

## Privacy and Persistence

`<Permissions, collection, external requests, retention/deletion, sync, frozen schemas, migration,
conflict handling, and rollback>`.

## Distribution and Documentation

`<Signed artifact/channel effects, metadata/privacy copy, release notes, licensing, known risks>`.

- [ ] Focused change with tests for affected behavior.
- [ ] Supported platforms, accessibility, and UI evidence reviewed.
- [ ] Privacy, persistence, sync, and migration contracts preserved or explicitly changed.
- [ ] Applicable documentation and release evidence synchronized.
- [ ] Failed/skipped checks and follow-up ownership recorded.

Leave inapplicable checks unchecked with N/A and a reason. Product privacy promises remain local.
