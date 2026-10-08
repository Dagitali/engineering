<!--
engineering/infrastructure/cdk-change-safety.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# CDK Change Safety

Review synthesized infrastructure as a public behavior boundary. Prefer stable constructs and typed
properties; document lower-level overrides when necessary. Validate configuration before resource creation.

Preserve stateful construct identities. Renaming or moving a construct can change logical IDs and replace
resources; compare synthesis and the authorized deployment diff before accepting a migration. Examine IAM,
public access, encryption/TLS, DNS, retention, update/delete policies, custom resources, availability, and cost.
A removal policy is not proof that non-empty storage will be deleted or retained exactly as expected.

Keep reusable constructs separate from consumer accounts, regions, deployment identity, content, APIs,
monitoring, and budgets. Use examples and regression assertions for the supported composition. Product
requirements such as certificate region, bucket defaults, and OAC stay in the construct's local contract.

Synthesis is a local validation step; deployments, destruction, DNS changes, and cloud recovery require
separate authority. Record migration and rollback ownership before operations affecting existing data.
