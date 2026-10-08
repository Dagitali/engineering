<!--
engineering/languages/python.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Python Development Practices

Use explicit typed interfaces, deterministic tests, and a single authoritative package-version
source. Apply the conventions selected by the consuming project; its package configuration owns the
supported interpreter range and tool settings. Git-derived versions are an option when the project
adopts them.

Use single-quoted strings, an 88-character code line length, strict typing, and NumPy-style public
docstrings where the project adopts these conventions. Keep docstring lines within 79 characters
including indentation. Document parameters, returns, propagated exceptions, side effects, and
diagnostics returned instead of raised. Omit irrelevant sections. Keep package-root exports
intentional and public typing distributable.

Separate parsing, configuration, business logic, and reporting. Prefer immutable keyword-only
configuration where it improves validation. Validate invalid combinations at the appropriate
boundary and test useful errors. Do not turn internal modules into promised consumer APIs without a
deliberate compatibility decision.

Keep source layout and dependency metadata canonical. For projects using setuptools-scm, derive
versions from Git rather than adding another version source. Pair supported dependency lower bounds
with their compatibility fixtures. Normal unit tests should not need network access, credentials, or
deployment. Use [Python testing](../testing/python.md) and the project's documented contributor
commands.
