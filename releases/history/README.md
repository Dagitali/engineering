<!--
engineering/releases/history/README.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Maintain engineering release history for this repository.

Responsibilities
- Maintain engineering release history for this repository.

Maintainer Notes
- Index records newest first and distinguish candidates from tagged revisions.
- Preserve recorded outcomes and disclose evidence gaps.
- Keep shared guidance independent of any originating project.
-->

# Engineering Release History

This archive indexes this collection’s release records, newest first. Use the [changelog] for
concise changes and the [release playbook] for preparation and closeout.

- [Records](#records)
- [Reading the Records](#reading-the-records)
  - [Evidence Boundaries](#evidence-boundaries)
  - [Release Operations](#release-operations)
- [Maintaining the Archive](#maintaining-the-archive)

## Records

- [v0.3.0] — 2026-10-08: Impact, dependency, task, and agent guidance.
- [v0.2.0] — 2026-10-08: Shared policies, reusable guidance, MIT licensing, and Markdown headers.
- [v0.1.0] — 2026-10-08: Initial project customization and documentation normalization.
- [v0.0.0] — 2026-10-08: Initial collection.

## Reading the Records

The changelog owns concise highlights; versioned records own scope, compatibility, support,
validation, recovery, and follow-up. A prepared candidate, existing tag, published release, and
consumer rollout are distinct states. Link to canonical policy rather than copying its full text.

### Evidence Boundaries

The 0.3.0 record is prepared in released form; its date is a release-document date, with tag and
publication evidence unverified. Local tags through 0.2.0 exist; each historical record retains the
evidence available at its preparation. They do not establish hosted validation, release publication,
or consumer rollout. Later inspection is not contemporaneous release evidence.

Dates shown for existing records come from annotated local tag metadata in America/New_York. They
are not verified publication dates. Preserve preparation and observation dates separately;
retrospective records do not change the original tagged tree.

### Release Operations

The [release policy] owns this collection’s validation and publication boundaries. The [release
playbook] provides a reusable sequence. Neither records nor policy files authorize commits, tags,
pushes, publication, or hosted changes. Preserve tag identity and prepare reviewed follow-up fixes.

## Maintaining the Archive

Add a record for each reviewed candidate or release, distinguish its state, and preserve immutable
tag identities. Follow the [release policy] and [evidence guide].

1. Create `releases/history/vMAJOR.MINOR.PATCH.md` for an agreed candidate. Mark an untagged
   candidate as planned and state its preparation date, or use undated when unknown.
2. Reconcile highlights and scope with the candidate tree and changelog. Retain applicable
   compatibility, support, validation, recovery, and follow-up sections.
3. Record actual checks, failures, skipped checks, and evidence gaps against the exact candidate. Do
   not transfer today’s successful checks to a historical tag.
4. Index records newest first with version, explicit state, date basis, and concise summary.
5. Follow the [validation procedure] for Markdown checks and complete the separate release-policy
   gates before authorized delivery.

Keep changes after the latest tag under Unreleased until assigned to a reviewed release.

[changelog]: ../../CHANGELOG.md
[validation procedure]: ../../CONTRIBUTING.md#validation
[release policy]: ../../RELEASE-POLICY.md
[release playbook]: ../../playbooks/release.md
[evidence guide]: ../evidence-and-history.md
[v0.0.0]: v0.0.0.md
[v0.1.0]: v0.1.0.md
[v0.2.0]: v0.2.0.md
[v0.3.0]: v0.3.0.md
