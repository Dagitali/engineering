<!--
engineering/runbooks/shared-automation-incident.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Shared Automation Incident Response

Use this procedure for suspected compromise or defects in released workflows, actions, and dependency pins.
Begin through the affected component's private reporting route; keep exploit details and sensitive evidence
out of public records. The component's local runbook owns concrete recovery commands and affected paths.

Identify the suspect revision, changed interfaces, credentials reachable by the workflow, known callers,
and previous known-good immutable revision. Distinguish confirmed impact from unknown adoption. Assign
containment and disclosure owners before separately authorized caller, credential, or hosted changes.

Preserve released history. Prepare a reviewed corrected immutable revision with compatibility and migration
notes, local contract checks, and representative hosted consumer evidence. Do not retarget an immutable tag
or assume a moving major tag updates all callers.

Roll out to known consumers in stages, recording owner, new revision, caller evidence, and rollback revision.
Verify event coverage, permissions, artifact behavior, and required-check identities. Restore compatible
callers and hosted check selections together when recovery needs both.

Close with the cause, affected scope, completed containment, verified migrations, unresolved consumers,
disclosure decision, and follow-up. Successful library tests do not establish consumer recovery.
