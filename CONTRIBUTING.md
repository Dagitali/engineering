<!--
engineering/CONTRIBUTING.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Explain contribution terms, editing conventions, and local validation.

Responsibilities
- Explain contribution terms, editing conventions, and local validation.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Contributing to Organization Documentation

- [Before You Begin](#before-you-begin)
- [Ways to Contribute](#ways-to-contribute)
- [First Contribution](#first-contribution)
- [Community Standards](#community-standards)
- [Contribution Terms](#contribution-terms)
- [Documentation Conventions](#documentation-conventions)
- [Local Setup and Hooks](#local-setup-and-hooks)
- [Validation](#validation)
- [Pull Requests](#pull-requests)

## Before You Begin

Search existing issues and pull requests before proposing a change. For substantial documentation
changes, describe the affected guidance and rationale in an existing relevant discussion or a draft
pull request for maintainer review. Use the repository's available contribution channels; this guide
establishes no new reporting service. Read the owning project's instructions when a proposal affects
its contracts, and use its private reporting route for suspected vulnerabilities.

## Ways to Contribute

Correct inaccurate guidance, repair links, improve examples, report sanitized adoption problems, and
propose reusable templates supported by demonstrated need. Explain the affected contract and
canonical evidence. Keep project-specific policy and completed private records with their owners.

## First Contribution

Use [developer onboarding] for a first local session and repository orientation.

1. Read the README, [repository instructions], and contribution terms below. Inspect the working
   tree and preserve unrelated changes.
2. Use an authorized checkout and create a topic branch from the repository's agreed base branch.
   Follow its naming and review policy; the shared GitFlow option is not a required branch model.
3. Make a focused edit using the documentation conventions below. Keep templates blank and preserve
   notices, existing anchors, and historical evidence.
4. Follow [local setup] and [validation], inspect the diff, and record results and skipped checks.
5. When submission is authorized, open a PR against the agreed base branch using the [PR guidance].
   Use a draft for early feedback and address review findings.

## Community Standards

Follow the [Code of Conduct]. Use the [support guide] for help and the [security policy] for
sensitive findings. Public contributions must omit confidential project content and personal data.

## Contribution Terms

Keep edits focused and ground claims in their owning repository. Preserve project-specific
licensing, privacy, support, branch routing, release contracts, and dated evidence. Source
attribution and notices are maintained in [NOTICE] and [NOTICES.md]. Contributions submitted for
inclusion in this repository are provided under its [MIT License]. Submit only material you are
authorized to license under those terms, and retain applicable third-party attribution and notices.

## Documentation Conventions

Use descriptive headings, relative links within this checkout, and sorted bottom reference
definitions. Use descriptive reference labels for document and external-resource links, reusing a
definition for repeated destinations. Keep compact, one-use navigation links inline when converting
a dense catalog would add excessive definition lines. Group definitions at the bottom and sort by
destination exactly as written (case-sensitive), then by label. Preserve destination casing,
fragments, and encoding. Keep table-of-contents anchors inline and literal link syntax in fenced
examples unchanged. Keep file-header comment lines within 79 characters. Include the copyright line
and a short description specified by [documentation maintenance], preserving front matter and source
notices. Templates retain explicit replacement fields; maintained guides should contain actual
instructions and links. Run Markdown destination/anchor and reference checks; inspect external
claims separately. Update README navigation for new topics.

Use repository-relative links for local documents and verified canonical URLs for shared resources.
Keep reusable guidance independent of its originating project. Examples should use replacement
fields or neutral fixtures; migration inventories and completed source-specific records belong
outside this repository. Validate local destinations, heading anchors, reference labels, and source
independence before integration.

## Local Setup and Hooks

Use Git and a Markdown editor. Read the [repository instructions] and inspect `git status` before
editing. This checkout has no Makefile, documentation-site builder, or pinned Python validation
environment; commands from sibling repositories are not its local quality gate.

Optional hooks use pre-commit 4.0.0 or newer and the tools pinned in the [hook configuration].
Prepare pre-commit in your chosen tool environment, then validate its configuration:

```sh
pre-commit validate-config
```

To install the configured commit-message, pre-commit, and pre-push hooks deliberately, run
`pre-commit install`. Installation changes local Git hooks. Initial hook execution can download
repositories and create tool environments; setup needs network access when they are not cached.

## Validation

For configured checks, run `pre-commit run --all-files` on your working branch. Some hooks can
rewrite files, including table-of-contents updates; inspect the resulting diff. The branch hook
rejects commits on `main` and `develop`. Commit-message validation runs separately at its configured
stage. These hooks do not replace Markdown destination, anchor, and reference-label review.

If a reviewed Popo installation is already available in your selected Python environment, run:

```sh
python -m popo check-docs --root .
```

This optional command checks local Markdown destinations and heading anchors; it does not install
Popo or establish external URL availability. Review undefined reference labels, definition sorting,
template placeholders, source notices, and factual accuracy separately. Run `git diff --check` and
inspect the complete diff. Record tool versions, actual checks, failures, and skipped checks. Use
[documentation maintenance] for source-of-truth and evidence boundaries.

## Pull Requests

Keep changes focused on the documented need. Use the repository's agreed branch and review route;
the shared [GitFlow guide] is optional and does not establish this checkout's branching model.
Describe the resulting guidance, affected links or templates, validation, and remaining limitations.
Preserve existing anchors and historical records. Commits, pushes, publication, and hosted changes
require task authority; documentation edits alone do not authorize them.

[hook configuration]: .pre-commit-config.yaml
[repository instructions]: AGENTS.md
[Code of Conduct]: CODE_OF_CONDUCT.md
[local setup]: CONTRIBUTING.md#local-setup-and-hooks
[PR guidance]: CONTRIBUTING.md#pull-requests
[validation]: CONTRIBUTING.md#validation
[MIT License]: LICENSE
[NOTICE]: NOTICE
[NOTICES.md]: NOTICES.md
[security policy]: SECURITY.md
[support guide]: SUPPORT.md
[developer onboarding]: development/onboarding.md
[documentation maintenance]: documentation/maintenance.md
[GitFlow guide]: git/gitflow.md
