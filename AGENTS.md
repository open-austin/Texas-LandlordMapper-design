# Agent Instructions
This repository holds design files for Landlord Mapper, an Open Austin project. It contains no application code: the data pipeline lives in [open-austin/landlord-mapper](https://github.com/open-austin/landlord-mapper) and the web frontend in [open-austin/landlord-mapper-frontend](https://github.com/open-austin/landlord-mapper-frontend). Read [BOUND-DESIGN](docs/agent-policies/BOUND-DESIGN-keep-work-within-design.md) for the agent scope boundary.

## Workflow source
This project adopts `project-workflows/` as a Git submodule. Read [workflow.toml](docs/workflow.toml) for configured document locations, then use its `<skill-name>/SKILL.md` procedures. The pinned shared procedures take precedence over global seeds, and these instructions override seed defaults. General skills and external-service tooling are optional unless explicitly adopted.

The submodule uses an exact detached shared-source pin. Project configuration, adopted policies and local procedures remain outside the package; `.gitmodules` tracks shared main while the gitlink records the accepted revision. Use [setup-project-workflows](project-workflows/setup-project-workflows/SKILL.md) for adoption and docs setup and [update-project-workflows](project-workflows/update-project-workflows/SKILL.md) for shared improvements, project reconciliation, branch metadata and consumer pins. Publication scope and remote availability are verified separately.

Use [Coordinate Project Contribution](project-workflows/coordinate-project-contribution/SKILL.md) to start contribution and review work under this project’s existing human direction. Each agent keeps its own spike; a branch may carry several spikes/issues and later reviews. Existing privacy, validation and publication rules remain authoritative.

## Agent policy routing
Read the project-owned [agent policy index](docs/agent-policies/policy.index.md), select the applicable adopted obligations and load their complete prerequisite closure once, prerequisites before dependents. The adopted kernel governs policy decisions, identity and dependency loading; bundled candidates remain proposed. Use the selected collection's [Create](project-workflows/create-agent-policy/SKILL.md), [Edit](project-workflows/edit-agent-policy/SKILL.md), [Review](project-workflows/review-agent-policies/SKILL.md), [Adopt](project-workflows/adopt-agent-policies/SKILL.md) and [Retire](project-workflows/retire-agent-policy/SKILL.md) procedures for policy work. Package updates supply candidates without adopting or replacing these project-owned policies.

## Documentation
README explains the project and how to start. TODO indexes active work. The [agent policy index](docs/agent-policies/policy.index.md) records policy scope and status; spike pairs in `docs/active-spikes/` hold scoped reasoning and work state; `docs/scratch/` is provisional; `docs/archive/` preserves history. Actual project documents live in this repository, outside the workflow submodule.

Read [MAINTAIN-ARTIFACTS](docs/agent-policies/MAINTAIN-ARTIFACTS-preserve-source-and-provenance.md) for hosted-file, export and token-naming obligations. README owns the export procedure, and `penpot-export.json` owns its project-specific selection.

## Design artifacts
Read [MAINTAIN-ARTIFACTS](docs/agent-policies/MAINTAIN-ARTIFACTS-preserve-source-and-provenance.md) for artifact provenance, example-data labeling and public-record boundaries.

## Privacy
Read [PROTECT-PRIVACY](docs/agent-policies/PROTECT-PRIVACY-keep-public-content-safe.md) before handling files or public content.

## Validation and Git
Read [VALIDATE-CHECKPOINTS](docs/agent-policies/VALIDATE-CHECKPOINTS-validate-and-request-commits.md) for validation, commit approval and publication boundaries. Agents must still ask before committing, including updater-created child merge commits.

## Markdown style
Read [PRESERVE-PROSE](docs/agent-policies/PRESERVE-PROSE-retain-wording-and-note-scope.md) for prose edits, small subject notes and preservation of existing notes.

The procedures live at the collection root. The parent gitlink records the exact adopted workflow revision. The [adoption record](docs/active-spikes/project-workflows-adoption.md) and [policy migration archive](docs/archive/agent-policy-migration.md) preserve prior verification and migration history. Current policy definitions and status belong to the [agent policy index](docs/agent-policies/policy.index.md); remaining fresh-client checks are tracked in TODO.
