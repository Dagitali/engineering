<!--
engineering/playbooks/release.md
Dagitali organization documentation

Responsibilities
- Explain release playbook and its ownership boundaries.

Maintainer Notes
- Link canonical guidance and preserve purposeful project differences.
-->

# Release Playbook

- [Prepare](#prepare)
- [Validate](#validate)
- [Tag and Publish](#tag-and-publish)
- [Close Out](#close-out)

## Prepare

Identify the component’s owning release policy, supported surface, candidate revision, previous
release, and complete diff. Review compatibility, migration, attribution, and recovery. For this
collection, follow the [repository release policy]; for other components, use their local policy.

## Validate

Run focused checks and the applicable broader gate from the candidate. Validate artifacts,
installation, device behavior, or hosted callers only where the contract requires them. Record
commands, environment, results, skipped checks, and identity using [release evidence]. A source
check does not establish publication or deployed compatibility.

## Tag and Publish

Use the owner’s authorized branch route, tag convention, and publication mechanism. Confirm the
reviewed revision and immutable identity before delivery. Commits, tags, pushes, and publication
need task authority; this playbook does not enable them. Retain separate evidence for each stage.

## Close Out

Reconcile changelog and version records with actual outcomes. Index the record in the owning
archive, disclose limitations and follow-up owners, and preserve tags. Correct defects through
reviewed follow-up releases. Verify consumer rollout separately from publication.

[repository release policy]: ../RELEASE-POLICY.md
[release evidence]: ../releases/evidence-and-history.md
