---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [neural-network, tutorial, python, ai-basics]
processed: false
---

# Building a Single Neuron from Scratch

## Question
I need help learning to write and train a single neuron.

## Answer / Full Tutorial

A neuron takes numbers in, does math, spits one number out. Training = slowly adjusting weights until correct.

### Forward Pass
```
output = (input1 × weight1) + (input2 × weight2) + bias
```
Weights = how much the neuron cares about each input. Bias = baseline nudge.

### The Code
```python
import random, math

data = [([0,0],0), ([1,0],0), ([0,1],0), ([1,1],1)]  # AND logic

w1 = random.uniform(-1, 1)
w2 = random.uniform(-1, 1)
bias = random.uniform(-1, 1)

def sigmoid(x): return 1 / (1 + math.exp(-x))
def forward(inputs):
    total = inputs[0]*w1 + inputs[1]*w2 + bias
    return sigmoid(total)

lr = 0.1
for epoch in range(10000):
    for inputs, correct in data:
        out = forward(inputs)
        err = correct - out
        adj = err * out * (1 - out)  # sigmoid derivative
        w1 += adj * inputs[0] * lr
        w2 += adj * inputs[1] * lr
        bias += adj * lr

print(forward([0,0]), forward([0,1]), forward([1,0]), forward([1,1]))
```

### Results with AND logic
| Input | Expected | Learned |
|-------|----------|---------|
| [0,0] | 0 | ~0.0002 |
| [0,1] | 0 | ~0.055 |
| [1,0] | 0 | ~0.055 |
| [1,1] | 1 | ~0.934 |

### Proper Names
- Forward pass = running inputs to get prediction
- Loss/error = how wrong you were
- Backpropagation = nudging weights using error
- Gradient descent = the adjustment formula
- Epoch = one full pass through all training data

File: `~/Desktop/ai/neuron.py`
