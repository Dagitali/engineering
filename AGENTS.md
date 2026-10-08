<!--
engineering/AGENTS.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Define repository boundaries and required evidence for agent work.

Responsibilities
- Define repository boundaries and required evidence for agent work.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Engineering Repository Instructions

Read [README.md] and [CONTRIBUTING.md] before changes. Preserve unrelated work, project-owned contracts,
source notices, stable links, and historical evidence. Shared guidance does not override local
licenses, support commitments, toolchain versions, branching models, or public product behavior.

Validate Markdown destinations, headings, reference labels, template placeholders, and source
accuracy. Keep templates blank and private completed records out of this checkout. Do not publish,
commit, tag, configure remotes, or change hosted state without task authority. Report actual checks
and limitations.

- [Repository Map](#repository-map)
- [Validation and Release Readiness](#validation-and-release-readiness)
- [Completion Report](#completion-report)

## Repository Map

Use the [architecture overview] for ownership and layout, [design guidance] for content constraints,
and the [change impact map] for the smallest complete review scope. The [documentation index]
links maintenance and adoption procedures. Consumer-specific sources and completed records remain
with their owners.

## Validation and Release Readiness

Follow the [validation procedure] and select checks appropriate to the changed boundary. Review
source accuracy and reference labels separately from destination checks. Inspect formatting-tool
side effects; preserve front matter, blank placeholders, notices, and stable anchors.

For release work, use this collection’s [release policy] and [release playbook]. Distinguish
candidate preparation, local tags, hosted validation, publication, and consumer rollout. Preserve
historical outcomes and immutable tag identities; documentation alone does not establish delivery.

## Completion Report

Follow [completion evidence] when reporting work. State the result, affected files, relevant source
evidence, actual checks and outcomes, failed or skipped checks with reasons, adoption effects, and
remaining work. Keep current-checkout results separate from historical and hosted evidence. Report
limitations without implying unperformed checks passed.

[architecture overview]: ARCHITECTURE.md
[CONTRIBUTING.md]: CONTRIBUTING.md
[validation procedure]: CONTRIBUTING.md#validation
[design guidance]: DESIGN.md
[README.md]: README.md
[release policy]: RELEASE-POLICY.md
[change impact map]: architecture/change-impact-map.md
[documentation index]: documentation/README.md
[completion evidence]: documentation/maintenance.md#completion-evidence
[release playbook]: playbooks/release.md
