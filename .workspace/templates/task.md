# Task — <bounded outcome>

Save shared records with ordinary names such as `task.md`. The `*.workspace.*`
pattern is reserved for ignored local configuration, not shared task evidence.

## Contract Before Execution

- Owner and receiving coordinator: <durable ownership and handoff>
- Purpose and observable outcome: <smallest useful result>
- Authority: <user request and any explicit external authorization>
- Scope and permitted paths: <included changes and concurrent write boundaries>
- Acceptance criteria: <observable scenarios, expected results and invariants>
- Validation plan: <methods, relevant failure cases and expected evidence>
- Approach and rollback: <minimal implementation, dependencies and recovery>

## Execution & Evidence

Record material decisions, changed paths and actual validation commands/results.
Identify skipped checks and their reasons. Preserve unrelated work and the original
acceptance criteria; distinguish assumptions from observed behavior.

## Distinct Review Pass

Record review kind, outcome against the contract, actual diff and evidence,
findings and their disposition. Do not represent same-agent review as independent.

## Receipt & Handoff

Record delivered behavior, acceptance, limitations, rollback, retained knowledge,
follow-ups, receiving owner and next action. Distinguish local completion from
commit, integration, publication and deployment; retain pending dispositions.
For authorized Git delivery, record the owning repository, commit/branch, push
result and actual CI status. Local-only repositories need a local commit; blocked
publication stays pending with its concrete next step.

For retained knowledge, state **Update**, **Add** or **None** in that receipt.
Prefer existing keys; retained claims need a canonical source/date, evidence state,
limits and revalidation trigger. None needs no extra explanation or new note.
Name the receiving owner and whether shared integration is pending or acknowledged.
Keep project evidence local to its repository; do not copy private records into
portable guidance or change historical receipts.
