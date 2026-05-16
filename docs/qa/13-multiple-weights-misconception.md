---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [architecture, neural-network, hidden-layers, intuition]
processed: false
---

# Why Multiple Weights Per Neuron, Not One Input Spread Around

## Question
Why does it need multiple inputs instead of one input that gets spread to multiple neurons? Seems inefficient.

## Answer

### There IS Only One Input
```python
inputs = [0, 1]  # one list, passed once
```
It gets passed to the network once. Each hidden neuron reads from the same list but applies its own weights. Like handing one paper to two people — they each read it and form their own opinion.

### Why Multiple Hidden Neurons
One neuron draws one straight line. Two neurons draw two lines. Combined they can carve up the data in more complex shapes. XOR needs two lines — no single line separates it.

### Why Multiple Weights Per Neuron
Each hidden neuron needs its own relationship with each input. Hidden neuron 1 might care about Input A a lot and Input B barely. Hidden neuron 2 might be the opposite. They need independent weights to learn independently.

It's not one input spread around — it's the same input being interpreted differently by different neurons. That's where the power comes from.
