# Connector Boundary

## Purpose
This file defines safe boundaries for ChatGPT/GitHub connector use in this repository.

## Allowed by default
- Read repository metadata.
- Read files and pull request diffs.
- Create draft governance branches only after explicit approval.
- Open draft pull requests for review.

## Blocked without separate approval
- Merge or auto-merge.
- Force-update refs.
- Delete branches or files.
- Change secrets, environment variables, billing, or repository settings.
- Deploy, publish packages, or mutate external registries.
- Rerun workflows with side effects.

## Required evidence for connector actions
- Action timestamp.
- Actor/account.
- Repository and branch.
- Files changed.
- Commit SHA or PR URL.
- Rollback note.

## Current boundary
This repository is part of the Workspace OS GitHub root-hygiene pilot. All changes must remain reviewable and reversible.
