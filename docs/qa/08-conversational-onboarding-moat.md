---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [onboarding, conversational-ux, tone-capture, product-differentiation]
processed: false
---

# Conversational Onboarding as a Moat

## Question
I want an onboarding where the user uploads a CV, then the system has a conversation with them until it understands their tone — like Matt Pocock's grill_me skill.

## Answer

### The Onboarding Flow
```
User uploads CV → System reads it, finds gaps → 
Conversational interview ("tell me about this project",
"what would your last manager say about you?") → 
Builds tone profile + personality map → 
Generates test cover letter → user rates/edits → 
System learns from edits → Locked in
```

### Why This is the Moat
The conversation that builds understanding is a great use of a small orchestration layer:
- One model reads the CV
- One conducts the interview
- One synthesises the tone profile
- One generates applications
- All small, all specialised, all coordinated

Mail merge is easy to build. Conversational tone capture is hard — it creates a defensible moat. Every conversation trains the model better.
