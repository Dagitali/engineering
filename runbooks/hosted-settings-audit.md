<!--
engineering/runbooks/hosted-settings-audit.md
Dagitali organization documentation

Responsibilities
- Guide read-only settings observations and follow-up evidence.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Hosted Settings Audit

Compare explicit repository expectations with authenticated, read-only hosted observations. Keep
inventory, expected contexts, reviewed tool revision, and exact invocation in the consuming
project's configuration. The selected audit tool's maintained reference owns its schema and exact
result names.

- [Prepare and Run the Audit](#prepare-and-run-the-audit)
- [Evidence and Access](#evidence-and-access)
- [Interpret Results](#interpret-results)
- [Exceptions and Follow-Up](#exceptions-and-follow-up)

## Prepare and Run the Audit

Define explicit repositories, branches, expected settings, required contexts, and audit exclusions.
Omitted expectations are outside the audit scope, not implicitly satisfied. Confirm the inventory
with its owner; desired configuration alone does not authorize changing hosted state.

Keep credentials outside the report. Store private operator details in restricted records. Use the
installed reviewed tool through the consuming project's reproducible environment; audits must not
silently install dependencies or repair settings. Keep authenticated checks opt-in and separate from
ordinary offline validation.

## Evidence and Access

Use the least-privilege read access needed for the selected observations. Distinguish an observable
absence from authentication failures, ambiguous not-found responses, omitted fields, rate limits,
network errors, and incomplete pagination. An unavailable protection source is not evidence that
protection is absent. Preserve affirmative observations while disclosing incomplete coverage.

Record whether evidence describes effective rules or merely declared policy. Identify the observed
branch and revision for file-based controls; presence on a default branch does not establish
presence on every branch. Match required contexts exactly and inspect source identity separately
when it is part of the policy. Record observation time: URLs to mutable hosted resources are not
immutable snapshots. Retain sanitized evidence in storage appropriate to its sensitivity.

## Interpret Results

- Confirmed match: an observable expectation matches; this does not prove every enforcement path.
- Confirmed drift: an observable mismatch or absent expected object is confirmed.
- Insufficient evidence: permissions, ambiguity, omitted fields, or incomplete responses prevent a
  conclusion.
- Approved exception: confirmed drift has an applicable reviewed, unexpired exception; access gaps
  remain gaps.

Record observation time, exact scope, sanitized details, API evidence, exit status, and tool
revision. Do not infer current enforcement, source-App identity, administrator bypass behavior,
notification delivery, or a monitored mailbox from configuration presence. Check representative
execution and blocking separately.

## Exceptions and Follow-Up

Assign follow-up ownership and retain dated observations. Exceptions need exact scope, rationale,
compensation, approval evidence, and expiry. Verify approval legitimacy through the owner’s review process; a tool accepting an approval URL or
approver field does not authenticate that approval. Close corrected or expired exceptions through
review. Missing access remains an evidence gap and cannot be converted into an approved deviation.

Request remediation separately; an audit is not
authorization for hosted writes, caller dispatches, or test reports.
