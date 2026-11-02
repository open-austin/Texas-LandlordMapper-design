---
id: PROTECT-PRIVACY
type: operational
scope: "Agent handling of files and public content in this repository."
status: adopted
authority: "Aslan — explicit approval of the exact migration set in the active chat, 2026-11-02."
revised: "2026-11-02"
depends_on: []
related_to: ["MAINTAIN-ARTIFACTS", "VALIDATE-CHECKPOINTS"]
---
# Protect private material in public content
This is a public repository. Never commit credentials, tokens, design-tool keys, private notes or personal machine paths. Keep local secrets in ignored files and run `git check-ignore -q <path>` before adding new files.
