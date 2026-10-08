<!--
engineering/runbooks/repository-ci-incident.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Repository and CI Incident Response

Diagnose repository checks, CI, artifacts, and release failures from the exact failing revision.
Project runbooks supply commands and component-specific recovery steps.

1. Identify workflow, job, step, commit/tag, artifact, and the first meaningful error. A failed wrapper
   target may only report a downstream symptom.
2. Inspect current checkout and working-tree state before reproducing. Separate historical failure
   evidence from a successful run of today's branch.
3. Reproduce with the narrowest safe local diagnostic. Distinguish tool/environment failures from
   configuration, dependency, source, and test-contract failures.
4. Restore the intended contract through a reviewed correction. Do not weaken assertions or policy
   merely to obtain a pass. Use isolated temporary artifacts instead of deleting unrelated output.
5. Verify the focused failure, applicable local gate, and separately authorized hosted results.
6. Record cause, impact, correction, evidence, skipped checks, and outstanding work.

Check dependency lower bounds against compatibility fixtures; source tests against clean artifact
installation; tag-derived versions against the tagged tree and dated changelog. Preserve immutable tags
and prepare a corrected release when appropriate. A workflow declaration does not establish hosted
publication, environment reviewers, or branch protection. Reruns, settings changes, secret access,
publication, and external cleanup need separate authority.
