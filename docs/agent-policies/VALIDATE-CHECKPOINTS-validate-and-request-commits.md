---
id: VALIDATE-CHECKPOINTS
type: operational
scope: "Agent validation, local commits and publication boundaries in this repository."
status: adopted
authority: "Aslan — explicit approval of the exact migration set in the active chat, 2026-11-02."
revised: "2026-11-02"
depends_on: ["PROTECT-PRIVACY"]
related_to: ["MAINTAIN-ARTIFACTS"]
---
# Validate changes and request commit approval
Validate token exports with the Agent Hands preview command documented in README; this repository has no application build or automated test suite. A commit policy has not been set: ask before committing, commit by explicit pathspec, never use `git add -f`, and never add a `Co-Authored-By:` trailer. Agents never push; publishing and other remote actions follow the user's authorization.
