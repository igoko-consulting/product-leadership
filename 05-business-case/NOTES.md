# Module 5 notes: Build the Business Case and the Kill Line

Session 5, 16 Nov 2026. Sources: Module 5 slides and Lab Guide. Builds on: [Module 2's rocks](../02-roadmap/outcome-roadmap.md). Output: [business-case.md](business-case.md).

## Labs

### Funding decision (practice) · Case A: Fable team tier

The Lab Guide's case: a $12-a-seat team tier for small businesses, fed by individual users who complete three AI check-ins a week and are prompted to share a week-four "productivity and wellbeing report" with their manager. It assumes 4% individual-to-team conversion, 6 seats, 15% annual churn and $38 CAC per individual, and claims $103,680 of new ARR in Q1 and a 4.7-month payback.

| Conversion | Teams per quarter | ARR | CAC per team | Payback | LTV:CAC at 15% churn | at 25% churn |
|---|---|---|---|---|---|---|
| 4% (plan) | 120 | $103,680 | $950 | 13.2 months | 6.1 | 3.6 |
| 3.2% (20% off) | 96 | $82,944 | $1,188 | 16.5 months | 4.9 | 2.9 |
| 2.8% (30% off) | 84 | $72,576 | $1,357 | 18.8 months | 4.2 | 2.5 |

- **The assumption doing the most work:** 4% conversion, because it sets both the revenue and the real cost of a team ($38 per individual ÷ 4% = $950 per converting team). At 20 to 30% below plan, payback runs to 16 to 19 months, and with churn 10 points higher LTV:CAC falls below 3:1. Missed: team size is a close second; 4.2 seats instead of 6 also gives an 18.8-month payback.
- **What doesn't add up:** the 4.7-month payback needs a CAC of about $338 per team, not $950; the CAC comes from paid social while the users are said to have adopted Fable organically; 4% of a fixed 3,000 converts once, not every quarter; and the conversion mechanism sends wellbeing data to people's managers, which breaks the trust Fable is known for and is likely special-category data under GDPR. Missed: the privacy problem would cut the conversion rate before the maths does, since people stop answering check-ins honestly.
- **The kill criterion:** it has a metric (conversion), a threshold (3%, a quarter below plan) and a deadline (end of Q2), but no financial consequence: "reassessed before Q3 headcount" hands the decision back to the room. A complete version: below 3% by the end of Q2, the team-tier build stops and its Q3 budget and engineers return to the core app.
- **My verdict, don't fund:** the payback is 13 months, not 4.7, on an untested 4% conversion that relies on sending people's wellbeing reports to their managers. Missed: in my own strategy "Fable for Teams" (#13) was the alternative hard no and employers sit outside Where to play; this fixed case shows from the other side why that call holds.
