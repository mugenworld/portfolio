# Claude Company OS — Public Project Snapshot

> Curated snapshot from the private Company repository. The full repository remains private because it is designed to eventually hold client / contract / operational information.

## What it is

Claude Company OS is an AI-native company operating experiment for a Founder working with AI agents across product work, research, learning, and eventually external client work.

The repository does **not** contain the product source code itself. It contains the operating rules, decision criteria, project registry, approval rules, learned knowledge, and reusable workflows that coordinate work across repositories.

## Actual repository structure

The private repository currently uses a structure like this:

```text
.claude/
  agents/
  hooks/
  skills/
  settings.json

academy/
company/
ops/
projects/

CLAUDE.md
README.md
```

Main responsibilities:

| Area | Purpose |
|---|---|
| `CLAUDE.md` | rules Claude reads every session |
| `company/` | purpose, principles, authority boundaries, quality criteria, ADR decisions |
| `projects/` | registry / control state for repositories the Company works on |
| `academy/` | raw learning → distilled notes → adoption decisions → reusable practice |
| `ops/` | approvals and operational controls |
| `.claude/skills/` | reusable procedures |
| `.claude/agents/` | isolated roles for work that benefits from separate context |
| `.claude/hooks/` | best-effort accident-reduction rules for risky local operations |

## How the AI organization currently works

```text
Founder (human)
   │
   └── Chief / Orchestrator (main Claude Code session)
          ├── Planner — read-only investigation / planning
          └── Review workflow — independent quality review
```

The current design deliberately does **not** create an agent for every role.

A new sub-agent is added only when the work benefits from context isolation, can run independently, does not require continuous Founder dialogue, and can return a defined artifact.

Implementation currently stays in the main working session because active build work benefits from continuous context and human feedback.

## Human approval boundary

The core rule is simple:

> Internal, reversible, non-public work can be more autonomous. External, irreversible, high-risk work must return to the Founder.

The Company currently distinguishes four practical autonomy levels:

1. **Fully automatic** — internal research, summaries, planning, learning distillation
2. **Automatic + result review** — branch implementation, tests, PR preparation, internal reports
3. **Founder approval before execution** — external commitments, payments, production/public changes, scope / deadline commitments
4. **Not automated** — direct main merge or unattended external action loops

The local hook / deny configuration is treated as an **accident-reduction layer**, not a security guarantee. The final control remains Founder review and explicit approval.

## Example working loop

For a normal development request, the intended flow is:

```text
Founder gives objective
→ Company inspects the current repository / docs
→ plan is created
→ implementation happens on a feature branch
→ tests / checks run
→ a separate review step evaluates the result
→ Founder receives a decision-ready report
→ Founder decides whether it should be merged / released
→ useful lessons are recorded for reuse
```

For future external client work, the same engine can be reused behind a separate client-delivery entry flow:

```text
Opportunity
→ Bid / no-bid decision
→ proposal
→ clarify what 'done' means
→ build
→ verify
→ Founder review
→ delivery
→ retrospective / learning
```

## What has been tested so far

The Company has already been used as an operating layer for private product work rather than remaining only a theoretical folder structure.

Examples of what has been exercised:

- project registration and state tracking
- planning / implementation separation
- branch-based implementation
- review and verification loops
- explicit Founder approval boundaries
- best-effort prevention of direct `main` writes through Claude Code
- documenting known limitations rather than claiming stronger guarantees than actually exist
- using product work to reveal what the Company OS is missing

## What I do in the project

My responsibility is the Founder / manager layer:

- define the objective
- decide what AI may and may not decide
- set quality / safety boundaries
- review important outputs
- approve or reject changes
- decide whether an operational rule should become reusable Company knowledge

Claude Code handles much of the reading, planning, implementation, testing, comparison, and documentation work inside those boundaries.

## Why the full repository is private

The real Company repository contains internal operating material and is intended to support future client work. Publishing the entire repository would work against the privacy and separation rules the system itself is designed to enforce.

This snapshot exposes the architecture and actual operating model while keeping private operational material private.
