<!--
engineering/development/onboarding.md
Dagitali organization documentation

Responsibilities
- Explain developer onboarding and verification boundaries.

Maintainer Notes
- Preserve consumer-owned commands, configuration, and policy.
-->

# Developer Onboarding

- [Prerequisites](#prerequisites)
- [First Local Session](#first-local-session)
- [Learn the Repository](#learn-the-repository)
- [Safe Learning Path](#safe-learning-path)
- [Pull Request Expectations](#pull-request-expectations)

## Prerequisites

Use Git and a Markdown editor. Read the [contributor guide] for optional tools and setup. This
checkout has no application build, package installation requirement, or cloud-account prerequisite
for editing documentation. Tool installation and initial hook execution may need network access.

## First Local Session

Inspect the checkout before editing:

```sh
git status --short
git diff --stat
```

Read the [repository instructions] and preserve existing work. Choose a bounded documentation change
and locate its canonical evidence. Follow [local setup] if using optional hooks; installation
changes local Git configuration and is separate from editing files.

## Learn the Repository

Use [Architecture] for ownership and layout, [Design] for content constraints, and the
[documentation index] for maintenance. Distinguish reusable topic guidance from root repository
policies and historical records. Source templates stay blank; completed forms belong with their
consumers. The [onboarding template] supports separate project-specific onboarding.

## Safe Learning Path

Try the [adoption tutorial] with disposable fixtures. Review a tool’s inputs, dependencies, and side
effects before running it. Follow the [validation procedure] for this checkout; do not assume a
sibling’s commands or installed environment are available. Use [testing guidance] for consumer
validation layers. Avoid publishing, tagging, or changing hosted settings as a learning exercise.

## Pull Request Expectations

Follow the [pull request guidance]. Explain source accuracy, adoption effects, actual checks, and
limitations. Preserve stable links, attribution, and historical evidence. Use the [incident runbook]
when a failure requires diagnosis.

[repository instructions]: ../AGENTS.md
[Architecture]: ../ARCHITECTURE.md
[contributor guide]: ../CONTRIBUTING.md
[local setup]: ../CONTRIBUTING.md#local-setup-and-hooks
[pull request guidance]: ../CONTRIBUTING.md#pull-requests
[validation procedure]: ../CONTRIBUTING.md#validation
[Design]: ../DESIGN.md
[documentation index]: ../documentation/README.md
[adoption tutorial]: ../documentation/adopt-markdown-check.md
[incident runbook]: ../runbooks/repository-ci-incident.md
[onboarding template]: ../templates/developer-onboarding.md
[testing guidance]: ../testing/README.md
