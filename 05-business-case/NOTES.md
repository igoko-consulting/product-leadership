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
- **Independent check, our addition:** the Lab Guide's CFO stress-test prompt, run on Case A in both models ([replies](ai-replies/1-cfo-check-case-a.md)). Both would not approve, both reproduce the $950 team cost and a payback of at least 13 months, both find LTV:CAC under 3:1 if churn is 10 points higher, and both score the kill criterion as missing its financial consequence. Claude added an estimated $160k build, which pushes payback to about 40 months, and showed the Q1 date isn't credible. Missed: Claude's chat carried earlier context again, so the clean confirmation comes from GPT-6 alone.
- **Confidence in the verdict, about 85%:** no reading of the numbers gives 4.7 months (it would need 11.2% conversion at $38 per individual); the "fund with a condition" option removes the case's only route from individual to team, so it funds a different case nobody has written; and an independent CFO read on the case's own numbers reached the same verdict. Missed: the remaining doubt is about the idea, not this case. A team plan that individuals choose to buy, with no manager report, might work, but it would be Fable for Teams (#13) and a separate decision.
