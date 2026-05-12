# AGENTS.md

## Workspace OS agent instructions

Purpose: provide safe, explicit guidance for AI-assisted work in this repository.

### Default operating mode
- Read before write.
- Prefer draft branches and draft pull requests.
- Do not merge without explicit human approval.
- Do not deploy, publish packages, rotate secrets, or change billing/settings from an agent run.
- Keep evidence in the pull request body and linked artifacts.

### Approved branch pattern
- `workspace/*` for Workspace OS governance and hygiene work.
- `repair/*` for bounded repairs.
- `audit/*` for evidence-only audits.

### Required PR evidence
Each agent-created PR should include:
1. Intent and scope.
2. Files changed.
3. Risks and rollback notes.
4. Tests or inspection performed.
5. Human approval needed before merge.

### Protected boundaries
Blocked unless separately approved:
- Merge or auto-merge.
- Force-push or destructive ref updates.
- Secrets, tokens, credentials, or environment changes.
- GitHub Actions reruns that mutate state.
- Public release, deployment, or package publishing.
