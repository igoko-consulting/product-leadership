# Module 5 notes: Build the Business Case and the Kill Line

Session 5, 16 Nov 2026. Sources: Module 5 slides and Lab Guide. Builds on: [Module 2's rocks](../02-roadmap/outcome-roadmap.md). Output: [business-case.md](business-case.md).

## Why the stakes change: speaking finance

| P&L line | What moves it |
|---|---|
| Revenue | Pricing, retention, churn, tier changes and new ways to charge |
| COGS | The variable cost of delivering the product: infrastructure, support, build-or-buy |
| Gross margin | Revenue minus COGS: does each sale make money before team costs? |
| Operating expenses | Headcount and team overhead; the line that moves when you ask for people |
| Operating income | What's left after every cost; where a strategic bet is judged |

- **AARRR tells you where users drop off, not whether the work is worth funding:** acquisition, activation, retention, revenue and referral are product signals; finance reads the P&L. Missed: Fable's strategy works almost entirely on retention, and Module 4 handed referral to Growth, so the case has one AARRR stage to translate rather than five.
- **Bridge the result to money and timing:** "this will improve retention" is a hypothesis to finance; "a 5-point lift adds this much ARR per cohort, because…" is a case, and "you'll see the first signal by week 6 and payback by month N" answers when. Missed: the steady plan's first signal (nightly use in the concierge test) arrives in weeks, but its money arrives in year two, which is why the cash curve had to be in the case.

## The financial toolkit

- **LTV is the ceiling, CAC is the floor:** LTV is what a customer brings in over the relationship, and retention is its riskiest input because small changes compound; CAC is the fully loaded cost to win one, usually understated because it leaves out sales overhead, onboarding and support. Missed: a retention bet has no CAC, so the programme cost per retained user stood in for it in both CFO reads. Whether the team of 14 counts as new spending or as a team Fable pays for anyway decides how good that ratio looks.

| LTV:CAC | Reading |
|---|---|
| Below 1:1 | Burning runway: every customer loses money |
| 3:1 | Sustainable: the usual healthy target |
| Above 5:1 | Room to accelerate spending on growth |

- **Payback and contribution margin:** payback is how long until the investment in a customer pays for itself; the longer it runs, the more committed the business is before it knows. Contribution margin is what each customer earns before fixed costs. Missed: Fable's case clears 3:1 only at its assumed churn, and its payback is about 22 months, so its strongest financial argument is the kill line, not the ratio.
- **Four questions before approving a model you didn't build:** which assumption, 30% off, most changes the outcome; what the retention curve looks like, and LTV with churn 10 points higher; payback with acquisition costs 20% higher; and what the kill criteria are. Missed: these four are the Lab Guide's CFO prompt. Running the prompt on Case A and on my own case was the same discipline applied twice, and it caught the same kind of error both times: a return presented in the wrong time frame.
- **Trace a decision forward and back:** forward from a product change to the line it moves (reduce onboarding friction, retention improves, LTV extends, payback shortens); backward from a line that moved to the product cause (NRR below 100%: which behaviour changed?). Missed: AI personalisation adds inference cost to COGS every month it runs, so "rules-based first, AI only once v1 lifts retention" protects gross margin as well as build risk.

## Building and defending the bet

- **Four costs a model leaves out:** the ceiling (a bet can pay for itself and still be too small to matter), people beyond engineering (implementation, customer success and support absorb the work), opportunity cost (every team on this bet is off another, usually someone's goal) and time to value (how long the business waits without knowing). Missed: for Fable, the concierge test's hand-built plans land on the content team, the opportunity cost is the onboarding redesign and the Apple Watch work, and the time to value is month 22, so all four belong in the room, not only the engineering estimate.

| Kill criterion | Metric | Threshold | Deadline | Consequence |
|---|---|---|---|---|
| "We will reassess if the numbers are not where we need them by Q3" | ✕ | ✕ | ✓ | ✕ |
| "If 90-day retention hasn't reached 28% by end of Q3, we will discuss next steps" | ✓ | ✓ | ✓ | ✕ |
| "…we stop funding the initiative and reallocate the Q4 headcount before it is committed" | ✓ | ✓ | ✓ | ✓ |

- **Agree the number that ends the bet before the work starts:** a vague criterion leaves the decision open just when the team is most invested. Missed: the course's own Cursor example ends with "the go-to-market approach changes before Q3 headcount is committed", which by the slide's own test has no consequence, and Case A copied that shape.
- **The four parts of a one-page case:** the strategic bet (how the product decision leads to a financial result, not a strategy summary), the assumptions ranked by how much each would change the conclusion, the expected return as a per-customer figure for finance and a volume target for the board, and the kill criterion. Missed: the template has no line for the ask, so the bottom-line-up-front rule from Module 4 has to ride in the Rock line.

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

### Business case one-pager

- **The rock and the ask:** Rock 1, the steady plan and self-check. The ask sits in the Rock line, so the first thing read is the decision: fund a one-quarter concierge test, and the build only if it passes, as Module 4's bottom-line-up-front rule asks. Missed: the template puts "Rock" first rather than "Ask", so the ask rides in a field meant for a name.
- **The model:** every input is an estimate ($12 a month, about $8.40 left after app-store fees and running costs, 6% monthly churn after day 180, 20,000 monthly-plan deep users reaching day 90 each month, $160k a head for the team of 14, about $75k for the regulatory opinion and partner). At the planned 20-point KR1 lift a year of cohorts earns about $7.4M of lifetime margin, 3.2 times its cost; it breaks even at a 6-point lift, KR1 at 41%. Missed: it clears 3:1 only at the full lift and at the assumed churn; a 20% shortfall or churn 10 points a year higher both drop it to 2.6x.
- **The assumptions, riskiest first:** demand after recovery, then whether an automated plan keeps the concierge test's lift, then the cohort size, which is the one checkable in Fable's data today. Missed: if the automated plan keeps 70% of the concierge lift, the return falls to about 2.3x, so assumption 2 is where the case is most exposed.
- **The kill criterion:** the same four conditions as Now Bet 1's stop rule, so the roadmap and the case can't disagree, with the unspent budget for Next and Later going back to the board. About $560k, one quarter's cost, is what's at risk. Missed: four conditions are harder to enforce than one; paid return alone was the simpler alternative.
- **CFO stress-test, in both models:** run in new memory-off chats ([replies](ai-replies/2-cfo-stress-test.md)). Both would fund the one-quarter concierge test and not yet the build, which is exactly the case's ask. Both said "$7.5M a year" was lifetime margin presented as annual cash, that "$12 after app-store fees" was ambiguous, and that churn 10 points higher drops the return below 3:1. Claude caught that the kill criterion had left out Now Bet 1's 30% opt-in, and an arithmetic slip ($7.2M, not $7.5M). Missed: both models' fixes rested on their own cash models, which disagreed (month 27 against my month 22), so the curve in the case is my own, with its assumptions stated.
- **What changed:** the ask names its cost (about $0.6M); the per-customer figure states price, net and churn; the return is lifetime margin per year of cohorts plus a cash curve (about $0.3M in year one, break-even around month 22, month 25 at worst); the kill criterion gained the 30% opt-in, sample sizes, a dollar figure returned to the board, a new-business-case rule and a build-stage line; and assumption 2 measures the concierge group against a matched holdout. The roadmap's Next signal and Bet 1 signal changed to match. Missed: the 2.6x at higher churn stays in the case on purpose, because the answer is Fable's own churn data, not a better-looking number.
- **Aligned before Module 6:** the charter no longer lets the product lead override a kill criterion, since a kill line the person who benefits can lift isn't one; the roadmap's Bet 1 now carries the matched holdout and the case's consequence; KR3's mid-point uses cohort timing; "by month 12" is defined as cohorts reaching day 90 by month 12, read by month 15; and shared-service time is named as uncounted. Missed: tightening the kill line in Module 5 quietly broke the charter written in Module 3, which only a read across all five modules found.
- **Fixed after the Module 6 board review:** both models read the per-customer line as 18 months after day 180 and got about $140, so it now says what Section 5 already did: about 2 more months to day 180, then about 17 at 6% monthly churn, about $155. The kill criterion invites at least 500 churned and 400 current users, so 150 churned participants follows from a 30% opt-in, and adds a 15-point gap over the matched holdout; assumption 2 now carries the 2.3x at 70% of the lift into the presentation, since the builder doesn't pull Section 5. Replies: [board review](../06-final-presentation/ai-replies/2-board-review.md). Missed: 15 people paying again is still a thin signal, so the build-stage line, day-180 retention of 45% for the first two cohorts on v1, stays the real proof.
- **Fixed after the second board review:** the build-stage line now says why 45%: 10 points of lift returns about 1.6x, against break-even at 41%, so it reads as the point where the case stops paying rather than a soft target; and the holdout also gets the reminder and load-time fixes, so the $7.4M rests on the steady plan's own lift. Replies: [second review](../06-final-presentation/ai-replies/3-board-review-revised.md). Missed: GPT-6 still wanted the assumptions shown to be credible on their own, which only Fable's churn and cohort data can do.
- **The debrief question, what became clearer once it had a number:** the value of the kill line is in money not spent. The test puts about $0.6M at risk to protect about $1.7M, which is a stronger argument to a board than a 3.2x return that rests on estimated churn. Missed: that argument only holds if the stop rule is enforced, so the charter now says only a new business case to the board can lift it, not the product lead.
