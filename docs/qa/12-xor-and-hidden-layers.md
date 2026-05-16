---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [xor, hidden-layers, neural-network, architecture]
processed: false
---

# XOR and Why One Neuron Isn't Enough

## Question
What is XOR and why does it need hidden layers?

## Answer

### XOR = Exclusive Or
"One or the other but not both." Like a light switch two people control — same position = off, different position = on.

| A | B | XOR Output |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

### Why a Single Neuron Can't Learn XOR
A single neuron draws one straight line through the data. There's no single straight line that separates XOR correctly. This was used in the 1960s to argue neural networks were useless — until hidden layers solved it.

### What Hidden Layers Add
- **Hidden neuron 1**: learns "are the inputs different?"
- **Hidden neuron 2**: learns "is either input on?"
- **Output neuron**: combines both → XOR

No single neuron could figure that out alone. Minimum layers for XOR: input → 1 hidden layer → output.

### What Tiny Networks Like This Can Do
Even a tiny 2-layer network can:
- Recognise handwritten digits (with enough neurons)
- Basic spam detection
- Sentiment analysis (positive/negative)
- Any pattern that isn't linearly separable
