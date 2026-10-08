<!--
engineering/infrastructure/cdk-change-safety.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide resource identity, migration, and synthesis review.

Responsibilities
- Guide resource identity, migration, and synthesis review.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# CDK Change Safety

Review synthesized infrastructure as a public behavior boundary. Prefer stable constructs and typed
properties; document lower-level overrides when necessary. Validate configuration before resource
creation.

- [Resource Identity and Migration](#resource-identity-and-migration)
- [Consumer Boundaries](#consumer-boundaries)
- [Cost and Retained Resources](#cost-and-retained-resources)
- [Production Readiness](#production-readiness)
- [Operational Verification](#operational-verification)

## Resource Identity and Migration

Preserve stateful construct identities. Renaming or moving a construct can change logical IDs and
replace resources; compare synthesis and the authorized deployment diff before accepting a
migration. Examine IAM, public access, encryption/TLS, DNS, retention, update/delete policies,
custom resources, availability, and cost. A removal policy is not proof that non-empty storage will
be deleted or retained exactly as expected.

## Consumer Boundaries

Keep reusable constructs separate from consumer accounts, regions, deployment identity, content,
APIs, monitoring, and budgets. Use examples and regression assertions for the supported composition.
Product requirements such as certificate region, bucket defaults, and OAC stay in the construct's
local contract.

## Cost and Retained Resources

Retained resources can continue incurring charges after a stack is removed. Identify the owner of
retained data/resources, review cost drivers and lifecycle behavior, and assign budget/alert and
eventual cleanup decisions at the consumer's appropriate account, project, or resource boundary.
Recheck estimates when usage or enabled features change using current service pricing. A reusable
construct does not establish ownership of account-wide spending or authorize cleanup.

## Production Readiness

Before production deployment, record the intended environment and reviewed deployment identity,
change approval, expected resource/data effects, smoke tests, monitoring, budget decisions, and
retained-resource ownership. Define rollback or a forward-fix path and how recovery will be
verified. Keep concrete commands, thresholds, identities, and operational records with the consumer.
Local synthesis and tests are preparation evidence; separately verify the deployed candidate and its
recovery behavior where authorized.

## Operational Verification

Synthesis is a local validation step; deployments, destruction, DNS changes, and cloud recovery
require separate authority. Record migration and rollback ownership before operations affecting
existing data.
