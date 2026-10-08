<!--
engineering/testing/infrastructure.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Infrastructure Testing

Start with deterministic synthesis and property validation. Assert meaningful resource properties,
trust boundaries, lifecycle policies, and invalid inputs. Guard logical identities when intentional
tests protect stateful resources. Examples should demonstrate supported compositions and participate
in validation.

Review replacement, IAM, public access, TLS/DNS, retention, custom resources, availability, and cost
before an infrastructure change is accepted. Synthesis establishes generated configuration, not
deployed behavior, permissions, drift, service availability, or cleanup success.

Keep normal CI free of deployment credentials. Optional security, package-installation, and
cloud-deployment suites remain explicit when their dependencies or side effects differ. Use
[disposable cloud tests](disposable-cloud-tests.md) for an authorized bounded operational check;
consumer account, identity, domains, monitoring, and rollback remain consumer-owned.
