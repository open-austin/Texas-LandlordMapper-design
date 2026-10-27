---
attention: live
---
# Penpot token export integration
Keep reusable extraction in Agent Hands under `use-penpot/scripts/export_tokens.py`, while this repository owns `penpot-export.json`. The manifest selects the existing native Wireframes archive, exact file identity, four palettes and six JSON destinations. It contains no credentials or executable commands.

## Scope and constraints
Use the observed native archive format rather than an unverified live API. The command validates source identity, token structure and references, previews output paths and hashes, and requires a matching preview digest before changed writes. It reproduces the browser export ordering of numeric palette keys, preserves other source token order and normalizes active-set membership to palette order, reproducing this snapshot's existing representation. No design values, native archive bytes or PNGs need to change to adopt it.

The source still needs to be refreshed from the intended Penpot file. Archive extraction does not fetch live state, prove freshness or regenerate board exports. README owns the maintained usage instructions; the manifest owns project-specific source/output selection. The Agent Hands export guide owns the reusable format and safety contract.

## Validation and publication
Verify the existing archive with a preview and no-change execution, then confirm hashes of all fourteen existing design artifacts remain unchanged. Run synthetic tests in Agent Hands and review selected changes before commits. Publish the reusable tool only after its prior outgoing history and exact workflow dependency are available, then publish this project integration and verify remote retrieval. Fresh-client MCP behavior and design human QA remain separate.
