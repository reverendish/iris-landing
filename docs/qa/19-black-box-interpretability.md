---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [interpretability, black-box, ai-concepts]
processed: false
---

# The Black Box Question: Can You Trace Why AI Decides What It Does?

## Question
Is this why people say AI is a black box? Surely that can't be true — all you'd have to do is follow the error signal?

## Answer

### You're Half Right
You CAN follow the error signal. You can see which inputs each neuron weighted heavily. Researchers do this — it's called **interpretability** and it's an entire field.

### Why It's Still Called a Black Box
The weights don't come with explanations. A neuron might weight input 3 heavily, but it won't tell you *why* in human language. You can see that it matters, not why it matters in a way that makes intuitive sense.

With billions of parameters, the relationships become so tangled that even following every weight doesn't give a clean human-readable reason. It's not that you can't look — it's that what you see doesn't translate neatly into language.

### Analogy
Try to explain why you recognised a friend's face. You can't list the rules. You just know. Neural networks are similar — knowledge is distributed across millions of weights with no single place where the "reason" lives.

### Why This Matters for Iris
If Iris rejects a job you wanted, can you understand why? That's a feature worth building — show the user which inputs scored low. That's **interpretability made useful**.
