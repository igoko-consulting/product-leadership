# Module 5 · 2. CFO stress-test of my business case

Replies to the Lab Guide's CFO prompt in [PROMPTS.md](../../PROMPTS.md#2-cfo-stress-test-of-my-business-case--new-memory-off-chats-in-both-models), run 16 Nov 2026 in new memory-off chats. Words unchanged.

Jump to: [GPT-6](#gpt-6) · [Claude](#claude)

## GPT-6

*[Copied from ChatGPT with its formatting flattened: headings, lists and tables restored here; bold, italics and formula layout could not be recovered.]*

### CFO Review: Fable Steady Plan & Self-Check

Overall assessment: This is a considerably stronger business case. You are asking for a limited investment to validate demand before committing to a full build, and you have connected retention improvements to incremental contribution margin.

However, there are three financial weaknesses: your $150 per-customer figure needs a clearer churn assumption, your $7.5M annual return appears to mix different time horizons, and your month-12 volume target may not allow enough time for day-180 measurement.

#### 1. Load-bearing assumption: A 20-percentage-point retention improvement

Finding

Your most important assumption is that a personalised steady plan can improve day-180 retention from 35% to 55%.

This is the assumption that makes the investment attractive.

Your calculation is:

- 20,000 monthly-plan deep users reach day 90 each month.
- A 20-percentage-point retention improvement produces 4,000 additional paying users per monthly cohort.
- Each retained customer contributes approximately $150 in margin.
- Incremental margin per monthly cohort: $600,000.

But consider what happens if the improvement is 20–30% smaller.

| Retention improvement | Additional retained users | Margin per cohort |
|---|---|---|
| 20 points (base) | 4,000 | $600,000 |
| 16 points (-20%) | 3,200 | $480,000 |
| 15 points (-25%) | 3,000 | $450,000 |
| 14 points (-30%) | 2,800 | $420,000 |

The opportunity remains attractive, but the economics deteriorate.

There is another critical assumption: your concierge experiment must demonstrate that the hand-built experience can be replicated through a rules-based product.

If concierge participants receive unusually high attention, their retention improvement might not survive automation.

Question you must answer:

Can you demonstrate that the concierge experience produces a meaningful retention improvement that survives automation, rather than simply proving that a highly personalised, human-supported service works?

---

#### 2. Per-customer economics: Your $150 figure needs a churn sensitivity

Finding

You state that each additional monthly-plan subscriber retained at day 180 generates approximately $150 in margin over the following 18 months.

Your $150 figure implies an average of:

$150 / $12 = 12.5 paid months over the next 18 months.

In other words, you are implicitly assuming that customers generate 12.5 months of contribution margin before churning.

That is an important assumption.

Using a simplified monthly survival model:

| Metric | Base case | Higher churn |
|---|---|---|
| Monthly churn | 2.65% | 3.55% |
| Annualised churn | 27.5% | 35.2% |
| Expected paid months over 18 months | 12.5 | 11.0 |
| Contribution margin per customer | $150 | $132 |
| Margin reduction | - | 12% |

I’ve estimated monthly churn mathematically to reproduce your $150 figure, assuming $12 monthly contribution and constant monthly churn. Actual churn may behave differently.

Does LTV:CAC remain above 3:1?

You haven’t supplied a CAC because this is a retention initiative rather than an acquisition initiative.

However, we can calculate an equivalent investment cost per incremental retained customer.

Assuming the full $2.2M annual team cost is attributable to generating 48,000 additional retained customers across 12 monthly cohorts:

$2.2M / 48,000 = $45.83 per incremental retained customer.

Illustrative LTV:CAC:

| Metric | Base case | Higher churn |
|---|---|---|
| Customer margin | $150 | $132 |
| Equivalent cost per retained customer | $45.83 | $45.83 |
| LTV:CAC | 3.27:1 | 2.88:1 |

This is an illustrative allocation, not a conventional acquisition CAC calculation. It assumes all 12 cohorts mature and the entire team cost is attributable to those retained customers.

The important finding: At 10 percentage points higher annual churn, your economics could fall below the 3:1 benchmark.

Also, your $12 figure needs to be confirmed as contribution margin after app-store fees, infrastructure, AI inference and other variable costs, rather than simply revenue after app-store fees.

Question you must answer:

What historical monthly churn supports the $150 figure, and does the initiative still generate at least a 3:1 return after variable servicing costs and a 10-percentage-point increase in annual churn?

---

#### 3. Volume target: Your $7.5M return needs reconciling

Finding

Your volume target is 4,000 additional paying subscribers per monthly cohort.

Your calculation appears to be:

4,000 × $150 × 12 = $7.2M.

That’s approximately your stated $7.5M.

But there is a problem.

You are multiplying an 18-month customer margin figure by 12 monthly cohorts and calling the result annual margin.

Those are not necessarily equivalent.

Let’s distinguish three different figures.

| Measure | Calculation | Result |
|---|---|---|
| Margin per monthly cohort | 4,000 × $150 | $600,000 |
| Aggregate margin across 12 cohorts | $600,000 × 12 | $7.2M |
| Annualised margin at steady state | 48,000 × $12 × 12 | $6.912M |

The $7.2M represents the aggregate 18-month margin contribution from 12 monthly cohorts, assuming each generates the full $150.

The $6.912M represents an illustrative annualised run rate at 48,000 additional active subscribers, assuming each continues generating $12 monthly.

Neither figure is automatically the realised annual margin during year one.

There is also a timing problem.

Your users reach day 90 each month, but your primary KPI measures retention at day 180.

That means you need another 90 days to observe the result.

If you start the programme in month one, you cannot have 12 fully matured monthly cohorts by month 12.

You need to account for that measurement lag.

What does it cost?

Your stated annual team cost is $2.2M.

Assuming a relatively even allocation:

| Period | Estimated team cost |
|---|---|
| One quarter | $550,000 |
| Six months | $1.1M |
| Twelve months | $2.2M |

These figures assume the $2.2M is fully loaded and spread evenly across the year.

At steady state, using your 48,000 additional subscribers:

- Annualised contribution margin: $6.912M.
- Annual team cost: $2.2M.
- Annualised surplus: $4.712M.
- Margin return on team investment: approximately 3.14x.

This is attractive, provided the assumptions hold.

What if costs increase by 20%?

Your annual investment becomes:

$2.2M × 1.20 = $2.64M.

The annualised surplus falls to $4.272M.

The economics still look attractive at steady state.

However, the real question is whether the board is willing to fund the programme for long enough to realise those returns.

Question you must answer:

Can you provide a month-by-month cash and contribution-margin forecast showing when cohorts reach day 180, when incremental retention becomes measurable, and when cumulative contribution margin exceeds the $2.2M investment (or $2.64M under cost stress)?

---

#### 4. Kill criterion: Strong, but needs one financial clarification

Finding

Your kill criterion is substantially better than the original enterprise case.

| Requirement | Present? | Assessment |
|---|---|---|
| Specific metric | Yes | Wind-down usage and paid return |
| Specific number | Yes | 35% and 10% |
| Specific timeline | Yes | End of month 3 |
| Specific financial consequence | Yes | Stop build and return unspent budget |

Score: 4/4.

I particularly like that you have three independent failure conditions:

1. Insufficient engagement.
2. Insufficient willingness to pay.
3. Regulatory clearance not obtained.

Any one of these can stop further investment.

That is good capital discipline.

However, I would tighten the financial consequence.

You say:

“Return the unspent initiative budget for Next and Later to the board.”

I would make clear that the remaining budget cannot be quietly redirected into another version of the same initiative.

Recommended wording

“If, by the end of month 3, fewer than 35% of concierge participants use the wind-down at least three nights a week by week 6, fewer than 10% of churned participants resume a paid subscription at the existing price, or the regulatory opinion does not clear the proposed self-checks, we stop the steady-plan build. Only the already-approved bedtime reminder and load-time fixes continue; all uncommitted initiative funding for subsequent phases is returned to the board, and any further investment requires a new business case.”

One additional CFO recommendation: specify minimum sample sizes for both concierge engagement and paid return. Otherwise, a small number of participants could produce misleading percentages.

Question you must answer:

How many participants must complete the concierge experiment for the 35% engagement and 10% paid-return thresholds to provide sufficiently reliable evidence for an investment decision?

---

### Final CFO decision

I would approve the one-quarter concierge test, but not yet the full build, because the strategic opportunity is attractive, the validation gates are sensible and the potential returns justify testing, but the lifetime margin and annual return calculations need reconciliation before further capital is committed.

#### The one thing to fix before presenting

Reconcile your financial model around the $150 per-customer margin and the 12-month cohort volume calculation.

Specifically, show:

1. The churn assumption underlying $150.
2. The margin contribution under 10 percentage points higher churn.
3. The number of cohorts that actually reach day 180 by month 12.
4. The cumulative investment versus realised incremental contribution margin.
5. The break-even month.

Your business case has the right investment philosophy: fund the evidence first, fund the product second.

Don’t weaken that good strategic decision with financial numbers that a board member can dismantle in five minutes.

## Claude

*[Claude Opus 5.5 in claude.ai, in a new incognito chat, pasted as Markdown, so the formatting is Claude's own; its title and section headings are moved down two levels to fit this file.]*

### CFO stress-test: steady plan and self-check

**Overall:** this case is much stronger than the team tier. It is cheap to test, the kill rule is real, and it builds on users Fable already has. The weak points are how the return is timed and labelled.

#### 1. Load-bearing assumption

**Finding: the 20-point lift surviving automation (your assumption 2) carries the case.**

- The hand-built concierge plans set the ceiling. If the automated plan keeps 70–80% of that lift, you get 14–16 points, not 20.
- That means 2,800–3,200 extra users per cohort, not 4,000. Margin falls to about $5.0–5.8M against $2.2M of cost.
- The case still pays back, but two things break:
  - **LTV:CAC drops to 2.3–2.6:1.** The cost per retained user rises from $46 to $57–65.
  - **Break-even slips** from about month 27 to months 31–33.
- **The planning point:** to deliver 20 points once automated, the concierge test probably needs to show about 25–29.

**Question:** What lift does the concierge test have to show, measured against a holdout group, for you to fund the build?

#### 2. Per-customer figure

**Finding: $150 over 18 months implies about 4.5% monthly churn (about 42% a year).**

- $12 × 18 months would be $216 if nobody left. $150 is about 12.5 paid months on average.
- There's no acquisition cost here, so I've treated the programme cost per retained user as the CAC: $2.2M ÷ 48,000 retained users a year = **about $46**.

| Scenario | Value per retained user | LTV:CAC |
|---|---|---|
| Your case (about 42% annual churn) | $150 | 3.3:1 |
| Churn 10 points higher (about 52% annual, 6% monthly) | $134 | **2.9:1** |
| Programme cost 20% higher | $150 | 2.7:1 |

- **With churn 10 points higher, it drops just below 3:1.** The case still pays back, but it no longer clears the standard bar.
- **Unclear wording:** "$12 a month, after app-store fees" could mean $12 is the price, or $12 is what's left after fees. App-store fees take 15–30%, so if $12 is the price, net value per user falls to about $105–128.

**Question:** Is $12 the price or the net figure, and how fast do deep users who make it past day 180 actually churn today?

#### 3. Volume target

**Finding: "$7.5M of margin a year" is the margin each year's cohorts earn over their 18 months of life. It is not cash earned within the year.**

- **Arithmetic check:** 4,000 × 12 cohorts × $150 = **$7.2M**, not $7.5M.
- **Cost to reach the target by month 12:** about $2.2M for the team, plus regulatory and partner costs. I estimate those at $50–100k; they aren't in your case.
- **My cash model.** It assumes v1 ships at month 6, the lift ramps to full by month 12, extra users start paying about three months after day 90, and churn is 4.5% a month.

| Month | Cash margin earned so far | Net position after team cost |
|---|---|---|
| 12 | about $0.1M | −$2.1M |
| 18 | about $1.1M | −$2.2M |
| 24 | about $3.5M | −$0.9M |
| **Break-even** | | **month 27** |

- **With costs 20% higher, break-even moves to about month 30.**
- **Would the business wait that long? Probably yes.** The 14 people are already on the payroll, and the alternative is continued churn. But that only holds if you present it as a break-even in two and a half years, not "$7.5M a year". A board that hears $7.5M expects it in year one.

**Question:** Can you show a month-by-month cash curve? And is the $2.2M extra spending, or the cost of a team Fable would pay for anyway?

#### 4. Kill criterion

| Element | Score |
|---|---|
| Metric | ✓ Three metrics: nights a week, paid return, regulatory clearance |
| Number | ✓ 35% and 10% |
| Timeline | ✓ Week 6, end of month 3 |
| Financial consequence | ✓ Stop the build and return the unspent budget |

**All four elements are present.** Three gaps remain:

- **No sample size.** If 30 churned people take part, "10% resume paying" means three people.
- **The 30% opt-in threshold from your roadmap is missing.**
- **The build stage has no kill rule.** You're asking for build money "only if it passes", but nothing stops the build if automation loses the lift.

**Tightened version:**

> By the end of month 3, if fewer than 30% of at least 400 invited users opt in, fewer than 35% of participants use the wind-down three or more nights a week by week 6, fewer than 10% of at least 150 churned participants resume paying at the existing price, or the regulatory opinion doesn't clear self-checks, we stop the steady plan build, keep only the reminder and load-time fixes, and return about $1.65M of Next and Later budget to the board. If the build goes ahead and day-180 retention for the monthly cohort is below 45% by month 6, the same consequence applies to the remaining budget.

#### Verdict

**I would approve the one-quarter concierge test (about $550k) but not yet the build, because the test is cheap, the kill rule is real and the upside is large, but the return is presented as annual cash when it is lifetime margin that breaks even around month 27.**

**The one thing to fix before presenting:** replace "$7.5M a year" with the cash curve: about $0.1M in year one, break-even around month 27, and $7.2M of lifetime margin per year of cohorts once the lift is at full strength. Correct the $7.2M figure at the same time. That one change makes the case believable, and every other gap above is a question you can answer in the room.
