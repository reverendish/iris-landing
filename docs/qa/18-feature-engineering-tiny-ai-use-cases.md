---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [feature-engineering, use-cases, tiny-ai, practical-ml]
processed: false
---

# Feature Engineering and Finding Use Cases for Tiny AI

## Question
What's the best way to pick relevant inputs for my use case? And what's a good way to find use cases for tiny AI?

## Answer

### Picking Relevant Inputs
Think like a human doing the job manually. What would you actually look at? Write that list. Those are your inputs.

For Iris: does the title match, does salary fit, is location right, how many skills match, is seniority right, company size preference. Six inputs. Strong start. Refine with real data.

**General rule:** if a smart human would look at it → relevant. If they'd ignore it → leave it out.

### Finding Use Cases for Tiny AI
The best use cases share a pattern:
- The decision is **repetitive** — same judgment made over and over
- The inputs are **structured** — measurable as numbers
- The output is **narrow** — one decision, one score, one classification
- A human **could do it** but it's boring or slow

### Where to Look
- Anything where someone uses a spreadsheet to score/rank things
- Any inbox getting the same type of message repeatedly
- Any decision with clear criteria but slow to apply manually
- Anywhere people say "I have to go through hundreds of these"

**Examples:** scoring job candidates, flagging wrong invoices, routing support tickets, deciding which leads to call first.

**The pattern is always:** boring repetitive judgment → perfect for a small classifier.
