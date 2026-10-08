<!--
engineering/documentation/maintenance.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Documentation Maintenance

Maintain one authoritative source for each claim and link to it from related guides. Project-specific
ownership maps stay beside the implementation. Product contracts and historical release records
remain with their projects.

## Sources of Truth

| Claim | Evidence | Maintained explanations to review |
| --- | --- | --- |
| Commands and environment selection | Makefile or equivalent command definitions | Onboarding, agents, testing |
| Runtime and dependency support | Package/tool configuration and compatibility tests | Requirements, support, release notes |
| Public behavior | Implementation, interfaces, examples, contract tests | Configuration, design, changelog |
| Resources and data flow | Implementation, synthesis, persistence and migration tests | Architecture, privacy, costs, decisions |
| Workflow behavior | Triggers, jobs, permissions, pins, artifacts | CI map, runbooks, branch protection |
| Hosted enforcement | Dated hosted observations and representative blocking checks | Operational records |
| Release state | Candidate tree, tag identity, artifacts, publication evidence | Changelog and release archive |

## Change Procedure

Search for the changed name or claim, inspect its canonical evidence, and update the smallest complete
set of maintained documents. Keep local ownership maps accurate. Preserve existing anchors referenced
by other guides; retain a local adapter when centralizing a procedure. Never rewrite historical
outcomes to imply current verification.

Use descriptive reference labels, grouped at the bottom and sorted case-sensitively by destination,
then label. Prefer relative links within a repository. Keep official names, useful tables of contents,
and attribution. Wrap file-header comment lines at 79 characters; preserve language directives and URLs.
Do not edit generated documentation, caches, distributions, or lockfiles as handwritten prose.

## Verification

Run the project's Markdown destination and heading checks. Separately inspect undefined reference
labels, images, external destinations, and factual claims. Run the documentation builder when its
sources or included documents change. A local link check does not establish external availability,
hosted enforcement, clean installation, or publication.

Use the [evidence inventory](../templates/evidence-inventory.md) for material claims requiring a fuller
record, not as a mandatory gate for every small edit. Store confidential completed records in an
access-controlled system; public statements link only to evidence their audience may inspect.

A documentation task does not authorize changing implementation or external state to make a claim true.
Report discrepancies requiring a separate implementation decision.
