<!--
engineering/templates/developer-onboarding.md
Dagitali organization documentation

Responsibilities
- Provide a blank developer onboarding template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Developer Onboarding Template

Complete prerequisites and commands from the consuming repository's actual configuration.

- [Prerequisites](#prerequisites)
- [First Local Session](#first-local-session)
- [Learn the Repository](#learn-the-repository)
- [Safe CLI Learning Path](#safe-cli-learning-path)
- [Contribution](#contribution)

## Prerequisites

`<Git, shell/build tools, supported runtime authority, platform requirements, install/network
boundaries>`.

## First Local Session

1. Read `<instructions, overview, architecture, design, contribution guide>`.
2. Inspect the working tree and preserve unrelated work.
3. Use `<documented setup>` in an appropriate isolated environment.
4. Inspect `<environment report>` and run `<quality gate>`.
5. Learn with `<small deterministic example>`; do not use production data or deploy as a learning
   shortcut.

## Learn the Repository

`<Canonical documentation index, implementation entry points, configuration authorities, test
layers/fixtures, and source-to-test ownership map>`. Trace one relevant behavior from its public
entry point through implementation and tests. Use the owning configuration to select focused checks
rather than copying another project's commands.

## Safe CLI Learning Path

`<Harmless deterministic example, explicit input/root, expected output and exit status, side
effects, credential/network requirements, and failure interpretation>`. Use disposable sanitized
inputs and identify whether the command only inspects or also changes files. A failed check is
evidence to investigate, not permission to rewrite policy or bypass gates. Keep production
operations and publication outside the learning exercise.

## Contribution

`<Branch routing, review, focused checks, affected documentation, local terms, support route>`.
Record skipped checks and evidence limits. Installing hooks, dependencies, or tools is an explicit
setup step, not an implicit side effect of validation.
