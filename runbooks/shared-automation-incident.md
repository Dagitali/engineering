<!--
engineering/runbooks/shared-automation-incident.md
Dagitali organization documentation

Responsibilities
- Guide affected-consumer assessment, recovery, and disclosure.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Shared Automation Incident Response

Use this procedure for suspected compromise or defects in released workflows, actions, and
dependency pins. Begin through the affected component's private reporting route; keep exploit
details and sensitive evidence out of public records. The component's local runbook owns concrete
recovery commands and affected paths.

- [Triage and Scope](#triage-and-scope)
- [Containment and Recovery](#containment-and-recovery)
- [Corrected Immutable Revision](#corrected-immutable-revision)
- [Consumer Migration or Rollback](#consumer-migration-or-rollback)
- [Disclosure and Closure](#disclosure-and-closure)

## Triage and Scope

Identify the suspect revision, changed interfaces, credentials reachable by the workflow, known
callers, and previous known-good immutable revision. Distinguish confirmed impact from unknown
adoption.

## Containment and Recovery

Assign containment and disclosure owners before separately authorized caller, credential, or hosted
changes. Preserve sensitive evidence in restricted storage and confirm a safe recovery revision
before rollout; a previously successful run alone does not establish that a revision is unaffected.

## Corrected Immutable Revision

Preserve released history. Prepare a reviewed corrected immutable revision with compatibility and
migration notes, local contract checks, and representative hosted consumer evidence. Do not retarget
an immutable tag or assume a moving major tag updates all callers.

## Consumer Migration or Rollback

Roll out to known consumers in stages, recording owner, new revision, caller evidence, and rollback
revision. Verify event coverage, permissions, artifact behavior, and required-check identities.
Restore compatible callers and hosted check selections together when recovery needs both.

Before rollback, verify that the previous revision is unaffected and compatible with the consumer.
If no safe rollback exists, record that limitation and obtain the affected owner's decision on
containment or a reviewed forward fix. Keep unresolved consumers visible until recovery is verified.
Changing a caller reference does not reverse credential exposure or already-published artifacts;
track their assessment and separately authorized remediation with responsible owners and evidence.

## Disclosure and Closure

Close with the cause, affected scope, completed containment, verified migrations, unresolved
consumers, disclosure decision, and follow-up. Successful library tests do not establish consumer
recovery.
