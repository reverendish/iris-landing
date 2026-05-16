---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [forward-pass, xor, network-code, python]
processed: false
---

# Forward Pass for a 2-Layer XOR Network

## Question
(Code example — the forward pass for a network with hidden layers)

## Answer

### The Structure
```
Input A ──┬──→ Hidden Neuron 1 ──┬──→ Output → prediction
          │                        │
Input B ──┴──→ Hidden Neuron 2 ──┘
```

### Weights Needed
- **Hidden layer:** 4 weights (2 inputs × 2 neurons) + 2 biases
- **Output layer:** 2 weights (1 from each hidden neuron) + 1 bias

### Initialisation
```python
# Hidden layer: 2 neurons, each with 2 weights from A and B
h_weights = [
    [random.uniform(-1, 1), random.uniform(-1, 1)],  # neuron 1
    [random.uniform(-1, 1), random.uniform(-1, 1)],  # neuron 2
]
h_bias = [random.uniform(-1, 1), random.uniform(-1, 1)]

# Output layer: 1 neuron, 2 weights (one from each hidden)
o_weights = [random.uniform(-1, 1), random.uniform(-1, 1)]
o_bias = random.uniform(-1, 1)
```

### Forward Pass
```python
def sigmoid(x):
    return 1 / (1 + math.exp(-x))

def forward(inputs):
    # Run each hidden neuron
    h1 = sigmoid(inputs[0]*h_weights[0][0] + inputs[1]*h_weights[0][1] + h_bias[0])
    h2 = sigmoid(inputs[0]*h_weights[1][0] + inputs[1]*h_weights[1][1] + h_bias[1])
    
    # Hidden outputs become inputs to output neuron
    output = sigmoid(h1*o_weights[0] + h2*o_weights[1] + o_bias)
    
    return output, h1, h2
```

Three things to notice:
1. h1 and h2 are hidden neuron outputs — they become inputs to the output neuron
2. We return h1, h2 alongside final output — needed for backpropagation
3. The structure is identical to the single neuron, just done twice before the final step
