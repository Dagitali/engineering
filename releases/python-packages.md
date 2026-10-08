<!--
engineering/releases/python-packages.md
Dagitali organization documentation

Responsibilities
- Guide package compatibility, artifact validation, and publication evidence.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Python Package Releases

- [Compatibility and Candidate Scope](#compatibility-and-candidate-scope)
- [Artifact Validation](#artifact-validation)
- [Publication and Recovery](#publication-and-recovery)

## Compatibility and Candidate Scope

Assess the complete candidate diff and documented public contract under the project's release
policy. Commands, flags, configuration, defaults, diagnostics, exports, supported runtimes, and
generated behavior can affect compatibility. Treat stricter validation as a potential consumer
migration.

## Artifact Validation

For Git-derived versions, build from the authoritative candidate and verify the intended version in
both wheel and source distribution. Validate content and metadata, run distribution checks, and
install each format in a clean environment without source-path leakage. Use a fresh output directory
if older artifacts would mix versions. A development fallback version is not release evidence.

## Publication and Recovery

Prepare a matching dated changelog and [release notes]. Record completed/skipped tests, support
boundaries, artifact identity, migration, and rollback. Follow local integration/tag policy; keep
tags immutable. PyPI, GitHub Releases, and other publication destinations are project-specific
opt-ins, not implied by a successful build or this guide.

[release notes]: ../templates/releases/python-package.md
