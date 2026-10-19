# GuignaLabs Repository Workflow

This public-safe workflow applies to independent GuignaLabs repositories. In the
company workspace, explicitly read `../AGENTS.md` and
`../.workspace/company/workflow.md` when present. An isolated clone uses this
snapshot without the company checkout. Local instructions refine shared defaults;
explicit user instructions authorize task-specific exceptions.

## Frame Before Execution

Communicate with the owner in Spanish unless another language is requested.
Preserve the repository's existing language, terminology and conventions; keep
public company material in English. Do not invent customers, contact details,
domains or licenses. Inspect applicable instructions, Git status,
remotes and relevant documentation. Preserve unrelated and concurrent work.

Before nontrivial execution, record a bounded outcome, authorized scope, permitted
paths, acceptance criteria and planned validation using the task template. Scale
the record to the risk. Name a durable owner and separate concurrent write
boundaries; use separate worktrees when implementation streams need isolation.
Reuse relevant evidence only within its date, scope and limitations. Distinguish
requested, implemented, tested, published and customer-validated behavior.

## Implement, Validate & Review

Choose the smallest useful change and document material decisions. Follow the
repository's detected commands and tools; do not invent stacks, licenses, test
frameworks or coverage requirements. Run relevant checks, including meaningful
failure or boundary cases. Record real commands, results and evidence, and explain
skipped or unavailable checks. Preserve the original acceptance criteria; do not
weaken them to manufacture success.

After validation, perform a distinct review pass against the original outcome,
actual diff and evidence. Resolve blocking findings and record the review's kind
(same-agent, independent or human) accurately. A local check does not establish
that hosted CI ran or a deployment succeeded.

## Delivery & Handoff

Retain a concise receipt: delivered behavior and paths, acceptance evidence,
review, limitations, rollback or recovery, follow-ups and the next owner/action.
Identify pending shared integration. Closure, commit, publication and deployment
are separate states; never claim approval or integration that did not occur.
The coordinator owns shared company records; project records stay in their
repository unless the user requests otherwise.

When Git delivery is authorized, finish validated changes as scoped commits in
their owning repository and push to its verified remote. Record the commit,
branch, remote result and actual CI status in the receipt. A local-only repository
stops at a local commit. If access or checks block delivery, retain the exact
pending step; do not report the change as published or silently leave it untracked.

Before closure, record **Update**, **Add** or **None** in the existing knowledge
receipt; combine Update and Add when needed. Reuse an existing key before creating
one. Retain findings that change a future decision; None needs no extra explanation
or filler note. Link the canonical source/date, evidence state, limitations and
revalidation trigger. The receiving owner integrates shared navigation; mark it
pending until acknowledged. Preserve historical receipts and project ownership.
When the company checkout is available, search its canonical knowledge before
repeating research; an isolated clone follows its repository's existing knowledge.

## Git & External Authority

Use Gitflow by default when `develop` exists: start scoped work from `develop`,
squash completed work into `develop`, and use a normal merge from `develop` to
`main` for an authorized release. Respect repository-specific refinements. When
`develop` is absent, inspect existing conventions rather than inventing branches.
Prepare and validate locally; commits, pushes, Git initialization, remote creation
or changes, visibility changes, deployments, cloud/data mutations and messages to
others require corresponding explicit user authority. Run required repository
checks before an authorized
commit. Request explicit approval before **every `bq query`**, including read-only
queries and `--dry_run`.

## Simple Flow Diagrams

For requests to draw or explain a process, use a concise Mermaid flowchart with
short action labels and real decision branches. In the company checkout, read
`../.workspace/skills/draw-simple-flows/SKILL.md` from the target repository root
when available. This is explicit repository routing, not global skill installation.
An isolated clone can use the same diagram convention without the central skill.

## Configuration & Portable Snapshots

Use ordinary filenames for shared records: `.workspace/workflow.md` is the
portable workflow and `task.md` is a suitable task record. Reserve
`*.workspace.*`, for example `config.workspace.json`, for local configuration.
The repository's managed `.gitignore` block ignores this pattern without relying
on machine-wide Git settings. Keep that block last so later rules cannot override
it. Ignore rules do not remove already tracked files; inspect their history and
obtain the appropriate authority before changing their tracking or publishing.

Preserve global profiles and credentials. Never copy credentials, private company
or product records, or another repository's deployment configuration into a new
repository. Install only public-safe templates. The repository's portable
workflow, task template, instruction and ignore blocks are versioned snapshots;
bootstrap `--check` detects missing files and drift. Review and update snapshots,
the managed blocks and their metadata together manually; bootstrap refuses to
overwrite conflicting content. A copied snapshot needs no central checkout to be
read or followed.
