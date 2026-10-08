<!--
engineering/automation/validation-and-delivery.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Validation and Delivery

Keep ordinary validation separate from deployment, package publication, signing, and hosted
administration. Shared workflows validate a consumer; they do not assume its release identity or
control its infrastructure.

Choose caller events, cancellation, directories, commands, and required results for the actual
project. Verify caller behavior at an immutable revision. Copied starter files require independent
review when their contents change; updating a shared reference alone does not update copied
configuration.

Delivery uses the project's reviewed workflow, explicit identity, environment controls, candidate
artifact, and rollback procedure. Local/source validation does not establish deployed compatibility
or signed binary behavior. Record each outcome separately and keep credentials out of routine
fixture tests.
