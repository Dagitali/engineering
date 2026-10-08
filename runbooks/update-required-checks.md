<!--
engineering/runbooks/update-required-checks.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide coordinated required-check replacement and blocking verification.

Responsibilities
- Guide coordinated required-check replacement and blocking verification.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Update Required Checks

Use this procedure when a job name, matrix, trigger, or branch policy changes. The project's branch
protection guide owns the exact branches and required contexts. Hosted edits need the appropriate
authority.

- [Plan the Transition](#plan-the-transition)
- [Observe and Update](#observe-and-update)
- [Verify Enforcement](#verify-enforcement)
- [Diagnose and Recover](#diagnose-and-recover)

## Plan the Transition

Record the current rules, source Apps, bypass actors, operator, representative PR, and rollback
configuration in appropriate storage. Inspect event coverage, filters, conditions, dependencies,
matrix exclusions, and concurrency cancellation. Check whether the workflow can emit every required
result for the target branch and, where used, merge groups. Step labels are not check names.

## Observe and Update

Obtain representative successful hosted results for the replacement checks. Record exact emitted
names and matrix variants. Add and verify replacements before removing old requirements; coordinate
workflow and rules changes so neither a missing result nor an unintended bypass becomes the
integration path. Do not infer emitted names or enforcement solely from YAML.

## Verify Enforcement

For an authorized representative PR, confirm every intended result reports and must pass, a
deliberately failing required result blocks merging, advisory results stay advisory, and obsolete
names are not pending. Verify reviews, history rules, bypass limits, and merge-group behavior where
applicable.

## Diagnose and Recover

For missing results, inspect event/branch, filters, conditions, canceled or skipped dependencies,
matrix variants, source, duplicate names, and stale requirements. Restore the known-good selection
and compatible workflow together if the transition blocks valid work or weakens enforcement. Verify
blocking behavior again and record the change, operator, evidence, unresolved gaps, and next review.
