# Neural Network Basics — Single Neuron from Scratch

> Hands-on ML fundamentals. Written 2026-05-16 during Iris project inception.
> Source: Claude-assisted tutorial. Ishi wrote the code line-by-line.

## The Single Neuron

A neuron is the smallest unit of a neural network. It takes numbers in, does maths, and outputs a prediction.

### Forward Pass

```
output = (input1 × weight1) + (input2 × weight2) + bias
```

- **Weights** = how much the neuron "cares about" each input
- **Bias** = a baseline nudge (the neuron's natural tendency)
- Weights + bias initialised with small random numbers (`random.uniform(-1, 1)`)

### Sigmoid Activation

Squashes any output into the range `[0, 1]`:

```
sigmoid(x) = 1 / (1 + e^(-x))
```

- Big positive number → close to 1
- Big negative number → close to 0
- **Cannot reach exactly 0 or 1** — asymptotic (e^-x never hits zero)
- Alternative: step function (outputs exact 0/1) but breaks gradient-based training
- Alternative: ReLU (`max(0, x)`) — used in modern networks, avoids vanishing gradients

### Training — Backpropagation

The training loop:
1. Run input through neuron → get prediction
2. Compare to correct answer → calculate error
3. Nudge weights in the right direction
4. Repeat thousands of times

**Nudge formula:**

```python
error = correct - output
adjustment = error * output * (1 - output)  # sigmoid derivative
w1 += adjustment * input1 * learning_rate
w2 += adjustment * input2 * learning_rate
bias += adjustment * learning_rate
```

- `output * (1 - output)` = sigmoid derivative — accounts for curve steepness
- `learning_rate` = small number (0.1) so we take small steps

**Epoch:** One full pass through all training data. ~10,000 epochs for simple learning.

## Working Code

```python
import random
import math

data = [
    ([0, 0], 0),
    ([1, 0], 0),
    ([0, 1], 0),
    ([1, 1], 1)
]

w1 = random.uniform(-1, 1)
w2 = random.uniform(-1, 1)
bias = random.uniform(-1, 1)

def sigmoid(x):
    return 1 / (1 + math.exp(-x))

def forward(inputs):
    total = (inputs[0] * w1) + (inputs[1] * w2) + bias
    return sigmoid(total)

learning_rate = 0.1

for epoch in range(10000):
    for inputs, correct in data:
        output = forward(inputs)
        error = correct - output
        adjustment = error * output * (1 - output)
        w1 += adjustment * inputs[0] * learning_rate
        w2 += adjustment * inputs[1] * learning_rate
        bias += adjustment * learning_rate

print(forward([0, 0]))
print(forward([0, 1]))
print(forward([1, 0]))
print(forward([1, 1]))
```

**Result with AND logic:**
| Input | Expected | Learned |
|-------|----------|---------|
| [0, 0] | 0 | 0.0002 |
| [0, 1] | 0 | 0.055 |
| [1, 0] | 0 | 0.055 |
| [1, 1] | 1 | 0.934 |

## Key Concepts (with proper names)

| What You Did | Proper Name |
|-------------|-------------|
| Run inputs → get prediction | Forward pass |
| Measure how wrong you were | Loss / error |
| Nudge weights using error | Backpropagation |
| `error * output * (1-output)` | Gradient descent with sigmoid derivative |

## Beyond One Neuron

- **OR gate** — one neuron handles it easily
- **XOR gate** — impossible for a single neuron (needs layers — the XOR problem)
- **Layers** — multiple connected neurons = a real neural network
- **ReLU** — modern activation function: `max(0, x)`
- **Evolutionary training** — no backpropagation: mutate survivors, keep the best
- **Reinforcement learning** — reward/punish instead of providing correct answer

## Hardware Context

- Ishi's machine: M1 MacBook Pro, 8GB RAM
- Can run ~1-3B parameter models locally via Ollama
- Can fine-tune Phi-3 Mini (3.8B) via MLX
- 8B models possible but slow
- GPT-3.5 level (~175B params) impossible locally — not an architecture problem, a parameter-capacity problem

## File Location

`~/Desktop/ai/neuron.py`
