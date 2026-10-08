<!--
engineering/playbooks/scaffold-consumer-project.md
Dagitali organization documentation

Responsibilities
- Guide a minimal consumer baseline and review its readiness boundaries.

Maintainer Notes
- Keep toolchains, contracts, and operational decisions consumer-owned.
-->

# Scaffold a Consumer Project

Create the smallest reviewable project that demonstrates the intended use of a shared component. Use
the consumer's local instructions and actual requirements; this playbook does not prescribe a
universal repository layout or authorize deployment.

- [Define Ownership](#define-ownership)
- [Choose the Smallest Example](#choose-the-smallest-example)
- [Create the Baseline](#create-the-baseline)
- [Validate Without Deploying](#validate-without-deploying)
- [Production Readiness](#production-readiness)

## Define Ownership

Identify the consumer's purpose, public contract, maintainer, contribution terms, supported
toolchain, configuration authority, and review route. Assign ownership for data, external services,
identity, delivery, monitoring, cost, and recovery where applicable. Keep private identifiers and
completed operational records outside this shared checkout.

## Choose the Smallest Example

Select one supported composition that demonstrates a real requirement. Use neutral fixtures and
consumer-owned configuration; do not copy another project's accounts, domains, credentials, product
promises, or deployment-test resources. For an existing project, inspect its current baseline and
migration needs rather than treating it as a new scaffold.

## Create the Baseline

1. Select a reviewed immutable shared-component revision and the consumer's supported toolchain.
2. Keep configuration in the consumer's established layer and declare required inputs explicitly.
3. Add deterministic checks for demonstrated behavior, invalid inputs, and important boundaries.
4. Document actual setup and validation commands, their dependencies, and side effects.
5. Copy only relevant [templates], replacing fields and verifying paths before use. Record durable
   decisions when alternatives and consequences warrant them.

Use [repository policy checks] when selecting validators or replacing existing scripts. Preserve
intentional consumer differences and coverage that replacement tools do not provide.

## Validate Without Deploying

Run the consumer's applicable local checks using sanitized inputs and isolated output directories.
Inspect generated artifacts or synthesized resources when those are part of the contract. Review
permissions, resource identity/lifecycle, compatibility, and migration effects where applicable. Use
[infrastructure testing] and [CDK change safety] for infrastructure consumers. Record results and
limitations; local success does not establish hosted access, deployed behavior, or publication.

## Production Readiness

Before delivery, assign the production environment, reviewed identity, change approval, smoke tests,
monitoring, budget decisions, retained-state ownership, and recovery verification as applicable. For
existing resources or data, compare the intended changes and migration path through the consumer's
authorized review process. Keep concrete operational commands and thresholds local. Use [release
evidence] to distinguish preparation from actual delivery. If deployed compatibility needs a
disposable test, apply the separately authorized [cloud test boundaries].

[repository policy checks]: ../automation/repository-policy.md
[CDK change safety]: ../infrastructure/cdk-change-safety.md
[release evidence]: ../releases/evidence-and-history.md
[templates]: ../templates/README.md
[cloud test boundaries]: ../testing/disposable-cloud-tests.md
[infrastructure testing]: ../testing/infrastructure.md
