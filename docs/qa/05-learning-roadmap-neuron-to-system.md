---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [learning-roadmap, transformers, fine-tuning, orchestration, deployable-system]
processed: false
---

# Learning Roadmap: From Neuron to Deployable System

## Question
I want to do transformers from scratch, tiny MoE, fine-tune Phi-3 Mini, build orchestration, AND make a useful narrow deployable system.

## Answer

### The Order (each builds on the last)
```
Neuron (DONE) → Transformers → Tiny MoE → Fine-tune Phi-3 → Orchestration → Iris
```

### What Each Stage Involves
| Stage | What | Time |
|-------|------|------|
| 0 | Single neuron (AND logic) | Done |
| 1 | Tiny transformer from scratch | Weeks |
| 2 | Tiny MoE from scratch | Weeks |
| 3 | Fine-tune Phi-3 Mini via MLX | Days |
| 4 | Orchestration layer | Weeks |
| 5 | Narrow deployable system | Depends |

### Key Insight
Choose the final domain early — use that training data throughout all stages. For Iris:
- Stage 1: transformer trains on your writing samples
- Stage 2: MoE routes "cover letter" vs "CV matching" vs "job scoring"
- Stage 3: fine-tune on job application data
- Stage 4: coordinates everything
- Stage 5: ships it
