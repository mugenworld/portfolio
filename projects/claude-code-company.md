# Claude Company OS — AI-Native Operations Experiment

## Summary

**Period:** August 2026  
**Summary:** A repository-based experiment for coordinating one person's AI-assisted development, research, review, learning, and multiple projects through explicit authority and human approval.

## Problem

Using AI across several projects created recurring problems: decisions disappeared between sessions, agents interpreted projects differently, and the ability to perform an action could be confused with permission to perform it. More automation could increase speed without increasing reliability.

The project asked how AI work could be organized without giving up human judgment and accountability.

## What I Tried

- Human and AI responsibility boundaries
- Autonomy levels based on risk and reversibility
- Approval points for external or irreversible actions
- Decision records and project authority levels
- Reusable skills and bounded agent roles
- A learning flow that connects notes to adoption decisions
- Best-effort safeguards and regression tests
- A ZOS audit and E2E planning exercise without modifying the product

I defined the operating principles, authority model, approval boundaries, quality expectations, and adoption criteria. I directed Claude Code, inspected the results, and decided which forms of automation were appropriate.

## What Was Built

The private repository includes:

- a company charter, operating model, and quality criteria;
- autonomy levels, approval records, and Architecture Decision Records;
- a project registry with permitted AI authority;
- an Academy flow for distillation, adoption, and concrete follow-up;
- reusable Claude Code skills and planner/distiller roles;
- a best-effort hook intended to reduce common accidental branch operations;
- regression tests for that hook;
- a code-trace audit and E2E runbook for ZOS.

Later branch work explored a development-verification role and a small development board. These remain additional experiments.

## AI / Tools

**Tools:** Claude Code, Markdown, YAML, Python hooks, shell tests, custom skills and agents

Claude Code helped implement the repository, audit inconsistencies between policy and enforcement, create tests, and trace another project's code against acceptance scenarios. Because AI was both the tool and the subject of the experiment, its controls and reviews also required human verification. I do not present the repository as entirely hand-coded by me.

## What Changed

- The focus moved from an “AI organization chart” to bounded tasks and verifiable outputs.
- Full autonomy was replaced by deliberate human approval for higher-impact actions.
- Client-side safeguards were documented as accident-reduction measures, not security guarantees.
- Learning was required to produce an adoption decision or concrete change, not only a stored summary.

## What I Learned

- AI autonomy should be based on reversibility, external impact, and evidence—not perceived intelligence.
- More agents do not automatically create a better organization.
- Written policy is not the same as technical enforcement.
- AI-generated controls can fail or overreach and must be tested like product code.
- Human approval can be an intentional system component rather than an obstacle.

## Status

Claude Company OS is a private internal experiment. It demonstrates an approach to AI-native coordination and its limits; it is not a secure autonomous-company platform.
