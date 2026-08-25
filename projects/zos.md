# ZOS — From Self-Observation Tool to Life Game OS

## Summary

**Period:** May–August 2026  
**Summary:** A local-first self-observation tool that evolved through repeated prototypes into a Life Game OS connecting direction, real-world action, and reflection.

## Problem

The project began with a question: could private reflection help someone understand their reactions and unresolved questions? As prototypes accumulated, a deeper problem became clear—recording and analyzing the self did not necessarily help the user return to action.

The product was therefore reoriented around short interactions with real life rather than long sessions inside an app.

## What I Tried

1. **Mirror:** Record reactions, emotions, underlying wants, free-form notes, and unanswered questions.
2. **Persona Map:** Connect observations to visual nodes such as roles, beliefs, relationships, anxieties, and masks.
3. **Ritual concepts:** Return a previous observation at the same moment in a repeated activity.
4. **Life Game OS:** Organize the experience around Vision, Quest, Action, Replay, and Character.

My role was to define and repeatedly revise the problem, organize requirements and MVP boundaries, make UI/UX and language decisions, direct the AI tools, test the result in browsers and on real devices, identify problems, and decide what to keep or reject.

## What Was Built

The private repository's main branch contains a static HTML/CSS/JavaScript MVP with:

- Mirror, unanswered questions, and Persona Map;
- a Japanese onboarding flow for Vision, Quest, and Action;
- localStorage persistence and reload recovery;
- Action start, completion, interruption, and skip states;
- a short Replay flow;
- an initial Character change from unobserved to observing;
- combined Save Data export and import;
- validation, pre-import backup, and rollback for local data;
- PWA metadata.

It does not require a backend or build system. Later branches explored notifications, routines, action chains, voice input, conversational setup, an AI Game Master, and alternative map and navigation designs. Those are additional experiments, not one completed feature set.

## AI / Tools

**Tools:** HTML, CSS, JavaScript, localStorage, PWA, Claude, Claude Code, Codex

AI helped translate decisions into specifications and interface code, audit existing behavior, review storage and state transitions, find contradictions, and draft acceptance criteria. I was responsible for product direction, constraints, validation, priorities, and final decisions. I did not write the entire codebase by hand.

## What Changed

- “Store my thoughts” became “connect observation to real-world action.”
- Persona analysis moved away from the product center.
- A journal-like experience became an Action and Replay loop.
- Game language was kept, while rankings, meaningless points, guilt, and dependency patterns were rejected.
- AI was positioned as a tentative observer, not an authority that diagnoses the user.

## What I Learned

- Building prototypes helped redefine the problem; the correct product was not clear at the start.
- A small, testable loop was more valuable than a large collection of related features.
- AI can implement conflicting directions equally quickly, so product boundaries and written decisions matter.
- Local-first recovery and migration are part of the user experience, not only technical concerns.
- I became more interested in finding and structuring problems than in code production by itself.

## Status

The main branch contains the local-first MVP described above. Later branch work is presented only as additional experimentation. This case study does not claim a single final production version or describe deployment status.
