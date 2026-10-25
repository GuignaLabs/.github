# Repository Workflow

Framework version: 0.3.0. Generated from the current method and reviewed project policy. This document does not install the tools: use the coordination root containing scripts, and report unavailable checks accurately.

## GuignaLabs Policy

Apply the current framework together with these company choices. Explicit owner
requests and host constraints govern task-specific authority. Product domain,
runtime and budget choices stay in their owning repositories.

### Communication And Ownership

Communicate with the owner in Spanish. Preserve repository code/documentation
language; public brand material stays in English. Do not invent customers,
contacts, domains, licenses, delivered capabilities or approval. The company root
stays outside Git; repositories own independent histories and remotes. The central
`.workspace` is local-only coordination. Read root/project/nested AGENTS rules.
Find the company root among checkout ancestors using root AGENTS.md and
`.workspace/company/workflow.md`; an isolated clone uses its portable snapshot.

### Git, Worktrees And External Authority

When develop exists, start scoped branches there, squash completed work into
develop and merge develop normally into main for an authorized release. Otherwise
inspect the repository's existing strategy. New product/organization worktrees
use `.worktrees/<repository>/task-<id>-<purpose>/` under the company root. Register
them centrally; permanent editor entries are optional. Existing sibling role
checkouts remain for separately scoped migration/retirement. Follow the core's
post-integration retirement or reason/owner/review-date retention rule.

Commits, pushes, Git initialization, branch/worktree creation/move/removal,
remote/visibility changes, deployment, cloud/data mutation and external messages
require corresponding explicit authority.
Request approval before every `bq query`, including read-only and dry-run.
Preserve global profiles, credentials,
required local files and runtime data. No task workflow grants spending authority.

### Local Records And Tools

The receiving coordinator owns shared navigation/knowledge and actual handoff
acknowledgements. Keep private product research/evidence in its owning location;
do not copy it into portable repositories. Use ordinary shared filenames and
reserve `*.workspace.*` for ignored local configuration. Adopt generated snapshots
and their metadata together, preserving project-owned AGENTS content.

Company checks are scripts/check_workflow.py and scripts/check_workspace.py;
schema1 release checks remain required for substantive changes. Git-candidate,
knowledge-retrieval, native-agent and product-runtime tools are optional adapters
used for relevant work. A local source check is not hosted CI or agent compliance.
For process diagrams, use the existing draw-simple-flows skill when available
under the company root; no global skill installation is implied.

## Working Method

Every substantive task has a bounded outcome: working behavior, a supported
answer, a decision or an enabling capability. Scale the work record and checks
to risk while preserving acceptance and authority. Project/company policy
supplies local choices; owner requests and host constraints govern execution.

## Frame And Retrieve

Inspect applicable instructions, Git state/remotes and relevant documentation.
Search existing project knowledge before repeating research; read the canonical
source with its date, scope and limits. Historical observations do not establish
current validity. Preserve unrelated/concurrent work and private configuration.

Use one task record with a stable ID and responsible owner. Before execution,
record beneficiary, purpose, actual authority, included/excluded paths, original
acceptance criteria, validation plan, approach and recovery. Name receiving
owners and dependencies. Keep at most three current actionable steps. A routine
task can use one criterion; retain a single canonical state instead of duplicate
hand-maintained result tables. Use the schema-1 task template routed by the local
entrypoint; fill examples with actual values before validation.

## Implement And Validate

Choose the smallest useful change. Follow detected repository commands and
conventions; do not invent stacks, licenses, numeric coverage or capabilities.
Define observable expectations before implementing. Test relevant successful,
failure, boundary and regression cases proportionally. Preserve original
criteria; explain material decisions and skipped/unavailable checks.

Bind a passing observation to the actual contract, delivered file hashes, UTC
time, environment and nonempty evidence. A hash does not prove semantic truth or
actual execution. Changing scope/criteria requires a new task revision with the
old contract, reason and authority retained. Changed artifacts invalidate affected
proofs. Revalidate; do not refresh approvals by replacing hashes alone.

Perform a distinct review against the original outcome, actual diff and evidence.
Record reviewer/kind and resolve blocking findings. Same-agent review is not
independent review. High-impact releases require the configured owner acceptance
and independent/human review. Local tests do not establish hosted CI or deployment.

## Integrate And Manage Worktrees

Use an independent checkout when parallel implementation or revision-specific
testing needs isolation. Follow the workspace's worktree location and branch
strategy. Assign one task/write owner per checkout; record repository, path,
branch and resolved base. Keep one index writer; shared refs and runtime resources
still need coordination. New worktrees do not inherit uncommitted source or ignored
configuration automatically. Set up explicit, separate runtime selectors as needed.

Verify the actual integration result against the current target, including merged
dependencies and conflicts. Earlier task acceptance does not validate a new merge
result. For squash integration retain the target commit/PR binding; branch
reachability alone does not prove the task's changes landed.

Before an authorized commit, validate the exact staged scope against its intended
resolved base using the applicable candidate checker. Bind scope/policy/candidate
digests, recheck immediately before committing and verify the actual commit.
Working-tree tests cannot prove the index contains required files. Missing
dependencies remain a delivery gap; never import another owner's bytes or waive
checks to force a pass. Check-to-commit is not atomic.

After integration resolve worktree, local-branch and remote-branch disposition
separately. Preserve needed tracked, untracked and ignored files, credentials and
runtime data before authorized retirement. Retire the temporary checkout using
Git, or record retention reason, responsible owner and review date. Update
inventory/editor entries after actual removal. Missing authority or unsafe cleanup
stays explicitly pending. Age, merge and task closure never authorize deletion.

## Deliver, Accept And Retain

Retain delivered behavior/paths, purpose, acceptance evidence, review, limitations,
recovery, useful knowledge, follow-ups and next owner/action. Distinguish local
completion, integration, commit, push, publication, deployment and customer
validation. Perform external actions only within corresponding actual authority.
Do not silently leave a contracted delivery unfinished; record its exact blocker
and pending step. Do not treat a prior owner's approval as authority for new work.

Use READY from the release gate and the required semantic/owner acceptance before
closing. Schema 1 fingerprints contract and artifacts; review also binds current
check/receipt digests, and owner acceptance binds review. Automatic acceptance is
derived only from an authorized policy. Tool readiness verifies recorded structure
and integrity; it cannot authenticate actors or prove claims, execution or cleanup.

Before closure record Update, Add or None for reusable knowledge. Reuse existing
keys. Retain findings that change a future decision with canonical source/date,
evidence state, scope/limits and revalidation trigger. None needs no filler record.
The receiving owner alone integrates shared navigation and acknowledges actual
handoff; keep it pending until observed. Preserve historical receipts and original
task ownership. A task may be closed locally while separately scoped integration
or publication remains pending, with explicit receiver/action.

## Maintain Instructions

Current rules live in this versioned core and the applicable project policy.
Record superseded rules and migration in CHANGELOG.md; keep outdated proposals
and dated evidence outside mandatory reading. Version tools, templates and
instructions together. Update only reviewed adopted copies and their metadata;
preserve local instructions and detect drift. Never infer installation, global
settings, permissions or agent compliance from the existence of a document.
