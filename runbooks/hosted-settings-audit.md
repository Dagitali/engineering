<!--
engineering/runbooks/hosted-settings-audit.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Hosted Settings Audit

Compare explicit repository expectations with authenticated, read-only hosted observations. Keep
inventory, expected contexts, reviewed tool revision, and exact invocation in the consuming
project's configuration. The selected audit tool's maintained reference owns its schema and exact
result names.

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

Keep credentials outside the report. Store private operator details in restricted records. Use the
installed reviewed tool through the consuming project's reproducible environment; audits must not
silently install dependencies or repair settings. Keep authenticated checks opt-in and separate from
ordinary offline validation.

Assign follow-up ownership and retain dated observations. Exceptions need exact scope, rationale,
compensation, approval evidence, and expiry. Request remediation separately; an audit is not
authorization for hosted writes, caller dispatches, or test reports.
