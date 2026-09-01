# ZOS — Public Project Snapshot

> Curated snapshot from the private development repository. This page exposes the product structure and current implementation state without publishing the full private source repository.

## What it is

ZOS is a Life Game OS experiment for connecting direction, real-world action, replay, and self-observation.

The core loop is:

```text
Reality
→ Action
→ Execute in the real world
→ Short Replay
→ Character / Current State changes
→ Return to reality
```

Core concepts currently used in the implementation:

- **Vision** — current direction
- **Quest** — meaningful unit that moves toward a Vision
- **Action** — concrete real-world step
- **Replay** — short observation after an Action
- **Character** — current self-image discovered gradually through behavior and Replay
- **Current State** — where the user is now and what to do next

## Current MVP implementation

The current MVP is intentionally small and local-first.

Implemented:

- Japanese dark-theme onboarding
- Vision selection / free input
- first Quest input
- recurring Action input
- Action time / weekday settings
- notification preference value
- local persistence
- MVP home showing Vision / Quest / next Action / Character / Current State
- Action start / complete / interrupt / skip
- short Replay after completed or interrupted Actions
- Character observation state beginning after the first valid Replay
- reload recovery for active Action / Replay-pending state
- Save Data export / import
- compatibility with earlier Mirror / Persona Map experiments

Not yet fully implemented:

- actual notification delivery
- Character progression beyond the first observation state
- cloud sync / accounts
- production multi-user architecture

## Technical structure

The current MVP deliberately avoids unnecessary infrastructure:

- single `index.html`
- HTML / CSS / JavaScript
- no external JS libraries
- no build step
- PWA manifest
- localStorage-based state

Main local data domains include:

```text
onboarding
lifeGame
Action Runs
Replays
Character
Mirror entries
Open Questions
Persona Map
Import Backup
```

A full Save Data import is validated before write. If validation or write fails, partial state is not kept.

## Earlier product experiments retained inside ZOS

ZOS started as a self-observation tool. Earlier experiments such as Mirror and Persona Map are still retained as lower-level observation features rather than being treated as the main MVP loop.

Examples:

- **Mirror** — reaction, emotion, underlying desire, free notes
- **Persona Map** — roles / beliefs / relationships / anxieties / masks as nodes
- **Mirror ↔ Persona** links
- unresolved questions
- one-minute silence flow

These are not currently the first screen or core loop.

## What I do in the project

My main responsibility is not manually writing every line of code. I work on:

- problem framing
- product concept
- requirements and scope
- priority decisions
- UX / interaction decisions
- instructions to AI coding tools
- browser / device validation
- acceptance / rejection of AI-generated changes
- documenting the current state and contradictions

Claude Code / Codex are used for implementation and verification support, while final product decisions remain human-controlled.

## Live demo

Current public build:

https://zos.mugen8world.com

The public build may not always match the newest private development branch.

## Why the full repository is private

The development repository contains unfinished product experiments and internal working documents. This public snapshot is intended to show the actual product structure, implementation state, and working method without exposing the entire private workspace.
