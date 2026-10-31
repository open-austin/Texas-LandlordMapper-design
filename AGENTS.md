# Agent Instructions
This repository holds design files for Landlord Mapper, an Open Austin project. It contains no application code: the data pipeline lives in [open-austin/landlord-mapper](https://github.com/open-austin/landlord-mapper) and the web frontend in [open-austin/landlord-mapper-frontend](https://github.com/open-austin/landlord-mapper-frontend). Work here does not change those repositories unless the user asks for that separately.

## Workflow source
This project adopts `project-workflows/` as a Git submodule. Read [workflow.toml](project-workflows/workflow.toml) for configured document locations, then use its `<skill-name>/SKILL.md` procedures. The project-specific copy is authoritative over global seeds, and these instructions override seed defaults. General skills and external-service tooling are optional unless explicitly adopted.

The submodule's project branch is `project/texas-landlordmapper-design`, separate from this repository's `main`. The parent Git pin records the exact adopted revision; `.gitmodules` names the project branch, but that does not make its local commits available remotely. Use [setup-project-workflows](project-workflows/setup-project-workflows/SKILL.md) for adoption and docs setup and [update-project-workflows](project-workflows/update-project-workflows/SKILL.md) for shared improvements, project reconciliation, branch metadata and consumer pins. Publication scope and remote availability are verified separately.

Use [Coordinate Project Contribution](project-workflows/coordinate-project-contribution/SKILL.md) to start contribution and review work under this project’s existing human direction. Each agent keeps its own spike; a branch may carry several spikes/issues and later reviews. Existing privacy, validation and publication rules remain authoritative.

## Documentation
README explains the project and how to start. TODO indexes active work. Current policies in `docs/policies/` define standing guidance; spike pairs in `docs/active-spikes/` hold scoped reasoning and work state; `docs/scratch/` is provisional; `docs/archive/` preserves history. Actual project documents live in this repository, outside the workflow submodule.

The hosted Penpot file linked from README is the editable source. `Wireframes.penpot` at the root is its native export, `exports/` holds PNG exports of its boards, and `design-tokens/` holds its token export, one file per palette. The project-owned `penpot-export.json` selects the native archive, file ID and token output paths for Agent Hands' reusable offline exporter; README documents preview and guarded execution. Refresh these together from the same state of the hosted file, and let Git history carry dates rather than dated file or folder names. Name semantic tokens by their role in the hierarchy, not by how they currently look.

## Design artifacts
State how each artifact was produced, such as derived from source code at a named commit or captured from the deployed site, and do not claim fidelity beyond that. Mark example data visibly as examples. Public artifacts must not contain real tenant, owner or other personal records unless the user confirms they are already public and appropriate to include.

## Privacy
This is a public repository. Never commit credentials, tokens, design-tool keys, private notes or personal machine paths. Keep local secrets in ignored files and run `git check-ignore -q <path>` before adding new files.

## Validation and Git
Validate token exports with the Agent Hands preview command documented in README; this repository has no application build or automated test suite. A commit policy has not been set: ask before committing, commit by explicit pathspec, never use `git add -f`, and never add a `Co-Authored-By:` trailer. Agents never push; publishing and other remote actions follow the user's authorization.

## Markdown style
Keep each prose paragraph or comment paragraph on one line and let editors wrap it. Avoid reflow-only edits. Preserve meaningful line breaks, existing local conventions, and explicit formatter requirements.

The recorded workflow pin is published and anonymous recursive retrieval has been verified. All eight procedures live at the collection root. Use capture-for-later for new small subject notes; preserve existing notes and deferred work without bulk migration. The [adoption record](docs/active-spikes/project-workflows-adoption.md) records the content review, publication evidence and remaining client checks.
