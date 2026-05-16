---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [mixture-of-experts, architecture, model-orchestration, moe]
processed: false
---

# Mixture of Experts on Small Hardware

## Question
Can't I make a bunch of 100M parameter models specialised for certain things, orchestrated by a slightly larger model (like 2B)?

## Answer

### This is Real Research
**Mixture of Experts (MoE)** — a router model sends each problem to specialist sub-models. GPT-4 is rumoured to use this. Mixtral definitely does. The architecture intuition is sound.

### Where It Breaks Down
Reasoning isn't separable from knowledge — to reason about something you need to know things about it. When GPT-3.5 solves a logic puzzle, the reasoning is entangled with everything it knows about language, maths, and concepts.

Practical problems:
- 10 × 100M = 1B total, still needs to fit on 8GB
- The orchestrator itself needs capacity to route correctly
- Passing context between models is lossy and slow
- Most effort goes to plumbing, not intelligence

### Where MoE IS Good
- Making already-capable models more efficient ✓ (why big labs use it)
- Narrow deployable systems ✓
- Specific domain expertise ✓
- GPT-3.5 level from tiny models ✗

Big labs use MoE to make already-huge models efficient — not to make tiny models punch above their weight.
