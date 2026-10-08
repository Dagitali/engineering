<!--
engineering/development/agent-assisted-workflow.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Agent Assisted Development Workflow

Use design discussion to clarify a decision and repository inspection to establish current behavior.
This process applies regardless of the assistant or editor. The project's local instructions define
its contracts, commands, and safety boundaries.

- [Explore the Decision](#explore-the-decision)
- [Ground the Work](#ground-the-work)
- [Prepare the Handoff](#prepare-the-handoff)
- [Execute and Verify](#execute-and-verify)

## Explore the Decision

Identify the outcome, alternatives, constraints, non-goals, and observable acceptance criteria.
Consider compatibility, privacy, accessibility, failure behavior, maintenance cost, and migration.
Separate accepted requirements from unresolved suggestions. A conversation is not implementation
evidence.

## Ground the Work

Read applicable instructions, current source, tests, configuration, and maintained documentation.
Inspect the working tree and preserve unrelated or staged changes. Trace commands to their
definitions, supported versions to configuration, and automation claims to workflow declarations and
hosted evidence. Resolve conflicts before expanding scope. Diagnosis does not authorize an
implementation change.

## Prepare the Handoff

Record the desired outcome, relevant paths, observed behavior, alternatives, constraints, acceptance
criteria, and validation plan. Use the [task template](../templates/development-task.md). Keep
private source, credentials, and confidential diagnostics out of public briefs.

## Execute and Verify

1. State the smallest complete file scope and appropriate checks.
2. Implement one coherent change while preserving local contracts and purposeful policy differences.
3. Run focused checks, then the project's applicable quality gate. Packaging needs artifact and
   clean-install evidence; synthesis and source tests do not prove deployed or signed behavior.
4. Follow [documentation maintenance](../documentation/maintenance.md) to update affected explanations.
5. Review the diff for unrelated edits, generated output, private data, and stale claims.
6. Report changed files, evidence, passed/failed/skipped checks, and outstanding work.

Record durable decisions and reusable failures where the project maintains them. Repository edits do
not implicitly authorize commits, tags, publication, hosted settings changes, or deployment.
