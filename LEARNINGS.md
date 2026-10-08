<!--
engineering/LEARNINGS.md
Dagitali organization documentation

Responsibilities
- Explain learnings and its ownership boundaries.

Maintainer Notes
- Link canonical guidance and preserve purposeful project differences.
-->

# Learnings

- [Reusable Lessons](#reusable-lessons)
- [Recording a Lesson](#recording-a-lesson)
- [From Diagnosis to Recovery](#from-diagnosis-to-recovery)

## Reusable Lessons

Start with [tooling lessons] for artifact-layer gaps, dependency drift, Markdown-check limits,
action pins, release identity, and copied-policy mistakes. Detailed lessons remain at their existing
paths so established links continue to work.

## Recording a Lesson

Describe the symptom, demonstrated cause, correction, and verification. Separate a hypothesis from a
confirmed diagnosis. Include the affected boundary and limitations; keep private source,
identifiers, and incident evidence with the owning project.

## From Diagnosis to Recovery

Use the [incident runbook] for recovery and [maintenance guidance] for synchronized explanations. A
reusable lesson informs review; it does not prove that every consumer has the same cause or
authorize operational changes.

[maintenance guidance]: documentation/maintenance.md
[tooling lessons]: learnings/python-and-repository-tooling.md
[incident runbook]: runbooks/repository-ci-incident.md
