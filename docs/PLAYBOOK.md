# Solo Founder Launch Playbook — Skeleton

> A repeatable workflow for vetting and launching business ideas.
> Zero budget. Solo founder. Everything in Second Brain.
> Case study: Iris (tracked alongside).

---

## The Pipeline

```
IDEA → QUICK KILL → MARKET PULSE → WAITLIST → GATE → MVP → LAUNCH
 5min     30min        1-2hrs       1hr       5min     weeks    event
```

---

## Stage 1 — Idea Spark (5 min)

**When:** A random idea hits you. Capture it immediately.

**Actions:**
- Write the idea into `~/SecondBrain/00-INBOX/ideas/` as a raw note
- One file per idea: `idea-name-YYYY-MM-DD.md`
- Frontmatter: `type: idea-spark`, `status: raw`, `created: date`
- Write whatever's in your head. No structure needed.

**Tool:** Any text editor, Obsidian, or tell OpenClaw "save this idea"

**Output:** A raw file in the inbox. Nothing more.

---

## Stage 2 — Quick Kill (30 min)

**When:** You have 30 minutes and want to see if the idea survives first contact with reality.

**Actions:**
1. **Competition check** — Google, Reddit, Product Hunt. Does it exist? Who does it well?
2. **Demand check** — Are people actually searching/buying/asking for this?
3. **"Can I do this?" check** — Does it fit your skills? Your hardware (M1 8GB)? Your time?
4. **"Will I enjoy this?" check** — Brutally honest. If you won't enjoy 100 hours of it, drop it.

**Decision gate:** If any of the 4 checks fail hard → kill it. Move on.
If all pass → move to Stage 3.

**Output:** Update the idea file with findings. Add tags: `survived-stage2` or `killed`.

---

## Stage 3 — Market Pulse (1-2 hours)

**When:** The idea survived stage 2. Now dig deeper before building anything.

**Actions:**
1. **Talk to 5 people** — Real humans in your target audience. Ask open questions, don't pitch.
2. **Reddit research** — Search relevant subreddits. What do people complain about? What do they wish existed?
3. **Value proposition draft** — Write one sentence: "Iris does X for Y so that Z"
4. **Price signal** — Check if anyone is paying for solutions in this space. How much?

**Decision gate:** If you can't articulate the value prop in one sentence → rework or kill.
If 3/5 people say "I'd use that" → move to Stage 4.

**Output:** Market notes appended to the idea file. Value prop written.

---

## Stage 4 — Waitlist (1 hour)

**When:** You've validated enough to warrant a landing page.

**Template (use Iris):**
- GitHub Pages repo (`project-name-landing`)
- Clean dark-theme landing page (copy from iris-landing)
- FormSubmit.co to your Gmail (free, unlimited)
- 3-4 value props + email signup

**Actions:**
1. Clone iris-landing as a template
2. Swap text for the new idea
3. Push to GitHub
4. Enable Pages

**Goal:** 10 signups = low signal. 50+ signups without any real marketing = strong signal.

**Output:** Live landing page, waitlist collecting emails, first signup data.

---

## Stage 5 — Decision Gate (5 min)

**When:** Waitlist has been live for 1-2 weeks. You have data.

**Questions:**
- How many signups? (0-10 = weak, 10-50 = promising, 50+ = strong)
- What did Reddit/LinkedIn think? (upvotes, comments, DMs?)
- Do YOU still want to build this? (honestly)
- Can you build an MVP in 2-4 weeks?

**Decisions:**
- **Kill** — Archive idea file. Move on. No shame.
- **Park** — Not now, but revisit in 3 months.
- **Build** — Proceed to Stage 6.

**Output:** Update idea file with decision. Tag accordingly.

---

## Stage 6 — MVP Build (2-4 weeks)

**When:** You've decided to build.

**Principles:**
- Scope to the absolute minimum (1 feature that delivers the core promise)
- Time-box (2 weeks is better than 4)
- Build in public (Twitter, LinkedIn)
- Track progress in Second Brain journal

**Output:** Working prototype. 5-10 test users. Feedback loop.

---

## Stage 7 — Launch

**When:** MVP works for real users.

**Free launch channels:**
- Product Hunt (free tier)
- Hacker News Show HN
- Reddit (r/SideProject, r/startups, niche subreddits)
- Build-in-public communities (Indie Hackers, Twitter)

**Goal:** 200+ users, validation that people will pay, or clear signal to pivot.

---

## Tools Stack (all free)

| Tool | Use Case | Why |
|------|----------|-----|
| GitHub Pages | Landing page hosting | Free, custom domain, fast |
| FormSubmit.co | Email collection | Free, unlimited, no account |
| Second Brain (Obsidian) | Project tracking | Already set up |
| GitHub | Version control + repo hosting | Already set up |
| Gmail | Form submissions | Already set up |
| Twitter/LinkedIn/Reddit | Distribution | Free |
| Product Hunt | Launch | Free tier |
| Ollama + DeepSeek API | AI work | Already using |

---

## Second Brain File Structure

```
SecondBrain/
├── projects/
│   ├── iris.md                          ← your project
│   ├── iris-outreach-campaign.md        ← your campaign
│   └── <new-idea>.md                    ← next one
├── 00-INBOX/ideas/
│   └── <idea-name-YYYY-MM-DD>.md        ← stage 1
└── daily-context.md                     ← decisions logged here
```

---

## Case Study: Iris (for reference)

- **Idea Spark:** Wrote in conversation with Claude
- **Quick Kill:** Checked competitors (Simplify, LazyApply, Sonara), found gap
- **Market Pulse:** Claude conversation validated demand
- **Waitlist:** GitHub Pages + FormSubmit.co, live within hours
- **Decision Gate:** TBD (waitlist needs 2 weeks of data)
- **Next:** Build Stage 0-5 technical roadmap → then prototype

---

*Skeleton v0.1 — ready to refine together. Cron set for Sunday 10am.*
