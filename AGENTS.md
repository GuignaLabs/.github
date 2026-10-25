# Repository Guidelines

## Project Structure & Module Organization

This repository contains GuignaLabs organization-wide GitHub material. The public organization profile lives in `profile/README.md`. Keep the independent software lab identity, exact motto, Chile origin, and early-development status of the first sports platform. Keep application code and internal planning in their own repositories.

## Development & Validation Commands

There is no application runtime, dependency installation, build, or test suite here. Validate Markdown changes locally:

- `git status --short --branch`: inspect the active branch and pending files.
- `git diff`: review tracked content changes; read new files directly before staging.
- `git diff --check`: detect whitespace errors in tracked changes.
- `git diff --cached --check`: check the exact staged candidate before an authorized commit.

Check relative links against existing paths and preview the profile as Markdown before publishing.

## Coding Style & Naming Conventions

Write public content in English and communicate with the owner in Spanish. Use descriptive Markdown headings, short paragraphs, and hyphen bullets. Preserve the motto “Small by nature. Built for complexity.” Avoid unsupported claims about released products, customers, contacts, or licensing.

## Branch, Commit & Pull Request Guidelines

Use Gitflow: `main` represents published content, `develop` integrates upcoming changes, and `chore/<purpose>` branches contain maintenance work. Example: `chore/organization-profile`. Start maintenance branches from `develop`. Always squash `feature/*`, `chore/*`, and other working branches into `develop`, producing one commit per change. Integrate `develop` into `main` with a normal merge that preserves history; do not squash this promotion.

When explicitly authorized to commit, use concise messages such as `chore: add organization profile`. Pull requests into `develop` should explain the change, its purpose, and validation. Link an issue when available; include a preview when visual presentation changes. Promote reviewed content to `main` through a release.

## Agent Instructions

Preserve existing files and unrelated work. Do not commit, push, create remote branches, or change repository visibility without explicit owner authorization. Keep global Git and SSH configuration unchanged.

<!-- guignalabs:begin -->
## GuignaLabs Shared Instructions

Before work, find the nearest checkout ancestor containing both `AGENTS.md` and
`.workspace/company/workflow.md`, then explicitly read both. Grouped worktrees
have a deeper company root; do not assume it is the immediate parent or rely on
automatic instruction discovery across Git roots. When no company root exists
in an isolated clone, read the portable `.workspace/workflow.md` instead.
Repository-local instructions refine the shared defaults; explicit user
instructions authorize task-specific exceptions. Use
`.workspace/templates/task.md` for a bounded task record when appropriate.

Implement ordinary repository tasks in a dedicated worktree and branch from
fetched `origin/develop`, using
`.worktrees/<repository>/task-<id>-<purpose>/` under the company root. Record its
owner/task/base SHA. Declared stack layers may use their recorded predecessor
as base/target, keeping trunk `develop` and one worktree per layer. Task layers
ultimately land by squash on `develop`; release MRs promote
`develop` to `main` with a normal merge. Never push directly to either branch.
Read `.workspace/development.md` for the shared branch catalog, review-size bands,
stack dependencies and manual story closure. One issue can span many PRs; do not
require line estimates or fixed PR counts when creating it. Prefer 400 changed
lines, warn with a reason at 401–600, and split larger work. Follow the shared
workflow's MR readiness, current-candidate CI and review duties.
After confirming the MR is merged and dependents no longer need it, preserve
needed local files/data, remove only its owned worktree/local/remote task branch,
and verify/update the inventory; never delete `develop` or `main`. Keep task
resources while the MR is unmerged or cleanup
has a concrete preservation blocker; record owner and review date. The owner's
standing direction covers scoped local worktree/branch setup and post-merge task
cleanup. It does not authorize commits, publication, MR merge, unrelated deletion
or cloud actions.

Keep shared workflow and task records in ordinary Markdown filenames, such as
`.workspace/workflow.md` and `task.md`. Reserve `*.workspace.*` names, such as
`config.workspace.json`, for local configuration ignored by the repository's
managed `.gitignore` block. Never put secrets or private records in portable files.

The portable files are reviewed snapshots. If bootstrap `--check` reports drift,
review the differences and update the affected snapshot, managed blocks and
metadata together manually; bootstrap never overwrites a conflicting version.
<!-- guignalabs:end -->
