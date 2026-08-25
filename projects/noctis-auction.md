# Noctis Auctions — Auction Prototype and Predecessor to Infinity

## Summary

**Period:** February–March 2026  
**Summary:** An early full-stack beat-auction prototype that expanded into a broader cultural-platform concept and later informed the Infinity rebuild.

Noctis Auctions is a predecessor to Infinity, not exactly the same product under a different name.

## Problem

The starting question was whether beats could be presented as scarce creative work in a focused auction experience rather than as items in an unlimited catalog.

The concept combined premium presentation with timed bidding, creator identity, clear market states, payment, and post-purchase delivery.

## What I Tried

- Separate discovery and prestige auction contexts
- Auction cards, lot details, countdowns, and bid states
- Creator eligibility and application flows
- Payment, settlement, and deliverable concepts
- A later expansion into rap, dance, beats, visual culture, rankings, and competition areas

I developed the concept and product rules, made information-architecture and visual decisions, directed AI-generated implementation, reviewed screens and flows, found problems, and decided when iteration should become a rebuild.

## What Was Built

The private Next.js application includes:

- auction lists and lot-detail pages;
- authenticated account flows and server-side bid routes;
- auction closing and checkout states;
- Stripe Checkout and webhook foundations;
- post-purchase deliverable access;
- creator and seller application surfaces;
- administration and operations pages;
- database migrations and access-control rules;
- UI shells and design documents for broader platform areas.

The repository mixes implemented auction foundations, UI shells, and future system design. The presence of a route or specification does not mean every broader concept was complete or production-ready.

## AI / Tools

**Tools:** Next.js, React, TypeScript, Supabase, Stripe, Tailwind CSS, v0, Genspark

AI supported initial interface generation, visual variations, implementation, fixes, and frontend cleanup. I used those outputs to make product decisions, test behavior, and set priorities rather than treating the first generated version as final. I do not claim to have coded the application entirely by hand.

## What Changed

The product began with the transaction: discover a beat, place a valid bid, settle the result, pay, and receive the work. It then expanded into a much larger hip-hop cultural-network vision.

That expansion revealed long-term possibilities but weakened the MVP boundary. Instead of continuing to add layers, the next project began again as Infinity with a reconsidered architecture and product model.

## What I Learned

- A visually convincing prototype does not prove that the transaction or market works.
- With money and ownership, state, permissions, settlement, and delivery matter more than visual tension.
- A larger vision can reveal opportunities while hiding the smallest useful product.
- Generated code still requires mobile checks, build fixes, and decisions about real versus placeholder behavior.
- Starting over can be the right product decision when the current structure no longer matches the question.

## Status

Noctis Auctions remains a private historical prototype. It is included because it connects the early UI experiments to Infinity and shows how implementation exposed the need to rethink the product.
