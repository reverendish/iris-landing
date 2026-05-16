---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [inputs, feature-engineering, data-quality]
processed: false
---

# The Purpose of Inputs in a Neural Network

## Question
What's the purpose of inputs? Why do relationships between them matter? Surely inputs aren't just "questions" — they can be anything?

## Answer

### Inputs Are Just Measurements
Anything you can measure or represent as a number can be an input. Questions are one way to get them but not the only way.

| What You're Predicting | Possible Inputs |
|---|---|
| Will this email get a reply? | Word count, time sent, sender history |
| Is this photo a cat? | Brightness of every pixel |
| Will this job application succeed? | Years experience, keyword matches |
| Should Iris apply to this job? | Salary match, role match, location, seniority |

### Why Relationships Matter
Example: Salary match = high, role match = low. A single neuron learns "high salary = apply" — wrong. A hidden layer learns the relationship: *both* salary AND role need to match. Neither alone is enough. That's a relationship between inputs, and one neuron can't learn it.

### More Inputs ≠ Better Output
**More relevant inputs** → better output. **More irrelevant inputs** → worse output.

If you add "favourite colour" as an input to Iris, the network might accidentally learn "blue lovers get jobs" from noise in training data. This is **overfitting** — learning the training data too well, including its accidents.

### Feature Engineering
Everything the network knows about a situation comes through input numbers. The richer your relevant inputs, the more the network has to work with. This is called feature engineering — it matters as much as the architecture itself.

For Iris:
- Bad inputs: `[job title, company name]`
- Good inputs: `[salary match, role match, location match, seniority match, tech stack overlap, company size, remote preference]`
