<!--
engineering/git/gitflow.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# GitFlow with Protected Branches

This is an optional model for projects that explicitly adopt GitFlow. Branch-neutral projects retain
their own routing. The consuming repository owns exact prefixes, integration branches, supported
release lines, and hosted checks.

Feature and bugfix branches normally target the development branch; release and hotfix branches
target the stable/default branch. Use reviewed hosted pull requests as the authoritative integration
path. Local `git flow ... finish` may merge into protected branches locally and should not replace
hosted review. After a verified hosted merge, clean up local branches without pushing local
integration merges.

For releases, stabilize scope, validate the candidate, review compatibility and artifacts, then
integrate through the required PR route. Tag only the authorized authoritative commit. Hotfixes need
an explicit path back to development and other maintained lines. Synchronize the default branch back
through a reviewed PR rather than bypassing protections. Support branches need an agreed maintenance
and backport strategy.

A solo maintainer cannot independently approve their own change. Record the review/enforcement
limitation and narrow recovery exceptions rather than pretending another approval exists. Keep
branch commands, required contexts, signing/distribution, deployment, and release mechanics local.
