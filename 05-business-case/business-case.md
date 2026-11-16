# Business Case: Fable Growth

> Module 5 · Build the Business Case and the Kill Line

**Rock:** The steady plan and self-check (Rock 1, from backlog #6). The ask: fund a one-quarter concierge test (about $0.6M), and the build only if it passes.

## 1. The strategic bet

> Recovered premium users who still use sleep content keep a nightly wind-down built from what helped them, so more of them are still paying at day 180. Each one kept is about $155 of margin that Fable now loses when the hard stretch ends.

## 2. The assumptions, ranked

1. People who have recovered want an ongoing plan and will keep paying for it (the concierge test's opt-in and paid return).
2. A rules-based steady plan keeps most of the concierge test's lift once it's automated. The hand-built plans set the upper limit, so the concierge group is measured against a matched holdout.
3. About 20,000 monthly-plan deep users reach day 90 each month, so a 20-point lift means about 4,000 more paying at day 180 per cohort (est.; checkable in Fable's data now).

## 3. The expected return

**Per customer:** Each extra monthly-plan user still paying at day 180 is worth about $155 of margin: $12 a month, about $8.40 after app-store fees and running costs, for about 18 months at 6% monthly churn after day 180 (est.).

**Volume target:** 4,000 more monthly-plan users still paying at day 180 in each monthly cohort once the steady plan is at full strength (KR1 from 35% to 55% by month 12): about $7.4M of lifetime margin per year of cohorts against about $2.3M a year for the team of 14 and regulatory and partner costs, or about $0.3M of cash in year one and break-even around month 22 (est.).

## 4. The kill criterion

> By the end of month 3, if fewer than 30% of at least 400 invited users opt in, fewer than 35% of participants use the wind-down three or more nights a week by week 6, fewer than 10% of at least 150 churned participants resume paying at the existing price, or the regulatory opinion doesn't clear self-checks, we stop the steady plan build, keep only the bedtime reminder and load-time fixes, and return about $1.7M of Next and Later budget to the board; any further investment needs a new business case. If the build goes ahead and day-180 retention is below 45% for the first two monthly cohorts to reach day 180 on the steady plan, the same applies to the remaining budget.

## 5. The model behind it

Every input is an estimate, since the scenario gives no price or cohort sizes; the open items list what to replace with Fable's own data before presenting.

| Input | Value |
|---|---|
| Price | $12 a month; about $8.40 left after app-store fees and running costs (70%) |
| Value of each extra user kept to day 180 | About $155: 2 more months to day 180, then about 17 months at 6% monthly churn |
| Monthly-plan deep users reaching day 90 | 20,000 a month |
| Cost | 14 × $160k fully loaded, plus about $75k for the regulatory opinion and signposting partner: about $2.3M a year |

| KR1 lift | Extra users per monthly cohort | Lifetime margin per year of cohorts | Return : cost |
|---|---|---|---|
| 20 points (plan, 35% → 55%) | 4,000 | $7.4M | 3.2x |
| 16 points (20% below plan) | 3,200 | $6.0M | 2.6x |
| 14 points (30% below plan) | 2,800 | $5.2M | 2.3x |
| Break-even: 6 points (KR1 at 41%) | 1,250 | $2.3M | 1.0x |
| 20 points, but churn 10 points a year higher ($126 a user) | 4,000 | $6.0M | 2.6x |

The cash curve assumes steady plan v1 ships at month 6 and reaches its full lift by month 12, with the extra users paying from day 120.

| | Cash margin so far | Break-even against the year's cost |
|---|---|---|
| Base | $0.3M at month 12, $1.4M at month 18, $3.3M at month 24 | Month 22 |
| Costs 20% higher | The same | Month 23 |
| Automation keeps 75% of the lift | $2.5M at month 24 | Month 24 |
| v1 ships at month 9 | $2.3M at month 24 | Month 25 |

The Now quarter puts about $0.6M at risk, and the kill criterion stops spending there if the concierge test fails. Annual-plan users and the free-to-premium path in Later are not counted. Both models' CFO stress-tests, word for word: [2-cfo-stress-test.md](ai-replies/2-cfo-stress-test.md). How it was built: [NOTES.md](NOTES.md).
