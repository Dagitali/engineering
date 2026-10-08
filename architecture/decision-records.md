<!--
engineering/architecture/decision-records.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Explain durable decision records and preservation of their history.

Responsibilities
- Explain durable decision records and preservation of their history.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Architecture Decision Records

- [When to Record a Decision](#when-to-record-a-decision)
- [Record Structure](#record-structure)
- [Superseding Decisions](#superseding-decisions)

## When to Record a Decision

Record durable decisions when alternatives and consequences will matter to future maintainers. Keep
project-specific records beside the implementation and preserve their historical context.

## Record Structure

Use the [decision template]: context, decision, alternatives, consequences, ownership, status,
verification, and references. Name the accepted boundary and its tradeoffs; do not substitute a
broad tutorial for the decision. Assign a stable identifier according to project convention.

## Superseding Decisions

When superseding a decision, link its replacement and retain the original record. Changes in
observed behavior belong in current implementation and guides; historical records should not be
rewritten to imply later verification. Do not create empty decision records solely to mirror another
repository's tree.

[decision template]: ../templates/architecture-decision.md
