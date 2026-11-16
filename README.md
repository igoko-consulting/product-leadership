# Fable Growth: Product Leadership Final Project, by Martin Cook

> My final project for Product School's **Product Leadership** certification. One scenario, **Fable Growth** (B2C mental wellness), taken from a board-ready product strategy to a complete business case across six in-class labs.

**How to read this repo:** start with the strategy sentence and the thread below. Each module folder then holds its deliverable and a `NOTES.md` with the module's ideas, my takeaways and how each lab decision was made. [PROMPTS.md](PROMPTS.md) keeps every lab prompt, run word for word in GPT-6 and Claude, and how the replies differed; each module's `ai-replies/` folder holds both models' replies as evidence.

---

## The strategy in one sentence

Fable bets its one initiative on the people it helped through a hard stretch: a personal nightly wind-down keeps them once they recover, and the community layer waits.

## The scenario: Fable Growth

*Fictional course material; Headspace and Calm appear only as the scenario's named competitors.*

- **The company:** a mental-wellness app for adults aged 25 to 45, built on guided meditations, sleep stories and breathing exercises. It peaked at 4.2M active users, known as the app that helped people through a hard stretch.
- **The problem:** growth has stalled because the product solves its first job. Deep users, usually in a high-stress period, recover within 90 to 120 days and drift away, with no next step. The users most likely to pay are the most likely to leave.
- **The market:** Headspace and Calm own awareness; AI mental-health apps target the same users with more personalisation.
- **The open call:** budget for one major initiative, and three camps: clinical wants CBT programmes, growth wants a community and social layer, content wants more content.
- **Constraints:** no repositioning as clinical; meditation and sleep content stays the foundation; the real competitor for the post-acute user is deciding they don't need Fable; a team of 14 across product, design, engineering, content and clinical advisory; the existing freemium and premium model.

**The other scenario** (Module 4's negotiation and Module 5's funding case use both): Meridian Foundations, a construction project-management platform and the system of record for 38 of the top 100 US general contractors. Its field teams barely use it and run the job on phone photos and group texts, while firms on $5M to $50M projects churn to simpler mobile-first tools. The enterprise team wants analytics, ERP integrations and the top 10 contractors; the product team wants a mobile field experience. Constraints: additive to the core platform, no removing features finance and compliance use, a team of 10, and the field first.

## Terms used in this repo

- **Hard stretch:** the period of high stress that brings someone to Fable, usually resolved within 90 to 120 days.
- **Post-acute users:** people whose need is easing after the hard stretch, about day 60 to 120. The strategy's target.
- **Deep users:** people who used Fable heavily in their first 90 days, the most likely to pay and the most likely to leave. Churned deep users have already left.
- **Steady plan:** each user's personal plan, built around a nightly wind-down from the meditation and sleep content that helped them before.
- **Nightly wind-down:** the bedtime session the steady plan is built around. KR2 counts the nights it is used.
- **Self-check:** a check the user starts, which brings back what worked. Fable never monitors or diagnoses.
- **Acute-level use:** the in-app pattern of a new hard stretch, with a non-diagnostic definition still to agree with the clinical advisers.
- **Concierge test:** the steady plan hand-built by the content team for a small consenting group, used in Now to test demand, nightly use and willingness to pay before building it. It replaced a fake door, an offer for a feature not yet built.
- **PM 1, PM 2, PM 3:** the scenario's three PMs, owning onboarding (days 0 to 60), retention (the post-acute experience, accountable for KR1–KR3) and the AI check-in layer.
- **Fable product lead:** my role in the scenario, over the three PMs. Only the product lead moves work between Now, Next and Later, and settles conflicts the PMs can't.
- **Shared services and shared platform:** shared services are teams outside the 14 lent to the initiative (Growth, Legal/Privacy, Data/Insights, Commercial); the shared platform is PM 3's AI check-in layer, which PM 1 and PM 2 both use.
- **Plateau:** day-180 retention flat for two monthly cohorts after the steady plan launches, judged by the Fable product lead at the monthly cohort review. It is the only condition for the buddy test.
- **Rocks and hard nos:** the quarter's three strategic bets, and three valuable things deliberately not done.

## How each module builds on the last

