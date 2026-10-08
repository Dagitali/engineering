<!--
engineering/learnings/python-and-repository-tooling.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Python and Repository Tooling Lessons

Use Symptom → Cause → Fix → Verification for reusable diagnosed failures. Keep project-specific
commands and historical incident evidence in local learnings and runbooks.

| Symptom | Cause to investigate | Correction and verification |
| --- | --- | --- |
| Source tests pass but installation fails | Default suite omits artifact layers | Build/inspect wheel and sdist; test clean installation and build-on-demand |
| Minimum-dependency policy fails | Metadata lower bound differs from fixture pin | Reconcile the intended range and fixture; rerun boundary tests |
| Markdown checker passes but a label is broken | Checker covers destinations, not undefined labels or external semantics | Inspect rendering and definitions separately |
| Action pin check fails | Floating or malformed remote reference | Review upstream revision and update immutable reference; rerun policy/contracts |
| Release artifact has the wrong version | Build/tree/tag identity or source-path leakage differs | Build from authoritative candidate; compare artifact metadata and clean install |
| Historical tag fails changelog validation | Tagged tree lacks the matching dated entry | Preserve tag; prepare reviewed corrected release rather than retagging |
| Documentation promises the wrong behavior | Policy was copied from another project | Trace canonical sources and retain purposeful consumer differences |

A passing checker proves only its implemented scope. Local tests do not establish hosted enforcement
or publication. Use the [incident runbook](../runbooks/repository-ci-incident.md) for recovery.
