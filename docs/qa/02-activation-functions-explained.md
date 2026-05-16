---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [activation-functions, sigmoid, relu, ai-concepts]
processed: false
---

# Why Sigmoid Can't Reach 0 or 1 — and Alternatives

## Question
Why can't sigmoid reach 1 and 0? Is there something that can? I heard there was a different way that wasn't forward pass and backpropagation.

## Answer

### Why Sigmoid is Asymptotic
`sigmoid(x) = 1 / (1 + e^(-x))` — to get 1, e^(-x) would need to equal 0, but e to any power never hits zero. Approaches forever.

- x = -10 → 0.0000454
- x = -100 → practically 0, never exactly

### Functions That CAN Hit 0 or 1

**Step function** — outputs exact 0/1 but breaks gradient-based training (flat everywhere, vertical at one point). Useless for backprop.

**ReLU** (`max(0, x)`) — used in modern networks. Negative → exactly 0. Positive → passes through. Maths works for training. Doesn't hit exact 1 either but stops mattering with layers.

### Other Training Methods

**Evolutionary algorithms** — create 100 neurons, test all, keep best, mutate survivors, repeat. No derivatives. Slower but can find solutions backprop gets stuck on.

**Reinforcement learning** — reward/punish instead of providing correct answer. How game-playing AIs are trained.
