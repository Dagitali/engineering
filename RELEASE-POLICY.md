<!--
engineering/RELEASE-POLICY.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Version classification, candidate validation, and publication boundaries.

Responsibilities
- Maintain engineering repository release policy for this repository.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Engineering Repository Release Policy

- [Scope](#scope)
- [Versioning and Compatibility](#versioning-and-compatibility)
- [Candidate Validation](#candidate-validation)
- [Release Records](#release-records)
- [Publication and Recovery](#publication-and-recovery)

## Scope

This policy covers revisions of this repository’s documentation and templates. Platform-specific
release guides describe consuming projects, whose release policies remain authoritative. This
checkout has local hooks and no repository-local GitHub Actions workflow; documentation does not
establish hosted publication or enforcement.

## Versioning and Compatibility

Existing tags use `vMAJOR.MINOR.PATCH`. Classify new candidates by adoption impact: corrections
without required migration are patch candidates; additive guidance or templates are minor
candidates. Required migration needs explicit compatibility review and release notes; after 1.0,
intentional incompatible contracts warrant a major version. Pre-1.0 revisions can change adoption
requirements, so review the complete diff rather than relying on the version alone.

Preserve linked paths, headings, reference labels, placeholders, and attribution where feasible.
Explain replacements and migration steps when these change. No fixed deprecation or backport window
is established; consult the [support guide].

## Candidate Validation

Review the complete candidate diff and contribution terms. Follow the [validation procedure] for
applicable hooks, local destinations, heading anchors, reference labels, and template checks. Verify
source claims and keep templates blank. Record exact commands, revisions, results, and skipped
checks. Validation of today’s checkout does not validate an older tag.

## Release Records

Maintain concise changes in the [changelog] and revision-specific records in the [release archive].
Record compatibility, migration, validation, limitations, and candidate identity. Distinguish a
prepared candidate, local tag, hosted tag, and published release. Git tag dates do not establish
publication dates. See the [evidence guide].

## Publication and Recovery

Creating commits or tags, pushing, and publishing require explicit task authority. Review the
candidate identity and authorized branch route before creating an immutable release tag. No
automated publication or package-distribution contract is established here.

Do not move existing tags to repair defects. Prepare a reviewed correction or new release and retain
dated clarification of earlier outcomes. Consumers decide when and how to update adopted copies; a
release does not modify those copies automatically.

[changelog]: CHANGELOG.md
[validation procedure]: CONTRIBUTING.md#validation
[support guide]: SUPPORT.md
[evidence guide]: releases/evidence-and-history.md
[release archive]: releases/history/README.md
