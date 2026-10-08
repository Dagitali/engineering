<!--
engineering/governance/branch-protection.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Branch Protection

Protect each maintained integration or release branch according to the project's actual branching
model. Shared guidance does not require fixed branch names, GitFlow, or identical consumer policies.

## Review Baseline

Use reviewed pull requests, resolved conversations, and successful required checks. Restrict deletion,
force pushes, and bypass access. Choose independent approval requirements appropriate to available
reviewers; authors cannot supply independent approval of their own changes. Review overlapping rules
and recovery exceptions. Record visibility or plan limitations rather than claiming unavailable controls.

CODEOWNERS routes review but neither grants access nor activates required approval. Verify owner access
and hosted rules separately. Local hooks provide feedback and do not replace server-side enforcement.

## Required Results

Choose exact names from representative successful hosted runs, including matrix expansion and source.
Preserve unique job names and trigger coverage. Required results must report on every applicable PR;
verify `merge_group` coverage before requiring them in a merge queue. Manual/advisory jobs and path-
filtered jobs need explicit review before becoming requirements.

Use the [transition runbook](../runbooks/update-required-checks.md) before changing names or selecting
new requirements. Keep exact branches, contexts, owners, and dated verification in the project.
The [GitFlow guide](../git/gitflow.md) is an optional model for projects that adopt it.
