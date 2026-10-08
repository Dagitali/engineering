<!--
engineering/interfaces/evolution-checklist.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Interface Evolution Checklist

Review documented commands, configuration, types, defaults, outputs, error behavior, automation inputs,
and generated resources as consumer contracts. A stricter validator can break consumers without changing
its command name.

- Identify the demonstrated need, owner, current contract, and affected consumers.
- Classify the change as additive, behavior-changing, deprecating, or breaking under local release policy.
- Specify valid/invalid inputs, defaults, failure behavior, compatibility, and migration before implementation.
- Preserve intentional exports, read-only guarantees, resource identities, and consumer ownership where promised.
- Test successful, invalid, missing-input, and boundary behavior through the real public entry point.
- Verify installed interfaces or synthesized resources when those boundaries change.
- Synchronize examples, configuration references, architecture, changelog, and affected release guidance.
- Report evidence, limitations, migration, and rollback; do not invent support guarantees.

Keep concrete API names, CLI dispatch cases, synthesis assertions, and validation commands in the project.
Use its [change impact map template](../templates/change-impact-map.md) structure to identify the complete scope.
