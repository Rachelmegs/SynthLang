# Repository Governance

## Status
Workspace OS root-hygiene draft. This file defines operating expectations for AI-assisted and human changes.

## Ownership and approval
- Repository owner: Rachelmegs.
- AI-assisted changes must be proposed through branches and pull requests unless a separate approval explicitly allows direct commits.
- Merge approval remains human-only.

## Change classes
| Class | Examples | Default handling |
|---|---|---|
| Read-only audit | inventory, evidence capture, documentation review | allowed with evidence log |
| Documentation hygiene | AGENTS.md, governance docs, repo passports | draft PR required |
| Code change | source, tests, build config | draft PR plus review required |
| Release/deploy | package publishing, deployment, external registry changes | blocked until separately approved |
| Sensitive operation | secrets, tokens, billing, repo settings | blocked until separately approved |

## Evidence requirements
Every governance PR should include:
- Scope summary.
- Files changed.
- Validation performed.
- Known limits.
- Rollback plan.

## Merge boundary
No agent-created PR may be merged automatically. Human approval is required before merge.