| Module | What I decided | What the next module takes from it |
|---|---|---|
| **M1** Strategy & OKRs | Post-acute users who still use sleep content; a steady plan built around a nightly wind-down, fitted by what helped them in the hard stretch; self-checks the user starts, not monitoring; no community layer. KR1 day-180 retention on monthly plans, KR2 wind-down nights, KR3 steady without feeling dependent, all by month 12. | Every M2 rock links to a KR, and the roadmap prompt carries the strategy word for word. |
| **M2** Roadmap | Rocks: the steady plan and self-check (backlog #6, KR3), the notification fix (#4, KR2), load time (#14, KR2). Hard nos: #5 therapist-matching tier, #3 social layer, #2 daily streak. Now tests demand first with a concierge test (plans hand-built for a small consenting group) and a stop rule; the Growth team co-owns the bedtime reminders; Next builds the steady plan only if the test passes. | M3's charter settles the tension with the Growth team; M4 writes a hard no to the Growth lead; M5 builds the business case for one rock. |
| **M3** Team charter | PM 2 owns the post-acute experience and KR1–KR3; PM 1 owns days 0 to 60; PM 3's AI layer is a shared platform whose output after day 60 is PM 2's call; the bedtime reminder is shared with Growth; Fable never starts a check-in. Conflicts go to a one-page note, then the Fable product lead, or the CPO when Growth is a party. | M4 writes a hard no to the Growth lead, the other side of this tension. |
| **M4** Stakeholder message | A hard no to the Growth lead: no community and social layer or progress sharing. What stays open is the bedtime reminder Growth co-owns; the only social work is a buddy test led by PM 2 and co-designed with Growth, run only if day-180 retention plateaus; and Growth gets a referral invite of its own that shares nothing about anyone's use. | M5 builds the business case for one Module 2 rock. |
| **M5** Business case | ☐ | |

**Open items carried forward:** for M5, the monthly versus annual plan mix, an LTV case against the cost of 14 people for a year, and real baselines for the roadmap's placeholder thresholds; optional, the charter's How We Work part.

## Deliverables at a glance

| # | Deliverable | Module | Status | File |
|---|---|---|---|---|
| 1 | **Product Strategy & OKRs** (Playing to Win + hard no + OKRs + AI pressure-test) | M1 | ✅ | [`01-strategy/strategy-and-okrs.md`](01-strategy/strategy-and-okrs.md) |
| 2 | **Outcome Roadmap & Trade-off Memo** | M2 | ✅ | [`02-roadmap/outcome-roadmap.md`](02-roadmap/outcome-roadmap.md) |
| 3 | **Team Charter** (What We Own + How We Decide) | M3 | ✅ | [`03-team-charter/team-charter.md`](03-team-charter/team-charter.md) |
| 4 | **Stakeholder Message** (a hard no to my Module 3 stakeholder) | M4 | ✅ | [`04-stakeholder-message/stakeholder-message.md`](04-stakeholder-message/stakeholder-message.md) |
| 5 | **Business Case** (bet, assumptions, return + kill criterion) | M5 | ☐ | [`05-business-case/business-case.md`](05-business-case/business-case.md) |
| 6 | **Final Presentation** (the five deliverables + a reflection on the course) | M6 | ☐ | `final-presentation.html`, downloaded from the Final Project Deliverables Builder |

## How to submit

- In Module 6, generate the presentation in the **[Final Project Deliverables Builder](https://product-school-platform.github.io/ps-content-library/certifications/plc/2026.1/Modules/Final%20Project%20Deliverables%20Builder.html)**. It pulls the deliverables from this repo; then I add my reflection and download `final-presentation.html`, and commit it to the root of this repo.
- Submit **both** the **repo URL** and the **presentation** on the Learning Platform within **7 days** of the cohort ending.

## Repo structure

```
product-leadership/
├── README.md                              ← this dashboard: strategy, scenario, thread, status
├── PROMPTS.md                             ← every lab prompt, and how GPT-6 and Claude replied
├── 01-strategy/
│   ├── strategy-and-okrs.md               ← M1: Playing to Win + hard no + OKRs + AI pressure-test   ★ Deliverable 1
│   ├── NOTES.md                           ← M1 ideas, takeaways and lab decisions
│   └── ai-replies/                        ← both models' replies, word for word
├── 02-roadmap/
│   ├── outcome-roadmap.md                 ← M2: trade-off memo + outcome roadmap   ★ Deliverable 2
│   ├── NOTES.md                           ← M2 ideas, takeaways and the scored backlog
│   └── ai-replies/                        ← both models' replies, and the roadmap visual for Module 6
├── 03-team-charter/
│   ├── team-charter.md                    ← M3: What We Own + How We Decide         ★ Deliverable 3
│   ├── NOTES.md                           ← M3 ideas, takeaways and the charter's decisions
│   └── ai-replies/                        ← both models' charter drafts, word for word
├── 04-stakeholder-message/
│   ├── stakeholder-message.md             ← M4: a hard no to my Module 3 stakeholder  ★ Deliverable 4
│   ├── NOTES.md                           ← M4 ideas, takeaways and how the message was written
│   └── ai-replies/                        ← both models' read of the message as the Growth lead
├── 05-business-case/
│   └── business-case.md                   ← M5: bet, assumptions, return + kill criterion  ★ Deliverable 5
└── final-presentation.html                ← M6: the final presentation, from the builder  ★ Deliverable 6
```
