# Iris — AI Job Agent (Business & Market)

> Business analysis for the Iris project. See [[../../projects/iris|Iris project]] for the full project file.

## Market Landscape

### Direct Competitors

| Company | What They Do | Gap |
|---------|-------------|-----|
| **Simplify** | Autofills job apps, browser extension, tracking | Mail merge, no tone capture |
| **Sonara** | Automated job applying — finds + applies | Bulk spamming, low quality |
| **LazyApply** | Bulk apply to jobs via extension | Zero personalisation |
| **Kickresume / Resume.io** | CV building + some app help | Templates, not AI-native |
| **Final Round AI / Interview.ai** | Interview prep side | Different angle entirely |

### The Real Gap

Everything existing is mail-merge with a CV. Cover letters are obviously AI-generated. Recruiters can tell immediately.

**Iris's differentiator:** Captures tone through conversation. The grill_me-style onboarding interviews the user until it understands how they think and write. No templates.

### Risks

⚠️ **Job boards actively block scrapers** — LinkedIn, Indeed especially. Technical and legal headache.
⚠️ **Subscription business** — needs volume to make real money.
⚠️ **Competing with funded companies** — Simplify has raised millions.

### Advantages

✅ Tone-capture onboarding is genuinely novel
✅ Founder understands every layer of the system (built from scratch)
✅ Could work as a small profitable indie product without beating Simplify
✅ **500 users at £20/month = £10k/month**
✅ Can niche down hard (tech roles, UK, creative industries)

## Product Onboarding Flow

```
1. User uploads CV
2. System reads CV, identifies gaps/ambiguities
3. Conversational interview:
   - "Tell me about this project"
   - "How would you describe your working style?"
   - "What would your last manager say about you?"
4. Builds tone profile + personality map
5. Generates test cover letter → user rates/edits
6. System learns from edits
7. Locked in — ready to apply
```

## Validation Strategy

**Phase 1 — Waitlist (free, zero code)**
1. Carrd landing page (carrd.co) — one-page site, free
2. Tally.so form collecting: name, email, industry
3. Optional: domain from Porkbun (~£5/yr)

**Phase 2 — Manual MVP (do things that don't scale)**
1. Conduct conversations by hand for 3-5 real people
2. Write cover letters yourself
3. Apply manually
4. Learn what actually matters, then automate

## Naming

- **Iris** — Greek goddess of messages and rainbows, messenger between gods and humans
- Domain candidates: meetiris.co.uk, heyiris.co.uk
- Clean, 4 letters, memorable, mythological

## Target Pricing

- £20/month subscription
- Free tier: limited applications, basic matching
- Paid: unlimited, full tone personalisation, priority jobs
