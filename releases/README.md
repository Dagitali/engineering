<!--
engineering/releases/README.md
Dagitali organization documentation

Responsibilities
- Index candidate verification and platform-specific release templates.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Release Guidance

Use the released component's own integration, versioning, support, and delivery policy. This
directory contains reusable procedures and this collection’s own [release archive]. Consumer release
records belong with their projects. Follow the [repository release policy] for this collection and
the [release playbook] for a reusable sequence.

- [Evidence and Identity](#evidence-and-identity)
- [Platform Guides](#platform-guides)
- [Record Templates](#record-templates)

## Evidence and Identity

Start with [release evidence] to distinguish preparation, tags, validation, publication, and
consumer rollout. Keep outcomes tied to their exact revision and artifact.

## Platform Guides

- [Python packages]: Compatibility, wheel/sdist validation, and publication evidence.
- [Apple apps]: Signed builds, beta acceptance, and public-release readiness.
- [Shared automation]: Interface versioning, hosted callers, and consumer migration.

## Record Templates

Choose the [Python notes], [Apple notes], or [automation notes] template. Keep this checkout's forms
blank and use actual outcomes in the owning project. The [template catalog] also contains release
checklists and verification records.

[repository release policy]: ../RELEASE-POLICY.md
[release playbook]: ../playbooks/release.md
[template catalog]: ../templates/README.md
[Apple notes]: ../templates/releases/apple-app.md
[Python notes]: ../templates/releases/python-package.md
[automation notes]: ../templates/releases/shared-automation.md
[Apple apps]: apple-apps.md
[release evidence]: evidence-and-history.md
[release archive]: history/README.md
[Python packages]: python-packages.md
[Shared automation]: shared-automation.md
