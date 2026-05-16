# Iris — Outreach Campaign

> Pre-launch outreach strategy for a solo-built, zero-budget product.
> Waitlist at https://reverendish.github.io/iris-landing/
> Status: Pre-revenue, pre-product, waitlist-only.

---

## 1. Core Truths to Anchor Everything

**The product doesn't exist yet.** The only thing we're selling is the waitlist — a promise that something better is coming. Every piece of outreach must either: get a signup, gather market intelligence, or build an audience for launch day.

**The differentiator is conversational onboarding.** Existing tools (Simplify, LazyApply, Sonara) are mail-merge machines. Iris learns your tone through conversation. That's the hill we die on.

**The audience is burned out.** Job seekers have been spammed by AI tools, ghosted by recruiters, and told to "network more." They're cynical. Meet them with honesty, not hype.

**Zero budget.** Every channel must be free. Time is the only currency.

---

## 2. Target Audience Breakdown

### Tier 1 — Immediate (highest signal)
| Segment | Where to Find Them | Why They Care |
|---------|-------------------|---------------|
| Tech workers actively job hunting | r/cscareerquestions, r/jobs, r/ExperiencedDevs | They apply to 50+ roles, know how bad templates are |
| UK tech workers | r/UKJobs, r/cscareerquestionsuk, LinkedIn UK | Founder is UK-based, product can start local |
| Career changers | r/careerguidance, r/careerchange, Reddit in general | Most desperate for tailored applications |
| Indie hackers / solo builders | IndieHackers.com, r/indiehacking, Twitter build-in-public | They'll root for you and give feedback |

### Tier 2 — Medium signal
| Segment | Where to Find Them | Why They Care |
|---------|-------------------|---------------|
| Designers / creatives | r/design, Dribbble, Behance | Portfolio-heavy, tone matters hugely |
| Remote job seekers | r/remotework, r/digitalnomad | High-volume applications, need differentiation |
| Underrepresented in tech | r/girlsgonewired, diversity-focused groups | Generic AI tools amplify bias, personalised tools don't |
| Recruiters (as partners, not users) | LinkedIn, r/recruiting | They hate generic applications too — potential referral source |

### Tier 3 — Long-term
| Segment | Where to Find Them | Why They Care |
|---------|-------------------|---------------|
| Recent graduates | r/csmajors, university career centres | First job hunt, most insecure about applications |
| General workforce | LinkedIn, Facebook groups | Mass market — lowest conversion but largest pool |

---

## 3. Channel Strategy

### Reddit — Primary channel

**Why:** Free, large engaged audience, can post value-first content. The product itself validates via conversation — Reddit is built for conversation.

**Approach by subreddit:**

| Subreddit | Strategy | Frequency |
|-----------|----------|-----------|
| r/jobs | Share personal story "I built a tool that applies to jobs in my actual voice" | 1 post ever (no promo) |
| r/cscareerquestions | Technical post about building a tiny MoE / training a personalisation model | 1 post ever (value-first) |
| r/UKJobs | "I'm building a UK-focused job application tool. What do you hate most about applying?" | Market research post |
| r/careerguidance | Comment on existing threads about cover letters, applications | Ongoing (organic) |
| r/ExperiencedDevs | Post about the architecture choices (small models, MoE, orchestration) | 1 post ever (dev audience) |
| r/SideProject | Share the landing page + ask for feedback | 1 post |
| r/startups | Launch announcement when ready | 1 post at launch |
| r/alphaandbetausers | Post the waitlist for early testers | 1 post |

**Reddit Post Drafts:**

*Draft 1 — Personal story (r/jobs)*
> Title: I got so tired of writing cover letters that I built an AI that writes them in my voice
> 
> Body: Brief personal story about the job hunt struggle. Mention trying existing tools and hating the generic output. Describe the conversational onboarding approach. Link to waitlist. Be transparent: "Still building this, no product yet. Just putting a flag in the ground."

*Draft 2 — Architecture (r/ExperiencedDevs)*
> Title: I'm building a small-model approach to personalised cover letters — here's why I chose MoE over a single big model
> 
> Body: Technical discussion. 1M param classifiers vs fine-tuned 3.8B. Router architecture. Why tone capture needs conversation, not templates. The dev audience loves architecture talk. No direct product plug — just mention what you're building naturally.

*Draft 3 — Market research (r/UKJobs)*
> Title: UK job seekers: what's your biggest frustration with cover letters?
> 
> Body: Simple question. Gather data. Learn what features matter. Reference at end: "I'm building something to address this — will share when it's ready."

### LinkedIn — Founder presence

