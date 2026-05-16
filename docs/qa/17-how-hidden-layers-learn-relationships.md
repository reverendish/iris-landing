---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [backpropagation, hidden-layers, learning, neural-network]
processed: false
---

# How Hidden Layers Learn Relationships

## Question
How do hidden layers learn the relationships between inputs?

## Answer

### The Backpropagation Mechanism
Remember the adjustment formula from the single neuron:
```
weight += error × input × learning_rate
```

In a network, this happens *backwards* through every layer. The output neuron gets the error first. Then it passes blame back to hidden neurons — each is told "you contributed this much to the mistake." They adjust accordingly.

### What Emerges Over Thousands of Rounds
Nobody programs specific roles for hidden neurons. They *emerge* from the error signal:

- Hidden neuron 1 gets rewarded when it notices A and B are different
- Hidden neuron 2 gets rewarded when it notices either input is on
- The output neuron learns to combine those signals correctly

This is why it's called **backpropagation** — the error propagates backwards through layers.

### Why Deep Networks Are Powerful
More layers = increasingly abstract relationships:
- Early layers: simple patterns (edges in image, salary is high)
- Middle layers: combine into shapes (role matches + salary fits)
- Later layers: combine into concepts (promising overall = apply)

For Iris:
```
Layer 1: salary is high, role matches
Layer 2: when both true → promising
Layer 3: promising + location match → apply
```

Nobody tells it that. It figures it out from thousands of examples.
