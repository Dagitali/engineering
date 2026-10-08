<!--
engineering/governance/branch-protection.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide review controls and verification of required check coverage.

Responsibilities
- Guide review controls and verification of required check coverage.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Branch Protection

Protect each maintained integration or release branch according to the project's actual branching
model. Shared guidance does not require fixed branch names, GitFlow, or identical consumer policies.

- [Review Baseline](#review-baseline)
  - [Approval Freshness](#approval-freshness)
  - [Optional History and Signing Controls](#optional-history-and-signing-controls)
- [Required Results](#required-results)
  - [Branch Currency and Required Checks](#branch-currency-and-required-checks)

## Review Baseline

Use reviewed pull requests, resolved conversations, and successful required checks. Restrict
deletion, force pushes, and bypass access. Choose independent approval requirements appropriate to
available reviewers; authors cannot supply independent approval of their own changes. Review
overlapping rules and recovery exceptions. Record visibility or plan limitations rather than
claiming unavailable controls.

CODEOWNERS routes review but neither grants access nor activates required approval. Verify owner
access and hosted rules separately. Local hooks provide feedback and do not replace server-side
enforcement.

### Approval Freshness

Where independent reviewers are available, consider dismissing stale approvals or requiring review
of the latest push so approval covers the changes being merged. Choose controls that fit the
project's review capacity, and verify their hosted behavior after changes to the PR. An approval of
an earlier revision does not establish review of later edits.

### Optional History and Signing Controls

Require linear history or signed commits only when compatible with the project's merge strategy and
contributor tooling. Review how the chosen merge method affects commit signatures and history, and
retain a documented integration and recovery path. These optional controls do not replace
independent review or successful required checks.

## Required Results

Choose exact names from representative successful hosted runs, including matrix expansion and
source. Preserve unique job names and trigger coverage. Required results must report on every
applicable PR; verify `merge_group` coverage before requiring them in a merge queue. Manual/advisory
jobs and path-filtered jobs need explicit review before becoming requirements.

### Branch Currency and Required Checks

Choose strict checks when a branch must be current with its target before merging; use loose checks
only when the integration risk is acceptable. Do not require a path-filtered workflow unless an
alternative reports the required result for excluded changes. Verify that every selected check
reports for queued merge groups before enabling a merge queue; ordinary PR results alone do not
establish queue coverage.

Use the [transition runbook] before changing names or selecting new requirements. Keep exact
branches, contexts, owners, and dated verification in the project. The [GitFlow guide] is an
optional model for projects that adopt it.

[GitFlow guide]: ../git/gitflow.md
[transition runbook]: ../runbooks/update-required-checks.md
