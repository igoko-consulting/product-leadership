# Module 5 · 1. CFO check of Case A (our addition)

Replies to the Lab Guide's CFO stress-test prompt, applied to the funding exercise's Case A as an independent check of the verdict ([PROMPTS.md](../../PROMPTS.md#1-cfo-check-of-case-a--our-addition-not-a-lab-guide-step)), run 16 Nov 2026 in new memory-off chats. Words unchanged.

Jump to: [GPT-6](#gpt-6) · [Claude](#claude)

## GPT-6

*[Copied from ChatGPT with its formatting flattened: headings, lists and tables restored here; bold, italics and any formula layout could not be recovered.]*

### CFO Business Case Review: Fable Team & Enterprise Tier

Overall assessment: The commercial opportunity is plausible, but the unit economics are not yet demonstrated. Your biggest problem is that the stated 4.7-month payback cannot be reconciled with your assumptions.

I would challenge four things before allowing this case near the investment committee.

#### 1. Load-bearing assumption: 4% individual-to-team conversion

Finding

Your most important assumption is that 4% of weekly-active individual users will convert into team accounts.

This drives almost the entire business case. You are assuming that individual engagement translates into organisational purchasing intent.

That is a substantial behavioural leap.

Someone completing three AI check-ins a week does not necessarily:

- Have authority to purchase software for their organisation.
- Want to share personal wellbeing information with their manager.
- Believe Fable is appropriate for workplace use.
- Have a manager willing to pay $12 per seat.

The last point is particularly important. Your proposed acquisition mechanism introduces a potential trust problem: users may interpret a personal wellbeing report being shared with their manager as workplace monitoring.

Sensitivity test:

| Conversion | Team accounts | Net new ARR |
|---|---|---|
| 4.0% (base) | 120 | $103,680 |
| 3.2% (-20%) | 96 | $82,944 |
| 3.0% (-25%) | 90 | $77,760 |
| 2.8% (-30%) | 84 | $72,576 |

A 20–30% deterioration in conversion reduces ARR by $20,736–$31,104 per quarter.

Your commercial opportunity becomes considerably less attractive, particularly if acquisition costs remain fixed.

Question you must answer:

Have you demonstrated that individual users will actively introduce Fable to their employers and that employers will purchase it, rather than simply assuming individual engagement creates enterprise demand?

---

#### 2. Per-customer economics: Your payback calculation is wrong or incomplete

Finding

Your $864 per-customer figure is mathematically correct as first-year revenue:

$12 × 6 seats × 12 months = $864.

However, you are confusing revenue per customer with customer lifetime value.

You assume annual churn of 15%.

Using a simplified perpetual subscription model:

LTV = Annual revenue / Annual churn

$864 / 15% = $5,760 revenue LTV per team account.

Now stress-test churn.

| Metric | Base case | Higher churn |
|---|---|---|
| Annual churn | 15% | 25% |
| Revenue LTV | $5,760 | $3,456 |
| Gross margin assumption | 80% | 80% |
| Gross profit LTV | $4,608 | $2,765 |
| CAC per team account | $950 | $950 |
| LTV:CAC | 4.85:1 | 2.91:1 |

I’ve assumed 80% gross margin because you haven’t supplied one. This is illustrative, not verified.

Your LTV:CAC falls below the 3:1 threshold if churn increases by 10 percentage points.

That is a material warning.

There is another problem: your $38 CAC is per individual user, not per converted team account.

At 4% conversion:

$38 / 4% = $950 CAC per team account.

This assumes every one of the 3,000 individual users incurs the $38 acquisition cost.

Your stated 4.7-month payback therefore doesn’t hold under that interpretation.

At six seats per team:

- Monthly revenue: $72.
- Monthly gross profit at 80% margin: $57.60.
- Team CAC: $950.
- Payback: $950 / $57.60 = 16.5 months.

Even using revenue rather than gross profit, payback is 13.2 months.

Other omitted costs include:

- Enterprise onboarding and implementation.
- Customer support.
- Security and privacy compliance.
- Report generation and AI inference.
- Sales and account management.

These could make the economics worse.

Question you must answer:

Is your $38 CAC genuinely the fully loaded acquisition cost of an individual user, and can you demonstrate that the resulting $950 team CAC produces at least a 3:1 gross-profit LTV:CAC ratio?

---

#### 3. Volume target: $103,680 ARR requires meaningful acquisition investment

Finding

Your target is 120 team accounts in Q1, originating from 3,000 weekly-active individual users.

At $38 CAC per individual:

3,000 × $38 = $114,000 acquisition investment.

Your resulting economics:

| Metric | Base case | CAC +20% |
|---|---|---|
| Individual users acquired | 3,000 | 3,000 |
| CAC per individual | $38 | $45.60 |
| Total acquisition cost | $114,000 | $136,800 |
| Team conversions | 120 | 120 |
| Team CAC | $950 | $1,140 |
| New ARR | $103,680 | $103,680 |
| Monthly revenue | $8,640 | $8,640 |
| Revenue payback | 13.2 months | 15.8 months |
| Gross-profit payback (80% margin) | 16.5 months | 19.8 months |

There are two important qualifications.

First, you describe these users as having organically adopted Fable, but use paid-social CAC to calculate acquisition costs.

If the 3,000 users already exist, their acquisition cost may be sunk. If you need to acquire 3,000 additional users, the $114,000 investment is relevant.

You need to distinguish these scenarios.

Second, you have not included the cost of converting individual users into organisational buyers. Someone sharing a report is not necessarily a completed enterprise sale.

At 20% higher CAC, you are approaching a 20-month payback period before allowing for additional enterprise costs.

Would the business still wait that long?

Possibly, but only if retention, expansion and gross margins justify the investment.

I would not approve the volume target without a quarterly acquisition budget, a conversion funnel and an explicit payback ceiling.

Question you must answer:

Are the 3,000 weekly-active users an existing, already-acquired audience or a new acquisition target, and what is the fully loaded budget required to generate 120 paying team accounts by the end of Q1?

---

#### 4. Kill criterion: Incomplete financial protection

Finding

Your current criterion:

“If individual-to-team conversion has not reached 3% by end of Q2, the go-to-market approach will be reassessed before Q3 headcount is committed.”

My score:

| Requirement | Present? | Assessment |
|---|---|---|
| Specific metric | Yes | Individual-to-team conversion |
| Specific number | Yes | 3% |
| Specific timeline | Yes | End of Q2 |
| Specific financial consequence | No | Reassessment doesn’t commit anyone to stopping expenditure |

Score: 3/4.

You have defined when to review performance, but not what happens financially when the initiative fails.

I would rewrite it:

Recommended kill criterion:

“If individual-to-team conversion is below 3% of eligible weekly-active users by the end of Q2, we will stop paid acquisition for the enterprise tier, freeze all uncommitted Q3 enterprise hiring and suspend further GTM investment. Restarting requires a revised business case demonstrating a gross-profit LTV:CAC of at least 3:1 and payback within 18 months.”

This establishes:

- The failure threshold.
- The decision date.
- The financial consequence.
- The conditions for restarting.

It also prevents the team from continuing to spend simply because it has already invested in the initiative.

---

### Final CFO decision

I would not approve this case because the 4.7-month payback is unsupported, the fully loaded team CAC is unclear, and the economics fall below a 3:1 LTV:CAC ratio when annual churn increases by just 10 percentage points.

#### The one thing to fix before presenting

Rebuild the unit economics from individual acquisition through to team subscription.

Show the complete funnel:

Individual acquisition → weekly active users → AI check-in engagement → report sharing → employer interest → team conversion → paid seats → annual retention.

For each stage, show:

- Conversion rate.
- Cost.
- Revenue.
- Gross margin.
- Payback.

Until you can reconcile the $38 individual CAC, $950 team CAC and claimed 4.7-month payback, your headline financial return is not investment-grade.

My advice: Don’t defend the $103,680 ARR figure until you can demonstrate how much it actually costs to generate and retain it.

## Claude

*[Claude Opus 5.5 in claude.ai, pasted as Markdown, so the formatting is Claude's own; its title and section headings are moved down two levels to fit this file. Its verdict refers to "your own roadmap" and to what "you just told Growth", neither of which was in the prompt, so this chat carried earlier context and isn't a clean memory-off read.]*

### CFO stress-test: Team & Enterprise Tier

#### 1. Load-bearing assumption

**Finding: the 4% individual-to-team conversion rate carries the whole case, because acquisition cost per team is 1 ÷ conversion.**

- At 4%, you need 25 individuals for each team that converts. At $38 each, that's **$950 to acquire one team**, not $38.
- At 20–30% lower conversion (2.8–3.2%), that rises to **$1,190–$1,360 per team**. Payback stretches to 21–24 months on an assumed 80% gross margin, and quarterly ARR falls to roughly $73k–$83k.
- I can't reproduce your 4.7-month payback from these inputs. On revenue alone, $950 ÷ $72 a month is 13.2 months.

**Question:** What evidence supports 4%? Specifically, how many users today share anything with a manager, and how many of those teams have bought?

#### 2. Per-customer figure

**Finding: $864 assumes no churn in year one, no seat changes, and revenue rather than margin. LTV:CAC clears 3:1 only at your 15% churn.**

My estimates: 80% gross margin (not in your case), and LTV = annual gross profit ÷ annual churn.

| Annual churn | LTV | LTV:CAC at 4% conversion | LTV:CAC at 3% conversion |
|---|---|---|---|
| 15% (your assumption) | $4,608 | 4.9:1 | 3.6:1 |
| 25% (10 points higher) | $2,765 | **2.9:1** | **2.2:1** |

- **With churn 10 points higher, the case drops below 3:1.** At 25% churn, conversion has to stay above about 4.1% to hold 3:1.
- 15% annual churn is optimistic for six-seat SMB accounts, where losing one buyer loses the whole account.
- If converting users already pay for an individual premium plan, the team seat partly replaces that revenue, so net new revenue is lower than $864.

**Question:** What gross margin per seat and what SMB account churn are you assuming, and what are they based on?

#### 3. Volume target

**Finding: reaching $103,680 of ARR in Q1 costs about 2.6 times what it earns in year one.**

My estimates:

- **Acquisition:** 3,000 active individuals × $38 = **$114,000**, if the pool has to be acquired fresh each quarter.
- **Build:** team billing, seat management, an admin view, the report itself and a privacy review take roughly 4 of your 14 people for a quarter, about **$160,000** (assuming about $160k a year fully loaded per person).
- **Total:** about **$274,000** for $103,680 of ARR.
- **Payback**, on $6,912 a month of gross profit:
  - acquisition only: about 16.5 months
  - including the build: about 40 months
- **With acquisition cost 20% higher:** about 20 months on acquisition only, and about 43 months including the build.
- **The Q1 date also isn't credible.** The report fires at week four, after a tier that doesn't exist yet has been built, so the first conversions can't land until well into the quarter.

A business with flat growth and one board-approved initiative would not wait 20 to 43 months for this.

**Question:** Is the 3,000 an existing base that converts once, or a fresh pool you must acquire every quarter? And which of the 14 people build the tier?

#### 4. Kill criterion

| Element | Score | Why |
|---|---|---|
| Metric | Partial | Conversion of whom, into what, over what period? |
| Number | ✓ (3%) | But 3% only holds 3:1 if churn is 15% |
| Timeline | ✓ (end of Q2) | |
| Financial consequence | ✗ | "Reassessed" is not a consequence |

**Rewrite:**

> If fewer than 3% of individuals who completed three check-ins a week for four weeks buy a team plan of four or more seats within 60 days of their week-four report, measured on cohorts reaching week four by 31 May, or if acquisition cost per converted team exceeds $1,100, we stop the team tier on 30 June. No Q3 headcount is committed, the unspent budget returns to the steady plan, and existing team accounts run to renewal with no new sales.

#### Verdict

**I would not approve this case because the payback is understated by a factor of about three, the unit economics only work under optimistic churn, and the growth mechanism depends on AI check-ins your own roadmap says won't exist this year.**

**The one thing to fix before presenting is the mechanism, not the maths.**

- The case sends a wellbeing report to the user's manager. That is sharing mental-health progress, which is exactly what you just told Growth you won't do because it puts people at risk.
- It also sells to employers, which your strategy rules out until the consumer business proves itself.

The board will spot both contradictions before they get to the numbers. Either recast this as the Later employer bet, gated on outcome evidence, or remove the manager report and rebuild the case around a team plan the individual chooses to buy.