**Strategy:** Don't pitch. Build in public. Ishi posts 2-3x/week about:
1. The technical learning journey (neuron → transformer → MoE → fine-tuning)
2. The product decisions (why conversational onboarding, why small models)
3. The founder struggle (solo, bootstrapped, trying to hit £2k/month)
4. Job market observations (what's broken, what people actually want)

**Post types:**
- "Today I learned X" — short technical notes
- "Decision log: why I chose Y over Z" — architecture/strategy posts
- "At signup #5 I learned..." — user research insights
- "Iris update: week 1" — builder diary

**Connection targets:**
- UK recruiters (50-100 connections)
- Tech workers who post about job hunting
- Indie founders (engage with their posts first)
- Product Hunt community members

**DM strategy:** None for now. Build audience first.

### Twitter/X — Build in public

**Handle:** @reverendish (existing) — can use for Iris content or create @heyiris

**Content rhythm:**
- Daily: 1-2 tweets about the build process
- Weekly: 1 thread about the problem/journey
- Monthly: 1 "state of the build" update

**Thread idea — "I'm building an AI that applies to jobs for me"**
> 1/ I've applied to 50 jobs this month. Every cover letter was AI slop. Recruiters know.
> 2/ So I'm building Iris. An agent that learns how I actually write, then applies in my voice.
> 3/ Not a template. Not chatGPT with my CV copy-pasted. An actual conversation that builds a tone model.
> 4/ Waitlist is live. Building in public. Follow along.

### Hacker News — Show HN

**When:** When there's a demo worth showing (not now).
**What:** A working prototype that someone can try. Even if it's janky.
**Title formula:** "Show HN: Iris – an AI agent that applies to jobs in your voice"
**Prep:** Have 3-5 friends test it first. Prepare for brutal feedback.

### Product Hunt

**When:** Launch day — after Reddit and Twitter momentum.
**What:** Free tier launch. No need for Product Hunt Pro.
**Prep:** Maker profile, first comment with story, engage every comment.

### Content Marketing — SEO play

**Blog posts to write (free, on GitHub or Substack):**
1. "Why existing AI job tools are hurting your chances" — problem analysis
2. "How I'm building a personalisation AI with < 8GB of RAM" — technical
3. "The cover letter is dead — here's what replaces it" — opinion piece
4. "I talked to 50 job seekers. Here's what they actually want." — research
5. "Building a product for a market that doesn't know it needs you yet" — founder story

**SEO keywords to target:**
- "AI cover letter generator" (high competition, long-tail instead)
- "personalised job application tool"
- "apply to jobs for me"  
- "job application automation"
- "cover letter that sounds like me"
- "best AI for job applications 2026"
- "AI job agent"

---

## 4. Launch Sequence (Timeline)

### Phase 1: Validation (Week 1 — NOW)
| Action | Channel | Goal |
|--------|---------|------|
| Share waitlist link with close contacts | DM, WhatsApp | First 5 signups + feedback |
| Post market research | r/UKJobs, r/careerguidance | 10-20 signups + user insights |
| Start build-in-public | Twitter/X | Followers + credibility |
| Connect with 20 UK recruiters | LinkedIn | Future distribution channel |

### Phase 2: Pre-launch (Week 2-4)
| Action | Channel | Goal |
|--------|---------|------|
| Personal story post | r/jobs, r/cscareerquestions | 50+ signups |
| Technical architecture post | r/ExperiencedDevs | Developer curiosity + credibility |
| First blog post | GitHub Pages / Substack | SEO seed content |
| 2-3 LinkedIn posts per week | LinkedIn | 100+ connections |
| Daily Twitter content | Twitter/X | 50-100 followers |

### Phase 3: Launch (Week 4-6 — when prototype is demoable)
| Action | Channel | Goal |
|--------|---------|------|
| Show HN post | Hacker News | 200+ upvotes, traffic spike |
| Product Hunt launch | Product Hunt | Front page, 500+ signups |
| Side Project post | r/SideProject | Developer curiosity |
| Reddit wave (posts on 3 subreddits same day) | Reddit | Organic virality |

### Phase 4: Scale (Month 2-3)
| Action | Channel | Goal |
|--------|---------|------|
| Weekly blog posts | Blog | SEO compounding |
| Recruiter partnerships | LinkedIn | Referral pipeline |
| Iterate on user feedback | All | Product-market fit |
| Consider paid ads | ? | Only if margins justify |

---

## 5. Messaging Framework

### Elevator Pitch (1 sentence)
"Iris is an AI agent that learns how you write through conversation, then finds and applies to jobs in your voice — no templates."

### The Problem (for landing page and outreach)
"AI cover letter tools today are mail-merge with your CV. Recruiters can tell immediately. Iris does it differently — it interviews you until it understands your tone, then generates applications that sound like a real person."

### The Promise (for signups)
"You write fewer applications. Each one sounds like you. You get more interviews."

### The Honest Truth (for Reddit / indie audiences)
"I'm a solo founder building this publicly. No VC, no investors. The product isn't ready yet — but the waitlist is live. If this sounds like something you'd use, get on the list and I'll keep you updated."

### Key Phrases to Use Everywhere
- "Your voice, not a template"
- "Applies in your actual tone"
- "Onboards through conversation"
- "Quality over quantity"
- "You stay in control"
- "Trained on you, not on generic data"

### Key Phrases to Avoid
- "Revolutionary" / "Game-changing" / "Disruptive" (overused, signals hype)
- "AI-powered" (everyone says this, means nothing)
- "Never write a cover letter again" (overpromise, sounds like a spam tool)
- "10x your applications" (signals bulk-spam approach, which is the opposite of Iris)

---

## 6. Metrics & Milestones

### Pre-launch Metrics
| Metric | Target (30 days) | Why |
|--------|------------------|-----|
| Waitlist signups | 100 | Validates demand |
| Twitter followers | 200 | Distribution channel |
| LinkedIn connections | 100 | Recruiter partnerships |
| Blog posts published | 3 | SEO foundation |
| Reddit posts with 50+ upvotes | 2 | Organic reach |
| User conversations (meaningful feedback) | 10 | Product direction |

### Launch Day Metrics
| Metric | Target |
|--------|--------|
| Product Hunt upvotes | 100+ |
| Hacker News upvotes | 50+ |
| New waitlist signups | 200+ |
| Website visitors | 2000+ |
| Newsletter signups (if separate) | 100+ |

### Ongoing Metrics
| Metric | How to Track |
|--------|-------------|
| Waitlist → engaged user conversion | Manual tracking |
| Referral signups | Ask "how did you hear about us?" in form |
| Subreddit traffic | UTM parameters on links |
| Most effective post type | Compare engagement per platform |

---

## 7. Constraints & Risks

**Zero budget, only time.** Everything above is free. If any channel requires money, skip it.

**No product to demo.** We can't show screenshots or walkthroughs. Outreach must sell the vision and the founder, not features.

**Founder energy is limited.** Ishi is also learning ML from scratch and may need to build the product. Outreach shouldn't consume more than 30 mins/day.

**Job boards block scrapers.** The messaging should emphasise personalised cover letters, not bulk automation. Don't sound like LazyApply.

**UK focus = smaller audience.** But also less competition. Local credibility ("built by someone in the UK job market") is an advantage.

**Reddit bans self-promotion.** Every Reddit post must pass the "would this be valuable even without the link?" test. 80% value, 20% mention.

---

## 8. Content Calendar (Week 1)

| Day | Platform | Content |
|-----|----------|---------|
| Sat 16 May | — | Landing page live ✅ |
| Sat 16 May | WhatsApp/DM | Send waitlist to 5 friends "what do you think?" |
| Sun 17 May | Twitter | First build-in-public tweet: "New project: Iris — an AI job agent that learns your voice. Waitlist is up." |
| Mon 18 May | r/UKJobs | Market research post: "UK job seekers: what frustrates you about cover letters?" |
| Mon 18 May | LinkedIn | "I'm building something new" — short post about the problem, link to waitlist |
| Tue 19 May | Twitter | Thread: "How I'm building a personalisation AI on an 8GB M1 MacBook" |
| Wed 20 May | LinkedIn | Technical learning update: "Today I built a neuron from scratch" |
| Thu 21 May | r/careerguidance | Comment on 3-5 existing threads about applications |
| Fri 22 May | Blog | First post on GitHub Pages: "Why existing AI job tools aren't solving the real problem" |
| Sat 23 May | Review | Review first week metrics. Adjust. |

---

## 9. Competitive Positioning (for messaging)

| Competitor | Position | How Iris is Different |
|-----------|----------|----------------------|
| Simplify | Autofill + tracking | Iris writes in your voice, doesn't just fill forms |
| LazyApply | Bulk apply to everything | Iris applies to fewer jobs with higher quality |
| Sonara | Automated job search + apply | Same — quality + personalisation differentiator |
| Kickresume / CV builders | Templates | Iris is dynamic, conversational, not static |
| ChatGPT + CV copy-paste | Manual | Iris is automated with a captured voice model |
| Recruiters (human) | Human touch | Iris is faster, cheaper, always available |

The competition is LESS intimidating when framed this way. No one is doing conversational tone capture. The slot is open.

---

## 10. Quick-Start Checklist (what to do today)

- [x] Landing page live on GitHub Pages
- [x] Form submit sending to Gmail
- [ ] Buy meetiris.co.uk (~£5 on Porkbun)
- [ ] Point domain to GitHub Pages
- [x] Fix trust line on landing page
- [ ] Send waitlist link to 5 people via DM/WhatsApp
- [ ] Create Twitter thread draft
- [ ] Draft r/UKJobs market research post
- [ ] Draft r/jobs personal story post
- [ ] Post first LinkedIn update
- [ ] Set up Google Analytics on landing page (or simpler: GitHub repo stars = vanity metric)
- [ ] Add UTM parameters to all future links

---

*Outreach campaign v1 — 2026-05-16*
*Generated by OpenClaw for Ishi. Review before executing any external actions.*
