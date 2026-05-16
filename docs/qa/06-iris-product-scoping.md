---
agent: main
created: 2026-05-16
type: clipping
source: "Claude chat (Ishi's ML learning session)"
project: iris
tags: [product-scoping, job-application, system-design, features]
processed: false
---

# Iris Product Scoping

## Question
The best thing I could think of is something that finds and applies to jobs for me in my tone.

## Answer

### What the System Needs to Do
1. **Find jobs** — scrape/pull from job boards, filter by criteria
2. **Score relevance** — match CV against job description (classifier, small model)
3. **Write in your voice** — fine-tuned model generates personalised cover letters
4. **Apply** — autofill forms, email directly, flag human-needed cases

### Component Map
| Component | Tool |
|-----------|------|
| Job finding | Python scraper + APIs |
| Relevance scoring | Small classifier (< 100M params) |
| Cover letter gen | Fine-tuned Phi-3 Mini |
| Orchestration | Router coordinating everything |
| Applying | Playwright browser automation |

### What You Need
- Your CV
- 5-10 cover letters/emails (capture your tone)
- Job criteria (role, location, salary, remote)
- Example good/bad job listings for calibration
