<!--
engineering/SECURITY.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Private reporting guidance and consumer security responsibilities.

Responsibilities
- Maintain security policy for this repository.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Security Policy

- [Reporting a Vulnerability](#reporting-a-vulnerability)
- [What to Include](#what-to-include)
- [Security Model](#security-model)
- [Consumer Responsibilities](#consumer-responsibilities)
- [Maintenance and Disclosure](#maintenance-and-disclosure)

## Reporting a Vulnerability

Coordinate sensitive findings privately with repository maintainers. Use GitHub private
vulnerability reporting if available; otherwise ask a maintainer for a private channel without
disclosing exploit details. This policy does not establish that a hosted feature is enabled or that
a particular email address is monitored. Do not disclose credentials or private evidence in public
issues or pull requests.

## What to Include

Provide the affected revision, document or template, impact, minimal sanitized reproduction, and
known mitigation. Identify whether the problem is in shared guidance or a consuming implementation.
Share sensitive supporting evidence only through the agreed private channel.

## Security Model

Documentation and templates require review before adoption. Local hooks can execute downloaded tools
and rewrite files; review the [hook configuration] and [contributor guide] before use. A passing
Markdown or credential-pattern check is not a security certification. The [workflow trust guidance]
covers separate execution and permission boundaries.

## Consumer Responsibilities

Consumers own execution environments, credentials, dependencies, deployment, and hosted settings.
Verify copied commands and instructions against local contracts. Keep completed operational records
and confidential incident evidence outside this public-facing documentation checkout.

## Maintenance and Disclosure

Coordinate remediation and disclosure with maintainers and affected consumer owners. Record
revision-specific evidence and distinguish local verification from deployed behavior. No response
deadline or security-support window is promised here; see the [support guide].

[hook configuration]: .pre-commit-config.yaml
[contributor guide]: CONTRIBUTING.md
[support guide]: SUPPORT.md
[workflow trust guidance]: security/workflow-trust-boundaries.md
