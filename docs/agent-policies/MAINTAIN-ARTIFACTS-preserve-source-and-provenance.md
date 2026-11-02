---
id: MAINTAIN-ARTIFACTS
type: operational
scope: "Agent creation, editing and export of Landlord Mapper design artifacts."
status: adopted
authority: "Aslan — explicit approval of the exact migration set in the active chat, 2026-11-02."
revised: "2026-11-02"
depends_on: ["BOUND-DESIGN", "PROTECT-PRIVACY"]
related_to: ["VALIDATE-CHECKPOINTS"]
---
# Maintain artifact source and provenance
The hosted Penpot file linked from README is the editable source. `Wireframes.penpot` at the root is its native export, `exports/` holds PNG exports of its boards, and `design-tokens/` holds its token export, one file per palette. The project-owned `penpot-export.json` selects the native archive, file ID and token output paths for Agent Hands' reusable offline exporter; README documents preview and guarded execution. Refresh these together from the same state of the hosted file, and let Git history carry dates rather than dated file or folder names. Name semantic tokens by their role in the hierarchy, not by how they currently look.

State how each artifact was produced, such as derived from source code at a named commit or captured from the deployed site, and do not claim fidelity beyond that. Mark example data visibly as examples. Public artifacts must not contain real tenant, owner or other personal records unless the user confirms they are already public and appropriate to include.
