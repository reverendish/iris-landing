# Iris — AI Job Application Agent

> **Project Iris.** Personal recruitment agent that learns your voice, finds relevant jobs, and applies with cover letters that actually sound like you.

## Status

✅ **Waitlist live** — Landing page at `https://reverendish.github.io/iris-landing/`
🔄 **Inception** — Idea stage, validated concept with Claude, beginning technical upskilling.

## Core Idea

A narrow-deployable AI system that:
1. **Onboards through conversation** — interviews the user (like Matt Pocock's grill_me) until it understands their tone, style, and thinking
2. **Finds quality jobs** — scrapes/filters job boards by criteria, scores relevance against CV
3. **Applies in your voice** — generates personalised cover letters from a fine-tuned small model, not templates
4. **Keeps you in control** — you approve everything before it sends

## Differentiator

Existing tools (Simplify, LazyApply, Sonara) do mail-merge with your CV. Iris captures *tone through conversation* — the onboarding itself is the moat. Recruiters can tell when a cover letter is AI-slop; Iris aims to sound indistinguishable from the real person.

## Technical Roadmap

The project doubles as Ishi's AI/ML education. Each stage builds a skill needed for the final system.

| Stage | What | What It Teaches |
|-------|------|-----------------|
| ✅ Stage 0 | Single neuron from scratch (AND logic) | Forward pass, sigmoid, backpropagation, gradient descent |
| 🔲 Stage 1 | Transformers from scratch | Attention mechanism, embeddings, tokens |
| 🔲 Stage 2 | Tiny Mixture of Experts from scratch | Router model, specialist sub-models, orchestration |
| 🔲 Stage 3 | Fine-tune Phi-3 Mini (MLX on M1) | Real model training on custom data |
| 🔲 Stage 4 | Orchestration layer | Coordinate multiple models, pass context, aggregate outputs |
| 🔲 Stage 5 | Narrow deployable system | Full product — Iris |

## Business Model

- **Target:** £20/month subscription, indie/SaaS model
- **Validation method:** Landing page with waitlist (Carrd + Tally.so) before building
- **Niche option:** Start with tech roles, UK market, or creative industries
- **Aspirational:" €10k/month = 500 paying users at £20/month"
- **Competition:** Simplify, Kickresume, Sonara, LazyApply, Final Round AI

## Market Insight

The gap in existing products: none of them genuinely capture *tone*. They slot CV details into templates. The conversational onboarding that builds a personality profile is a novel product approach.

## Key Decisions

- **Product name:** Iris (mythology — messenger goddess, guides between worlds)
- **Validation-first:** Landing page + waitlist before any code (do things that don't scale)
- **Learning = building:** Every technical stage feeds directly into the final product
- **Domain:** meetiris.co.uk or similar (check Porkbun ~£5/yr)
- **Waitlist:** GitHub Pages (`reverendish/iris-landing`), FormSubmit.co for email collection (sends to Gmail)
- **Stack:** Python, MLX (Apple ML framework for M1), Playwright (browser automation)
- **Small model approach:** Fine-tuned Phi-3 Mini (3.8B) for cover letters, small classifier for job scoring

## Tech Stack (planned)

- **Python** — primary language
- **MLX** — Apple's ML framework (optimised for M1/M2)
- **Phi-3 Mini** — small model candidate for cover letter fine-tuning
- **Playwright** — browser automation for applying
- **Carrd + Tally.so** — landing page and waitlist (free tier)

## Learning Resources Generated

- [[../wiki/research/ai/neural-network-basics|Neural Network Basics]] — The single-neuron tutorial written during ideation
- [[../wiki/research/ai/transformer-architecture|Transformer Architecture]] — Technical notes (existing)
- `~/Desktop/ai/neuron.py` — Working single-neuron implementation

## History

- **2026-05-16:** Project conceived during AI/ML fundamentals session with Claude. Single neuron built and trained. Iris name chosen. Waitlist concept validated. Decision to learn-by-building toward a real product.
- **2026-05-16 (10:15):** Landing page live at `https://reverendish.github.io/iris-landing/`. FormSubmit.co collecting submissions to Gmail.
