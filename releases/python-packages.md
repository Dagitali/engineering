<!--
engineering/releases/python-packages.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Python Package Releases

Assess the complete candidate diff and documented public contract under the project's release policy.
Commands, flags, configuration, defaults, diagnostics, exports, supported runtimes, and generated behavior
can affect compatibility. Treat stricter validation as a potential consumer migration.

For Git-derived versions, build from the authoritative candidate and verify the intended version in both
wheel and source distribution. Validate content and metadata, run distribution checks, and install each
format in a clean environment without source-path leakage. Use a fresh output directory if older artifacts
would mix versions. A development fallback version is not release evidence.

Prepare a matching dated changelog and [release notes](../templates/releases/python-package.md). Record
completed/skipped tests, support boundaries, artifact identity, migration, and rollback. Follow local
integration/tag policy; keep tags immutable. PyPI, GitHub Releases, and other publication destinations are
project-specific opt-ins, not implied by a successful build or this guide.
