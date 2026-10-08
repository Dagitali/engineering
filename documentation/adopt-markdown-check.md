<!--
engineering/documentation/adopt-markdown-check.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Demonstrate a local documentation check and deliberate failure recovery.

Responsibilities
- Demonstrate a local documentation check and deliberate failure recovery.

Maintainer Notes
- Keep experiments disposable and actual adoption consumer-owned.
-->

# Adopt a Local Markdown Check

Try a documentation validator against neutral files before selecting it for a consumer. This
exercise uses Popo as an example, not a required organization tool. Keep the experiment outside this
checkout and real consumer records.

- [Prepare the Environment](#prepare-the-environment)
- [Create the Example](#create-the-example)
- [Verify the Baseline](#verify-the-baseline)
- [Diagnose and Repair](#diagnose-and-repair)
- [Review Adoption](#review-adoption)

## Prepare the Environment

Use an isolated Python environment with a reviewed Popo installation, prepared through the selected
release's documented installation process. Confirm its supported interpreter before installation;
setup may require network access. Keep that environment selected for these commands:

```sh
python -m popo --version
python -m popo check-docs --help
```

Record the tool version. The example needs no Git initialization, Python project metadata, cloud
identity, or hosted changes. The check reads local files.

## Create the Example

Create a new disposable folder in your editor. Add `README.md` containing:

```markdown
# Example Documentation

Read the [guide].

[guide]: guide.md#overview
```

Add `guide.md` containing:

```markdown
# Overview

This is a neutral documentation fixture.
```

## Verify the Baseline

Replace the example path with the absolute path to your disposable folder:

```sh
python -m popo check-docs --root "/absolute/path/to/example"
```

Expect `PASS: local Markdown links are valid` and exit status `0`. Confirm the command has not
modified either file. Review reference-label resolution separately; this check does not establish
external URL availability, image-link coverage, or factual accuracy.

## Diagnose and Repair

Change `# Overview` in `guide.md` to `# Introduction` without changing the reference definition.
Rerun the same command. Expect exit status `1` and an anchor diagnostic identifying
`guide.md#overview`. Preserve the failure as evidence of the check's coverage.

Change the definition to `[guide]: guide.md#introduction`, then rerun. Expect exit status `0` and
the original success message. You made the repair; the validator reported the mismatch.

## Review Adoption

Use [repository policy checks] to compare the selected validator with existing consumer checks
before integrating it. Retain unsupported coverage and verify known-good and known-bad inputs. Keep
the same selected invocation and exit-status handling locally and in any separately reviewed CI
change. Use [documentation maintenance] to review labels, sources, and evidence limits. This
tutorial does not replace consumer setup instructions or authorize changes to its gates.

[repository policy checks]: ../automation/repository-policy.md
[documentation maintenance]: maintenance.md
