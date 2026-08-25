# Early Auction UI Experiments

## Summary

**Period:** February 2026  
**Summary:** Two related v0 and Genspark repositories used as one design experiment for a premium beat-auction interface before a real backend existed.

The original `v0-project` and `v0-project-ii` repositories are treated as iterations of the same question, not separate products.

## Problem

Before deciding on database, payment, or operational architecture, I needed something tangible enough to judge the visual language and information structure of a beat auction.

The questions included how to communicate scarcity, time, price, creator identity, and separate auction areas without making the interface feel like a generic marketplace.

## What I Tried

- Generated landing-page and auction layouts
- Auction cards, countdowns, and lot-detail concepts
- Dark visual styling and branding variations
- Pricing, hierarchy, and exclusivity copy
- Mobile adjustments and atmospheric effects

I defined the concept, directed the generated UI, reviewed variants, made hierarchy and branding decisions, found display problems, and selected ideas to continue into the next project.

## What Was Built

The experiments used Next.js, React, Tailwind CSS, and component libraries. They contained landing, auction, lot-detail, and account-related UI with mock bidding and purchase data.

There was no connected production database, real authentication system, or live payment backend. The two repositories share the same initial generated history; one is effectively an early snapshot and the other continued the UI revisions.

## AI / Tools

**Tools:** Next.js, React, Tailwind CSS, v0, Genspark

v0 and Genspark generated and revised substantial parts of the interface. My role was to define what should be explored, review the outputs, request changes, test the visual result, and decide what the prototype had and had not answered. I do not describe the UI as coded entirely by me.

## What Changed

The initial output established the page structure. Later iterations refined branding, hierarchy, auction-area presentation, pricing copy, effects, and build behavior.

The experiment eventually reached the limit of mock UI. Questions about valid bids, accounts, settlement, payment, and delivery required a real application model, leading to Noctis Auctions.

## What I Learned

- AI-generated UI can make an abstract idea testable very quickly.
- A polished screen can hide the absence of real data and behavior.
- Visual iteration helps decide how a product should feel, but cannot prove its core transaction.
- The next step should answer the most important unknown, not simply generate another screen.

## Status

These private historical experiments are the beginning of the sequence:

> **Early Auction UI Experiments → Noctis Auctions → Infinity**

No source code or original private-project assets are included in this portfolio.
