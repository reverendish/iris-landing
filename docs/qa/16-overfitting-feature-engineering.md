---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [overfitting, feature-engineering, data-quality]
processed: false
---

# More Inputs ≠ Better Output (Overfitting)

## Question
So more inputs means better output? That's why people add more?

## Answer

### The Trap
More inputs means more information — but not automatically better output. This trips people up constantly.

### How More Inputs Can Hurt
If you add irrelevant/noise inputs, the network wastes capacity trying to figure out they don't matter. Worse — it might find **fake patterns** in them.

Example: adding "favourite colour" as an input to Iris. Due to random noise in training data, the network might learn "people who like blue get jobs." That's **overfitting** — memorising the training data's accidents.

### The Real Answer
```
More relevant inputs → better output
More irrelevant inputs → WORSE output
```

The skill is knowing the difference. Feature engineering (choosing what to measure) matters as much as the architecture.

### How to Pick Good Inputs
Think like a human doing the job manually. If a smart human would look at it — it's probably relevant. If a smart human would ignore it — leave it out.

For Iris:
1. Does the job title match? ✓
2. Does the salary fit their range? ✓
3. Is location/remote policy acceptable? ✓
4. How many required skills do they have? ✓
5. Is seniority level right? ✓
6. Is company size they'd enjoy? ✓

Refine with real data — maybe company size doesn't matter, maybe tech stack overlap matters more than you thought.
