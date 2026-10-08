<!--
engineering/releases/evidence-and-history.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Release Evidence and History

Keep changelogs, archive indexes, and version records with the released component. Changelogs own
concise version highlights; records own candidate scope, compatibility, validation, artifacts,
limitations, and recovery.

Distinguish prepared candidate, existing local tag, hosted validation, published release, and
consumer rollout. Record event date/timezone separately from preparation or publication dates.
Evidence belongs to its exact commit, tag, artifact, configuration, and environment;
current-checkout success does not validate an old tag.

Preserve historical outcomes, including failed, skipped, and pending checks. Add a dated
clarification when needed rather than implying later verification was available at preparation time.
Keep immutable tags intact; repair through a reviewed correction or new release. Link to artifact
integrity and identity evidence without putting sensitive operational details in public records.

Use platform-specific [Python](python-packages.md), [Apple](apple-apps.md), and [shared
automation](shared-automation.md) guidance. Merging documentation is not proof of publication.
