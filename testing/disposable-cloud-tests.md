<!--
engineering/testing/disposable-cloud-tests.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Disposable Cloud Tests

Use a separately authorized manual test when synthesis cannot establish deployed compatibility. Define an
exact resource allowlist, isolated account/environment, dedicated short-lived identity, unique resource
names, concurrency limits, cost bounds, cleanup procedure, and responsible operator before execution.

Require reviewed environment controls and scoped identity trust. Manual dispatch alone is not evidence of
approval. Inspect the generated resource set before creation and reject unexpected services or resources.
Do not use production data, content, domains, or credentials as disposable fixtures.

Arrange cleanup after both success and failure, then verify resources are gone. Cancellation and partial
failure can still leave resources; retain diagnostic evidence and a bounded operator recovery procedure.
A cleanup step's existence is not proof that cleanup completed. Record resource identities privately,
observed residual state, costs where available, and ownership of follow-up.

Keep the consuming project's concrete workflow, OIDC subject, environment names, service allowlist, and
recovery commands local. Its normal CI remains deployment-free.
