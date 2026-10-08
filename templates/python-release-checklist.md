<!--
engineering/templates/python-release-checklist.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Python Release Checklist Template

Replace commands and integration routes using the project's release policy.

- [ ] Review the complete candidate diff and compatibility/migration impact.
- [ ] Confirm dependency support and fixtures; record intended version and matching dated changelog.
- [ ] Prepare versioned notes with candidate identity, support boundary, and outstanding evidence.
- [ ] Run `<focused checks>`, `<quality gate>`, and `<documentation checks>`.
- [ ] Build wheel and source distribution in a fresh directory; validate metadata and contents.
- [ ] Install and exercise each artifact cleanly without source-path leakage.
- [ ] Integrate through `<reviewed branch route>` and verify the authoritative candidate.
- [ ] Obtain task authority for tag/push/publication; preserve immutable tags.
- [ ] Verify actual hosted artifact/publication outcomes and consumer recovery path.
- [ ] Close records with results, skipped checks, limitations, and follow-up ownership.
