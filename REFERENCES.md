<!--
engineering/REFERENCES.md
Dagitali organization documentation

Responsibilities
- Index canonical local guidance and upstream documentation formats.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Engineering References

Use owning configuration and implementation for current behavior. These references provide
navigation and interpretation; they do not select tool versions or change consumer policy.

- [Repository Guidance](#repository-guidance)
- [Engineering Topics](#engineering-topics)
- [Tools and Formats](#tools-and-formats)

## Repository Guidance

- [Contributor guide]: Local setup, editing conventions, and validation.
- [Documentation maintenance]: Sources of truth and link/evidence review.
- [Template catalog]: Blank reusable instructions and verification records.

## Engineering Topics

- [Development index]: Planning, review, onboarding, and adoption learning.
- [Testing index]: Boundary-focused checks and operational evidence.
- [Release index]: Candidate identity, publication state, and platform guides.
- [Workflow trust]: Identity, untrusted inputs, and validation limits.

## Tools and Formats

- [CommonMark]: Markdown syntax specification.
- [GitHub Flavored Markdown]: GitHub's Markdown dialect specification.
- [pre-commit]: Hook configuration and command documentation.

Check behavior against the consuming project's selected tools and renderer. Format references do
not establish that a particular validator implements every syntax or checks every destination.

[Contributor guide]: CONTRIBUTING.md
[Development index]: development/README.md
[Documentation maintenance]: documentation/maintenance.md
[GitHub Flavored Markdown]: https://github.github.com/gfm/
[pre-commit]: https://pre-commit.com/
[CommonMark]: https://spec.commonmark.org/
[Release index]: releases/README.md
[Workflow trust]: security/workflow-trust-boundaries.md
[Template catalog]: templates/README.md
[Testing index]: testing/README.md
