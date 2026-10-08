<!--
engineering/templates/shared-automation-adoption.md
Dagitali organization documentation

Responsibilities
- Provide a blank shared automation adoption template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Shared Automation Adoption Template

Complete in the consumer's maintainer records. Keep private hosted settings and vulnerability
details restricted.

- [Adoption Record](#adoption-record)
- [Review Boundaries](#review-boundaries)

## Adoption Record

| Field | Record |
| --- | --- |
| Consumer, owner, review date | |
| Shared component and reviewed immutable revision | |
| Caller paths and copied starter revision | |
| Local policies, licenses, and intentional overrides | |
| Runtime, commands, directories, event coverage | |
| Permissions, environments, credentials, artifacts, cancellation | |
| Exact required check names and merge-group coverage | |
| Local checks and representative hosted caller evidence | |
| Hosted access, owners, rules, bypasses, notification verification | |
| Prior known-good revision and rollback | |
| Passed, failed, skipped, inaccessible, outstanding evidence | |
| Follow-up owner and next review | |

## Review Boundaries

Mark unsupported or unverified behavior explicitly. Adoption of defaults, copied starters, and
shared references are distinct operations. A checklist does not authorize hosted writes or consumer
migration.
