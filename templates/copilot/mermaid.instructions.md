---
applyTo: "**/*.mmd,**/*.mermaid,**/*.md"
---
<!--
engineering/templates/copilot/mermaid.instructions.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Mermaid Diagram Instructions

Use diagrams when relationships are clearer visually. Install locally as `.github/instructions/mermaid.instructions.md`
with this front matter before the content: `applyTo: "**/*.mmd,**/*.mermaid,**/*.md"`.

1. Choose a diagram type and derive nodes/relationships from current repository evidence.
2. Keep editable source in a Markdown Mermaid fence or dedicated Mermaid source file.
3. Validate syntax and preview with available tooling; report a missing preview rather than inventing a tool.
4. Synchronize labels with maintained prose and preserve source alongside any rendered export.

Editor/extension integrations are optional. Use only available documented commands. Cloud synchronization,
sharing, paid AI repair, and external writes need task authority; diagram generation alone grants none.
Use descriptive labels and readable layout; omit private identifiers. Do not assume a particular editor.
