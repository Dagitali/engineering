<!--
engineering/templates/development-task.md
Dagitali organization documentation

Responsibilities
- Provide a blank development task templates template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Development Task Templates

Replace fields and remove irrelevant constraints. One brief should produce one coherent reviewable
result.

- [Implement or Refactor](#implement-or-refactor)
- [Architecture or Interface Review](#architecture-or-interface-review)
- [Documentation Synchronization](#documentation-synchronization)
- [CI Maintenance](#ci-maintenance)
- [Incident Diagnosis](#incident-diagnosis)

## Implement or Refactor

```text
Implement <outcome> in <paths>. Inspect local instructions and the working tree first.
Preserve unrelated work and contracts outside scope.
Constraints: <compatibility, security, privacy, accessibility, data, lifecycle, non-goals>.
Acceptance: <observable behavior and verification>.
Run <focused checks> and <applicable broader gate>; update affected maintained documentation.
Report changed files, evidence, results, skipped checks, migration, and remaining work.
Do not commit, publish, tag, deploy, or change hosted settings unless authorized by the task.
```

## Architecture or Interface Review

```text
Review <proposal> against source, tests, configuration, and current docs. Compare <alternatives>.
Assess public contracts, malformed inputs, failure behavior, ownership, migration, and rollback.
Where applicable inspect resource replacement, permissions, retention, availability, and cost.
Do not edit. Return evidence-backed findings, unresolved questions, and a recommended decision.
```

## Documentation Synchronization

```text
Verify <claim> against canonical sources and update <maintained paths>.
Preserve local policies, anchors, notices, and historical outcomes. Do not edit generated output.
Run <Markdown checks and applicable builder>. Review undefined labels and factual accuracy separately.
Report mismatches requiring an implementation task; do not change behavior to make the prose true.
```

## CI Maintenance

```text
Update <workflow behavior> in <paths>. Inspect events, conditions, check names, permissions,
pins, commands, artifacts, and tests. Preserve ordinary validation and local branching policy.
Run <checks>. Synchronize CI map, branch protection, runbooks, and release notes as affected.
Distinguish local validation from hosted verification; external operations require task authority.
```

## Incident Diagnosis

```text
Diagnose <failure> from <revision/artifact>. Start read-only and identify the first meaningful error.
Separate environment, configuration, product, and policy defects. Avoid exposing private diagnostics.
Return cause, supporting evidence, containment/recovery options, verification, and follow-up.
Do not rerun hosted jobs, delete artifacts, move tags, publish, or change external state implicitly.
```
