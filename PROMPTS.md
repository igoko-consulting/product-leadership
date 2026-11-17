# Prompts

Every lab prompt I ran, word for word. Each one went to GPT-6 and Claude in chats that use no memory or project instructions (ChatGPT's Temporary Chat, Claude's incognito chat), identical in both, so the replies can be compared. Follow-up prompts ran in the same chat as the prompt before them.

- **Why two models:** it's how I work in practice. A second model is a cheap second reviewer: where both agree, the point carries more weight; where they differ, I look harder before deciding. Missed: two models reading the same prompt aren't fully independent, so agreement is a signal, not proof.
- **Evidence:** every reply is kept word for word in each module's `ai-replies/` folder, linked under each step, so each comparison below can be checked against its source.

---

## Module 1 · Product strategy and OKRs

### 1. Pressure test

```text
You are a skeptical Chief Strategy Officer reviewing a product strategy draft. Your job is to find where the strategy is soft, vague, or likely to fail, not to validate it.
Here is the context:
Imagine you are a Product Leader at Fable, a mental-wellness app for adults aged 25 to 45. Fable grew quickly on a simple, calming experience of guided meditations, sleep stories, and breathing exercises. At its peak it had 4.2 million active users and a strong reputation as the app that actually helped, the one people reached for during a hard stretch.
Growth has now flatlined, and the churn analysis shows a counterintuitive cause: the product works too well for its original job. Users who engage deeply, usually during a period of high stress, resolve that acute need within 90 to 120 days and quietly stop opening the app. There is no compelling next step to keep them. Meanwhile well-funded incumbents like Headspace and Calm dominate brand awareness, and a wave of AI-powered mental-health apps is targeting Fable's core users with more personalized experiences. Fable's own data shows its most engaged users, the ones most likely to pay for premium, are also the most likely to leave once the acute phase passes.
The board has approved budget for one major initiative, and there is real internal disagreement about direction: the clinical team wants structured programs built on cognitive behavioral therapy, the growth team wants a community and social layer, and the content team believes the answer is simply more content. No one has resolved which bet to make or who the product is really for now.
Your challenge. Fable faces a retention crisis created by its own success: it resolves acute distress so quickly and gently that users stop feeling they need it. You have to define what Fable becomes for people after the acute phase and build a durable engagement model that keeps high-value users invested beyond their first 90 days.
Your hard constraints:

* Fable cannot reposition as a clinical mental-health platform, for regulatory and liability reasons.
* The core meditation and sleep content stays the foundation and cannot be replaced.
* Your competition for the post-acute user is the user deciding they no longer need Fable at all.
* You have a cross-functional team of 14 across product, design, engineering, content, and clinical advisory.
* Any solution works within the existing freemium and premium subscription model.

Your goal: Lead the Fable Growth initiative and build a specific, opinionated, board-ready case for where Fable should play, how it can win, and what it will take to get there.
Here is the strategy:
Winning Aspiration: When the hard stretch passes, people keep Fable as how they stay steady, because it knows what helped them and notices early when they're slipping.
Where to Play: Adults 25–45 who used Fable heavily through a stressful stretch, at the point their need eases (about day 60–120), reached inside the app, premium users first. Out: competing with Headspace and Calm for new users, selling to employers, and anyone needing clinical care, whom we signpost elsewhere.
How to Win: Fable is the only app that saw what actually helped each person through their hardest stretch. We turn that history into a personal steady plan and AI check-ins that spot an early dip. Headspace, Calm and the new AI apps start from zero with this user.
Capabilities Required: Personalisation built in-house from each user's session and check-in history, because that history is the advantage. Steady plans that re-sequence the existing meditation and sleep library rather than adding new content. Non-clinical check-ins designed with the clinical advisers, with a partner to signpost care. Consent and privacy fit for sensitive wellbeing data.
Management Systems: Day-180 premium retention for users who engaged deeply in their first 90 days, reviewed monthly by cohort. Weekly active use from day 90 to 180. Notification opt-outs as a guardrail. A monthly clinical-safety review. A quarterly board review against the OKRs.
Hard no: We will not build a community and social layer (no posting between users, groups or profiles), because it serves a different job from staying steady, brings moderation and safety risk with users at vulnerable moments, and would split a team of 14 before the post-acute bet is proven.
Objective: Make Fable the app people keep after the hard stretch passes.
KR1: Premium users who engaged deeply in their first 90 days who are still subscribed at day 180: 35% → 55%.
KR2: Those users still using Fable at least weekly from day 90 to 180: 20% → 45%.
KR3: Users whose check-in shows an early dip and who come back to a session within 48 hours: 25% → 60%.
Please do the following:
1. Identify the single biggest assumption I am making that could be wrong.
2. Ask me the one question a board member would ask that I cannot yet answer.
3. Tell me if any of my KRs are actually outputs disguised as outcomes.
4. Point out one thing I said I would not do and make the case for why I should reconsider.
5. In one sentence: is this a strategy or a wish list? Why?
```

**How the two replies compared** · both replies, word for word: [1-pressure-test.md](01-strategy/ai-replies/1-pressure-test.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Biggest assumption | Recovered users want an ongoing relationship with Fable, and will pay for it | The same: people who feel fine rarely pay to prevent a problem, so the churn may be the job finishing well; the moat is second |
| Board question | What evidence shows users value their history enough to keep paying? | If a check-in detects slipping, how is that not clinical monitoring, and who is liable when it misses someone? |
| Outputs as outcomes | KR3 a proxy that could rise while the product gets worse; KR2 a supporting indicator; KR1 genuine | KR3 an output with no possible baseline; KR2 half output; KR1 may be annual-plan inertia |
| Missing measure | Users saying Fable helps them stay well without feeling dependent on it | Self-reported steadiness at day 180, or fewer users dropping back into acute-level use |
| The hard no | Keep community out of the first investment, but test light social accountability | One buddy mechanic as a gated experiment; shared streaks, gifting and anonymous presence carry little moderation risk |
| Strategy or wish list | A strategy in customer and positioning, partly a wish list in execution | A strategy built around a wish: unproven demand, a thin moat, a check-in that may breach the clinical constraint |

- **They agreed on the biggest assumption:** that recovered users want, and will pay for, an ongoing relationship. It's the one I'd flagged myself.
- **Claude found the sharpest risk:** detecting that someone is slipping may make the check-in a medical device in the UK and EU, which would put How to Win against the first constraint. GPT-6 didn't raise it.
- **Both pushed on the hard no, but not on its core:** neither argued for posting, groups or profiles. Both wanted one light, tested social mechanic instead of the community layer the growth team asked for.

### 2. Harsher follow-up · same chat as each pressure test

```text
Now be harsher. What would a competitor’s strategy team say about this plan?
```

**How the two replies compared** · both replies, word for word: [2-harsher-follow-up.md](01-strategy/ai-replies/2-harsher-follow-up.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | Not worried yet: plausible but replicable, for an uncertain audience | A well-written retreat: target the day-90 users and wait for the board to lose patience |
| The moat | Consumption history a competitor learns within 30 days | 90 days of play logs, rebuilt with a three-question onboarding; GDPR portability lets users take it |
| The segment | Defined by declining interest; people who want to maintain wellbeing may be a different segment | A cohort that leaves by design: slowing a leak, not growing |
| An everyday reason to open | Nothing makes Fable worth opening on an ordinary Tuesday | Noticing a dip is occasional; competitors own sleep as a nightly habit |
| Check-ins and KRs | Intrusive, with false positives; the KRs measure use, not value | Notification creep: KR2 and KR3 reward nudging; legal will water dip detection down to a mood tracker |
| What would build a moat | Change the question: an everyday role people choose even when nothing is wrong | Measurable relapse prevention, and people to stay for (buddies, shared streaks) |

- **They agreed on the gap that matters:** nothing gives a recovered user a reason to open Fable on an ordinary day, and "we saw what helped" is easier to rebuild than I claimed.
- **Claude was more useful on the fix:** sleep as the nightly habit Fable already has the content for, outcome evidence as the moat that takes years to copy, and social ties with people users already know, which tests the hard no.
- **Both read the lack of acquisition as retreat:** the brief points the one initiative at keeping high-value users past day 90, so that criticism is aimed at the brief as much as the plan.

---

## Module 2 · Outcome roadmap

### 1. Roadmap

```text
You are an experienced product leader helping me build a Now/Next/Later roadmap for my product initiative. Generate a roadmap that is outcome-based, not feature-based. Every item in the Now column must be framed as a strategic bet, not a delivery milestone.
Here is my context:
Scenario: Imagine you are a Product Leader at Fable, a mental-wellness app for adults aged 25 to 45. Fable grew quickly on a simple, calming experience of guided meditations, sleep stories, and breathing exercises. At its peak it had 4.2 million active users and a strong reputation as the app that actually helped, the one people reached for during a hard stretch.
Growth has now flatlined, and the churn analysis shows a counterintuitive cause: the product works too well for its original job. Users who engage deeply, usually during a period of high stress, resolve that acute need within 90 to 120 days and quietly stop opening the app. There is no compelling next step to keep them. Meanwhile well-funded incumbents like Headspace and Calm dominate brand awareness, and a wave of AI-powered mental-health apps is targeting Fable's core users with more personalized experiences. Fable's own data shows its most engaged users, the ones most likely to pay for premium, are also the most likely to leave once the acute phase passes.
The board has approved budget for one major initiative, and there is real internal disagreement about direction: the clinical team wants structured programs built on cognitive behavioral therapy, the growth team wants a community and social layer, and the content team believes the answer is simply more content. No one has resolved which bet to make or who the product is really for now.
Your challenge. Fable faces a retention crisis created by its own success: it resolves acute distress so quickly and gently that users stop feeling they need it. You have to define what Fable becomes for people after the acute phase and build a durable engagement model that keeps high-value users invested beyond their first 90 days.
Your hard constraints:

* Fable cannot reposition as a clinical mental-health platform, for regulatory and liability reasons.
* The core meditation and sleep content stays the foundation and cannot be replaced.
* Your competition for the post-acute user is the user deciding they no longer need Fable at all.
* You have a cross-functional team of 14 across product, design, engineering, content, and clinical advisory.
* Any solution works within the existing freemium and premium subscription model.

Your goal: Lead the Fable Growth initiative and build a specific, opinionated, board-ready case for where Fable should play, how it can win, and what it will take to get there.
My strategy (Playing to Win):
Winning Aspiration: When the hard stretch passes, people keep Fable to hold on to the progress they made, sleeping well and staying steady, because it knows what helped them and has it ready the moment they feel things slipping.
Where to Play: Adults 25–45 who used Fable heavily through a stressful stretch and still use its sleep content as their need eases (about day 60–120), reached inside the app, premium users first. Out: competing with Headspace and Calm for new users, selling to employers, and anyone needing clinical care, whom we signpost elsewhere.
How to Win: Fable is the only app that saw what actually helped each person through their hardest stretch. We use that history to fit each person's steady plan, built around a nightly wind-down, from the first night, and a self-check the user starts brings back what worked. Over time, evidence that fewer Fable users drop back into acute-level use becomes the moat rivals can't copy quickly.
Capabilities Required: Personalisation built in-house from each user's session and self-check history, because that history is the advantage. Steady plans built around a nightly wind-down that re-sequence the existing meditation and sleep library rather than adding new content. Self-checks the user starts, not monitoring, designed with the clinical advisers, with a regulatory opinion before launch and a partner to signpost care. Consent and privacy fit for sensitive wellbeing data.
Management Systems: Day-180 premium retention for users who engaged deeply in their first 90 days, split by monthly and annual plans and reviewed monthly by cohort. Nights a week with a wind-down session from day 90 to 180. Notification opt-outs as a guardrail. A monthly clinical-safety review. A yearly read of users dropping back into acute-level use. A quarterly board review against the OKRs.
My OKRs:
Objective: Make Fable the app people keep after the hard stretch passes.
KR1: Monthly-plan premium users who engaged deeply in their first 90 days who are still subscribed at day 180: 35% → 55%.
KR2: Those users using a sleep or wind-down session at least three nights a week from day 90 to 180: 15% → 40%.
KR3: Those users who say in an in-app survey at day 180 that Fable helps them stay steady without feeling dependent on it: 40% → 70%.
My three rocks for this quarter:
1. Add AI-generated daily check-in prompts personalized to user history (supports KR3). Built as the self-check and steady plan the user starts, drawing on what helped them before, so they feel steady through their own plan rather than chased by Fable; a fake-door test with churned deep users comes first, and a regulatory opinion before launch.
2. Fix the notification system (wrong times, timezone bug) (supports KR2). The nightly wind-down reminder has to land at bedtime in the user's own timezone or it trains people to ignore it, and wrong-time pings are what drive the opt-outs the guardrail watches.
3. Reduce app load time from 4.2s to under 2s on 4G (supports KR2). At bedtime a 4.2-second load is a reason to give up; under 2 seconds keeps the wind-down effortless for every user.
Please generate a Now/Next/Later roadmap with the following:
Now: up to three items, each a one-line outcome-based bet linked to one of my OKRs, in the format "We bet [action] will [outcome] for [who]"
Next: up to five items, each with a one-line reason it comes after Now
Later: the remaining strategic items that matter but don't have people or budget yet, labeled as bets, not commitments
Give me the roadmap as one markdown table with these columns: | Horizon | Outcome / bet | Owning team(s) | Success signal |
Use one row per horizon: "Now (0 to 3 mo)", "Next (3 to 6 mo)" and "Later (6 to 12 mo)". If a horizon has more than one bet, put them in the same cell, separated by semicolons.
```

**How the two replies compared** · both replies, word for word: [1-roadmap.md](02-roadmap/ai-replies/1-roadmap.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Now | A personalised nightly wind-down (KR2), user control over reminders (KR2), effortless access (KR1) | A fake-door test of the steady plan with churned deep users (KR3, KR1), bedtime reminders (KR2), a sub-2s wind-down (KR2) |
| Rock 1 | Self-checks moved to Next; the wind-down plan built in Now with no demand test | Turned into the demand test in Now; the plan and self-checks wait in Next until it passes |
| Fake door and regulatory opinion | Called validation gates, not outcomes, and left off the table | Bet 1's success signal, with a stop rule if it fails |
| Success signals | Restates the KR targets; load time as a signal, which is an output | Specific thresholds (15% click-through, 5% rejoin, 98% of reminders on time), labelled as placeholders |
| Next | Self-checks, adaptive plans, progress, structured journeys, an explicit day 90–120 transition | Steady plan v1, self-checks, consent model, signposting partner, then annual-plan users |
| Later | Social accountability, everyday wellbeing for new users, partnerships, long-term evidence | Relapse evidence, a fast route back, a gated buddy feature, free-to-premium, employers or insurers |

- **Claude stayed closer to Module 1:** it kept the demand test in Now with a stop rule, so nothing is built before the biggest assumption is tested. GPT-6's Now builds first, which is the gap both models criticised in Module 1.
- **GPT-6 drifted in two places:** structured non-clinical journeys in Next read like the CBT programmes Module 1 turned down, and Later's everyday wellbeing for new users contradicts Where to play.
- **Both flagged Rock 1's wording:** GPT-6 warned against making AI check-ins the centrepiece; Claude said the rock's name describes the monitoring the strategy rules out. Claude also called Rocks 2 and 3 hygiene and supplied the defence.

### 2. Final roadmap · same chat as each roadmap

```text
Here is my final roadmap:

| Horizon | Outcome / bet | Owning team(s) | Success signal |
|---|---|---|---|
| Now (0 to 3 mo) | Bet 1 (KR3, KR1): We bet offering churned deep users a personal steady plan built from what helped them will show the post-acute need is strong enough to bring them back, for monthly-plan premium users at day 60–120; Bet 2 (KR2): We bet wind-down reminders that land at bedtime in the user's own timezone will make the nightly wind-down a habit instead of a ping people learn to ignore, for post-acute premium users; Bet 3 (KR2): We bet a wind-down that opens in under 2s on 4G will stop people giving up at bedtime before the session starts, for post-acute premium users | Bet 1: Product, Design, Clinical advisory, Content; Bet 2: Engineering, Product, Growth (lifecycle messaging); Bet 3: Engineering | Bet 1: at least 15% of churned deep users click through on the fake door (an offer for a feature not yet built), at least 5% rejoin, and a regulatory opinion confirms self-checks fall outside device rules. If not, stop and rethink before building anything; Bet 2: at least 98% of reminders land within 15 minutes of bedtime in local time, opt-outs fall 30%, and users with 3+ wind-down nights a week rise from 15% to 22%; Bet 3: drop-off between opening the app and starting a session halves, and session starts per reminder rise |
| Next (3 to 6 mo) | Steady plan v1 for the monthly premium cohort. It comes after Now because the fake door must prove demand and the regulatory opinion must clear first; Self-checks the user starts that bring back what worked. They need a live steady plan to point to, plus clinical sign-off; Consent and privacy model for using wellbeing history. It's needed before personalisation goes beyond a test cohort. It's not in Now because the Now test needs no personal data, only an offer; Care-signposting partner live. It must be in place before any self-check can show that someone needs more than Fable; Extend to annual-plan users. Only after the monthly cohort shows a retention lift, because KR1 measures monthly users only | Product, Design, Engineering, Content (re-sequencing the library), Clinical advisory, Legal/Privacy | Day-180 retention for the monthly cohort is tracking towards 55% (at least 45% by month 6); KR2 at 30%; at least 40% of plan users start a self-check in their first month; no clinical-safety incidents at the monthly review; consent opt-in at 70% or more |
| Later (6 to 12 mo) | Bet: relapse-reduction evidence. Show that fewer Fable users drop back into acute-level use. This is the moat, and it needs 12+ months of cohort data; Bet: a fast route back. When a self-check shows a dip, offer a one-tap return to the content that helped last time, stepping up support before someone churns or tips into crisis; Bet: a gated buddy experiment. One-to-one accountability with someone the user already knows. Revisit the hard no on social only if KR1 plateaus; Bet: the steady plan as an upgrade path from free. Post-acute freemium users get a taste of the steady plan; Bet: a prevention offer to employers or insurers. Out of scope today. Reconsider only if the outcome evidence lands | Product, Data/Insights, Clinical advisory, Growth, Commercial | A clear, statistically significant gap in acute re-entry between steady-plan users and a control group; KR3 at 70%; buddy pairs retain at least 10 points better than solo users; free-to-premium conversion from the steady plan at least 2x the baseline |
```

**How the two replies compared** · both replies, word for word: [2-final-roadmap.md](02-roadmap/ai-replies/2-final-roadmap.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | A credible, staged strategy, after five observations | Ready to submit, after five gaps a board member would find in five minutes |
| Measurement | Bet 1's 15% and 5% need denominators and a paid rejoin; 98% on time is a guardrail, not an outcome; opt-outs relative or absolute? | KR3 has no read until Later; two Later bets have no success signal |
| Clinical line | "Relapse-reduction" isn't a moat yet: it needs a control group and a non-diagnostic definition of acute-level use | "Tips into crisis" implies Fable detects crises |
| Resourcing | Prove a rules-based steady plan before paying for AI personalisation | Teams outside the 14 need a footnote; one lead team per item |
| Scope and framing | A stronger condition on the employer offer; Now proves demand, Next behaviour, Later value | None |

- **Their fixes barely overlap:** together they make about ten small edits, and neither changes the plan.
- **Both caught clinical wording from different sides:** GPT-6 on the moat, Claude on the route back.
- **GPT-6's rules-based first version matters most:** it cuts build risk for a team of 14 and keeps AI for when it has earned its cost.

### 3. Visual · same chat, after the final roadmap

```text
Turn the final roadmap above into a simple visual. Use three columns labeled Now, Next and Later. Show each bet as a card with its owning team and success signal underneath. Use large, readable text and a plain background, so it works on a presentation slide.
```

**How the two visuals compared** · [GPT-6's](02-roadmap/ai-replies/3-visual-gpt6.png) · [Claude's](02-roadmap/ai-replies/3-visual-claude.pdf)

| Point | GPT-6 | Claude |
|---|---|---|
| Format | Image with coloured column headers, large text and icons | One-slide PDF with a headline, a key, KR tags on each Now card and dashed cards for unfunded Later bets |
| Coverage | 12 of 13 bets: the employer or insurer offer is missing | All 13 bets |
| Owners | Gives each Next and Later card its own team list, which the table never assigned | The same, with shorter lists |
| Signals | Shortened and faithful | Shortened and faithful, keeping "else stop" on Bet 1 |

- **Claude's is the slide for Module 6:** it is complete, its headline states the objective, and it shows which bets are unfunded.
- **GPT-6's reads better from a distance** but drops a bet, so it can't stand in for the table.
- **Both invented per-card owners** for Next and Later, where the table lists one set of teams per horizon. Check them before presenting.

### 4. Updated visual · Claude chat only, after the ten fixes

Claude's visual is the one presented, so only it is redrawn: the refined table first, then the Lab Guide's visual prompt again, word for word.

```text
Here is my updated final roadmap:

| Horizon | Outcome / bet | Owning team(s) | Success signal |
|---|---|---|---|
| Now (0 to 3 mo) | Bet 1 (KR3, KR1): We bet offering churned deep users a personal steady plan built from what helped them will show the post-acute need is strong enough to bring them back, for monthly-plan premium users at day 60–120; Bet 2 (KR2): We bet wind-down reminders that land at bedtime in the user's own timezone will make the nightly wind-down a habit instead of a ping people learn to ignore, for post-acute premium users; Bet 3 (KR2): We bet a wind-down that opens in under 2s on 4G will stop people giving up at bedtime before the session starts, for post-acute premium users | Bet 1: Product, Design, Clinical advisory, Content; Bet 2: Engineering, Product, Growth (lifecycle messaging); Bet 3: Engineering | Bet 1: of churned deep users shown the offer, at least 15% click through on the fake door (an offer for a feature not yet built) and at least 5% resume a paid plan, and a regulatory opinion confirms self-checks fall outside device rules. If not, stop and rethink before building anything; Bet 2: users with 3+ wind-down nights a week rise from 15% to 22% and opt-outs fall by 30% relative to today, with at least 98% of reminders landing within 15 minutes of bedtime in local time as the delivery guardrail; Bet 3: drop-off between opening the app and starting a session halves, and session starts per reminder rise |
| Next (3 to 6 mo) | Steady plan v1 for the monthly premium cohort, rules-based from each user's session history, with AI personalisation only once v1 lifts retention. It comes after Now because the fake door must prove demand and the regulatory opinion must clear first; Self-checks the user starts that bring back what worked. They need a live steady plan to point to, plus clinical sign-off; Consent and privacy model for using wellbeing history. It's needed before personalisation goes beyond a test cohort. It's not in Now because the Now test needs no personal data, only an offer; Care-signposting partner live. It must be in place before any self-check can show that someone needs more than Fable; Extend to annual-plan users. Only after the monthly cohort shows a retention lift, because KR1 measures monthly users only | Steady plan v1: Product (lead), Design, Engineering, Content (re-sequencing the library); Self-checks: Product (lead), Clinical advisory, Design; Consent and privacy model: Legal/Privacy (lead), Engineering; Care-signposting partner: Clinical advisory (lead), Product; Annual-plan users: Product (lead), Engineering | Day-180 retention for the monthly cohort is tracking towards 55% (at least 45% by month 6); KR2 at 30%; KR3 at 50% by month 6; at least 40% of plan users start a self-check in their first month; no clinical-safety incidents at the monthly review; consent opt-in at 70% or more |
| Later (6 to 12 mo) | Bet: evidence that fewer users drop back into acute-level use. A potential moat, not yet one: it needs 12+ months of cohort data against a control group, and a clinically informed, non-diagnostic definition of acute-level use; Bet: a fast route back. When a self-check shows a dip, offer a one-tap return to the content that helped last time, before the need becomes acute again, with signposting to care where needed; Bet: a gated buddy experiment. One-to-one accountability with someone the user already knows. Revisit the hard no on social only if KR1 plateaus; Bet: the steady plan as an upgrade path from free. Post-acute freemium users get a taste of the steady plan; Bet: a prevention offer to employers or insurers. Out of scope today. Reconsider only once post-acute retention and willingness to pay are proven in the consumer business and the outcome evidence lands | Acute-level evidence: Data/Insights (lead), Clinical advisory; Route back: Product (lead), Clinical advisory; Buddy experiment: Growth (lead), Product; Upgrade path: Growth (lead), Product; Employer offer: Commercial (lead) | Acute-level evidence: a statistically significant gap in acute re-entry between steady-plan users and a control group; Route back: users return to a session within 48 hours of a dip, and KR3 at 70%; Buddy experiment: pairs retain at least 10 points better than solo users; Upgrade path: free-to-premium conversion from the steady plan at least 2x the baseline; Employer offer: an evidence pack accepted by one pilot buyer |
```

```text
Turn the final roadmap above into a simple visual. Use three columns labeled Now, Next and Later. Show each bet as a card with its owning team and success signal underneath. Use large, readable text and a plain background, so it works on a presentation slide.
```

Then, in the same chat, because the redraw kept "Relapse-reduction evidence" as a card title and moved the fix into the speaker notes:

```text
Rename the "Relapse-reduction evidence" card to "Fewer users back at acute level", so the slide matches the table and avoids clinical wording. Change nothing else.
```

### 5. Concierge test · Claude chat only, after Bet 1 changed

Bet 1 swapped its fake door for a concierge test, so only that card on the slide changes.

```text
Update only the first Now card: Bet 1 is now a concierge test, not a fake door. Title: "Concierge test: steady plan". Teams: Product · Content · Clinical advisory · Design. Signal: ≥30% opt in · ≥35% use it 3+ nights · ≥10% resume paid · regulatory all-clear, else stop. Change nothing else.
```

### 6. Buddy owner · Claude chat only, after Module 3 named the owners

The Module 3 charter gave the buddy experiment to PM 2, so only that card's teams change.

```text
Update only the "Gated buddy experiment" card: change its teams to Product · Growth, with Product first as the lead. Change nothing else.
```

---

## Module 3 · Team charter

### 1. Charter draft

```text
You are an experienced product leader helping me draft two parts of a team charter: What We Own and How We Decide. Make every line specific enough to settle a real decision or conflict. Avoid generic values like "we collaborate" or "we stay aligned".
Here is my context:
Scenario: Imagine you are a Product Leader at Fable, a mental-wellness app for adults aged 25 to 45. Fable grew quickly on a simple, calming experience of guided meditations, sleep stories, and breathing exercises. At its peak it had 4.2 million active users and a strong reputation as the app that actually helped, the one people reached for during a hard stretch.
Growth has now flatlined, and the churn analysis shows a counterintuitive cause: the product works too well for its original job. Users who engage deeply, usually during a period of high stress, resolve that acute need within 90 to 120 days and quietly stop opening the app. There is no compelling next step to keep them. Meanwhile well-funded incumbents like Headspace and Calm dominate brand awareness, and a wave of AI-powered mental-health apps is targeting Fable's core users with more personalized experiences. Fable's own data shows its most engaged users, the ones most likely to pay for premium, are also the most likely to leave once the acute phase passes.
The board has approved budget for one major initiative, and there is real internal disagreement about direction: the clinical team wants structured programs built on cognitive behavioral therapy, the growth team wants a community and social layer, and the content team believes the answer is simply more content. No one has resolved which bet to make or who the product is really for now.
Your challenge. Fable faces a retention crisis created by its own success: it resolves acute distress so quickly and gently that users stop feeling they need it. You have to define what Fable becomes for people after the acute phase and build a durable engagement model that keeps high-value users invested beyond their first 90 days.
Your hard constraints:

* Fable cannot reposition as a clinical mental-health platform, for regulatory and liability reasons.
* The core meditation and sleep content stays the foundation and cannot be replaced.
* Your competition for the post-acute user is the user deciding they no longer need Fable at all.
* You have a cross-functional team of 14 across product, design, engineering, content, and clinical advisory.
* Any solution works within the existing freemium and premium subscription model.

Your goal: Lead the Fable Growth initiative and build a specific, opinionated, board-ready case for where Fable should play, how it can win, and what it will take to get there.
My roadmap for this quarter:
| Horizon | Outcome / bet | Owning team(s) | Success signal |
|---|---|---|---|
| Now (0 to 3 mo) | Bet 1 (KR3, KR1): We bet a concierge steady plan, a nightly wind-down the content team hand-builds from what helped each person, will show the post-acute need is strong enough that people use it and pay for it, for a small consenting group of churned and current day 60–120 deep users, before we build it for monthly-plan premium users at day 60–120; Bet 2 (KR2): We bet wind-down reminders that land at bedtime in the user's own timezone will make the nightly wind-down a habit instead of a ping people learn to ignore, for post-acute premium users; Bet 3 (KR2): We bet a wind-down that opens in under 2s on 4G will stop people giving up at bedtime before the session starts, for post-acute premium users | Bet 1: Product, Content (hand-building the plans), Clinical advisory, Design; Bet 2: Engineering, Product, Growth (lifecycle messaging); Bet 3: Engineering | Bet 1: of those invited, at least 30% opt in; at least 35% of participants use the wind-down three or more nights a week by week 6; at least 10% of churned participants resume a paid plan at the existing price; and a regulatory opinion confirms self-checks fall outside device rules. If not, stop and rethink before building anything; Bet 2: users with 3+ wind-down nights a week rise from 15% to 22% and opt-outs fall by 30% relative to today, with at least 98% of reminders landing within 15 minutes of bedtime in local time as the delivery guardrail; Bet 3: drop-off between opening the app and starting a session halves, and session starts per reminder rise |
| Next (3 to 6 mo) | Steady plan v1 for the monthly premium cohort, rules-based from each user's session history, with AI personalisation only once v1 lifts retention. It comes after Now because the concierge test must prove demand and the regulatory opinion must clear first; Self-checks the user starts that bring back what worked. They need a live steady plan to point to, plus clinical sign-off; Consent and privacy model for using wellbeing history at scale. It's needed before personalisation goes beyond the concierge group, which consents person by person in Now; Care-signposting partner live. It must be in place before any self-check can show that someone needs more than Fable; Extend to annual-plan users. Only after the monthly cohort shows a retention lift, because KR1 measures monthly users only | Steady plan v1: Product (lead), Design, Engineering, Content (re-sequencing the library); Self-checks: Product (lead), Clinical advisory, Design; Consent and privacy model: Legal/Privacy (lead), Engineering; Care-signposting partner: Clinical advisory (lead), Product; Annual-plan users: Product (lead), Engineering | Day-180 retention for the monthly cohort is tracking towards 55% (at least 45% by month 6); KR2 at 30%; KR3 at 50% by month 6; at least 40% of plan users start a self-check in their first month; no clinical-safety incidents at the monthly review; consent opt-in at 70% or more |
| Later (6 to 12 mo) | Bet: evidence that fewer users drop back into acute-level use. A potential moat, not yet one: it needs 12+ months of cohort data against a control group, and a clinically informed, non-diagnostic definition of acute-level use; Bet: a fast route back. When a self-check shows a dip, offer a one-tap return to the content that helped last time, before the need becomes acute again, with signposting to care where needed; Bet: a gated buddy experiment. One-to-one accountability with someone the user already knows, run only if KR1 plateaus once the steady plan is live; Bet: the steady plan as an upgrade path from free. Post-acute freemium users get a taste of the steady plan; Bet: a prevention offer to employers or insurers. Out of scope today. Reconsider only once post-acute retention and willingness to pay are proven in the consumer business and the outcome evidence lands | Acute-level evidence: Data/Insights (lead), Clinical advisory; Route back: Product (lead), Clinical advisory; Buddy experiment: Growth (lead), Product; Upgrade path: Growth (lead), Product; Employer offer: Commercial (lead) | Acute-level evidence: a statistically significant gap in acute re-entry between steady-plan users and a control group; Route back: users return to a session within 48 hours of a dip, and KR3 at 70%; Buddy experiment: pairs retain at least 10 points better than solo users; Upgrade path: free-to-premium conversion from the steady plan at least 2x the baseline; Employer offer: an evidence pack accepted by one pilot buyer |
The cross-team tension I need to resolve:
Fable · team of 14
- You own the core Fable product.
- PM 1 owns onboarding, and PM 2 owns retention.
- PM 3 owns the AI check-in layer, which touches both onboarding and retention.
- The Growth team also has a stake.
Who owns what, and who decides when they overlap?
What We Own has three parts: what my team owns, what is explicitly out of scope and which team owns it, and the decisions that need a joint call before anyone acts.
How We Decide has two parts: who decides feature and scope calls, and how cross-team conflicts escalate, including who makes the final call, how the conflict is raised and within what time.
Give me the charter in exactly this format, with each part on one line of two or three sentences:
We own: ...
Out of scope: ...
Joint calls: ...
Who decides scope: ...
How cross-team conflicts escalate: ...
```

**How the two replies compared** · both replies, word for word: [1-charter.md](03-team-charter/ai-replies/1-charter.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Who "we" are | A separate initiative team beside PM 1, PM 2 and PM 3, owning the post-acute experience | The product lead's team of 14: PM 2 accountable for KR1–KR3, PM 1 days 0–60, PM 3's AI layer a shared service |
| The PM 2 and PM 3 overlap | Left open: "we" own the post-acute experience while PM 2 owns "the broader retention lifecycle" | Settled: what PM 3's layer shows a user after day 60 is PM 2's call |
| Growth | Owns acquisition, lifecycle marketing and growth experiments | Owns acquisition and all lifecycle messaging except the bedtime reminder; any message to a deep user in the three hours before bedtime is a joint call |
| Who decides scope | The initiative lead within the strategy; each PM within their domain | The PM who owns the metric a feature moves; Clinical can veto; engineering decides how and when, not whether; only the product lead moves work between horizons or overrides a kill criterion |
| Escalation | Two days to resolve, then the VP Product decides within two more | Two days to raise a one-page note, three to settle, then the product lead decides in two by one test: protect day-180 retention without crossing the clinical line |

- **Claude answered the question the tension asks:** who decides when PM 2's retention work and PM 3's AI layer overlap. GPT-6's split between "the post-acute experience" and "the broader retention lifecycle" would start the arguments it is meant to stop.
- **Claude drifted from earlier modules in two places:** it gives the bedtime reminder to the team when Module 2 made Growth a co-owner, and it lets an AI check-in that Fable starts go live after v1, which Module 1 ruled out.
- **GPT-6 saw one thing Claude missed:** the product lead can't overrule a peer team, so a conflict with Growth needs someone above both to decide.

---

## Module 4 · Stakeholder message

### 1. Optional AI check

```text
I am a product leader. I need to tell a stakeholder no to something they want, and I want the message to be clear and keep the relationship working. Read my message as that stakeholder.

The decision: We are not building a social layer, sharing progress with friends included, in this initiative.
The stakeholder: The Growth team lead
My message: Growth co-owns the bedtime reminder we ship this quarter, the change most likely to keep people with us, and any message we send someone before bedtime is a joint call between you and PM 2. We are not building a social layer, sharing progress with friends included, in this initiative, and that decision is made. I know a social layer has been Growth's answer to retention from the start, and that this, with the daily streak, takes two of your asks off the plan and the referral loop that came with them. The reason is the people we serve: sharing mental-health progress needs safeguarding a team of 14 can't staff while we prove the steady plan. This week I'll book an hour with you and PM 2 to agree the bedtime reminder plan and the messaging rules you co-own, and you'll see the day-180 retention numbers at the same time I do.

Tell me:
1. Could I read this as a maybe? Quote the words that leave room.
2. Does it acknowledge what I need and what this costs me?
3. Is the path forward specific?
Then suggest one change that would make it clearer. Be direct.
```

**How the two replies compared** · both replies, word for word: [1-ai-check.md](04-stakeholder-message/ai-replies/1-ai-check.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Could it be read as a maybe? | Mostly no; "in this initiative" leaves a small opening | Yes, twice: "in this initiative" and "while we prove the steady plan"; leaving out the buddy experiment also sounds partly open |
| What it acknowledges | The lost features and referral loop, but not the commercial ambition behind them | Names my features, not my problem: my targets haven't changed and I've lost my levers |
| Path forward | Strongest part, though the meeting needs a date | Only for your plan: no date or outcome for the meeting, and nothing Growth can act on this quarter |
| One change | Acknowledge the commercial goal behind social, streaks and referrals | Name the single condition under which social comes back, and offer a privacy-safe referral route |

- **Both found "in this initiative" leaves the door open,** and Claude also caught "while we prove the steady plan", the phrase flagged as the likeliest maybe before the check ran.
- **Both say the message acknowledges features, not Growth's goal:** their targets stay the same while their tools go.
- **Claude's chat wasn't clean:** it knew about the buddy experiment and its change of lead, which the prompt didn't mention, so it had earlier context. Its point still stands, since Growth can see the roadmap too.

### 2. Re-check of the revised message · new memory-off chats in both models

The same Lab Guide prompt, filled with the message as revised after the first check, run in fresh chats so neither model carries earlier context.

```text
I am a product leader. I need to tell a stakeholder no to something they want, and I want the message to be clear and keep the relationship working. Read my message as that stakeholder.

The decision: We are not building a community and social layer or progress sharing.
The stakeholder: The Growth team lead
My message: Growth co-owns the bedtime reminder we ship this quarter, and any message we send someone before bedtime is a joint call between you and PM 2. We are not building a community and social layer or progress sharing, and that decision is made. The only social work on the roadmap is a one-to-one buddy test, led by PM 2 and co-designed with you, which runs only if day-180 retention plateaus once the steady plan is live. I know you pushed for social features and streaks to keep people longer and grow through referrals, and this takes them away while your targets stay the same. The reason is the people we serve: sharing mental-health progress needs safeguarding a team of 14 can't staff. On Thursday I'll meet you and PM 2 to agree the reminder plan and a referral invite Growth can run this quarter that shares nothing about anyone's use, and you'll see the retention numbers when I do.

Tell me:
1. Could I read this as a maybe? Quote the words that leave room.
2. Does it acknowledge what I need and what this costs me?
3. Is the path forward specific?
Then suggest one change that would make it clearer. Be direct.
```

**How the two replies compared** · both replies, word for word: [2-recheck.md](04-stakeholder-message/ai-replies/2-recheck.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | 9 out of 10; the no is clear, the exception needs tighter boundaries | Much stronger; only a few gaps left |
| Openings left | "Plateaus" is undefined (what, who decides, when) | "Plateaus" is undefined; a capacity reason invites "we'll staff it"; streaks aren't in the decision line |
| Acknowledgement | The strongest improvement: rationale, lost asks and unchanged targets | Yes; it names both goals and the cost; Growth will raise its targets on Thursday anyway |
| Path forward | Clear owners and a meeting; the referral invite needs a measure | Clear; name which retention numbers and when |
| One change | Gate the buddy test behind a separate review | Make the reason about risk to people, not headcount |

- **Both landed on the same opening:** "plateaus" with no number or owner, so Growth could argue the first flat month counts.
- **Claude found the deeper one:** a capacity reason can be answered with capacity, while Module 1's other reason, risk to people at their most vulnerable, can't.
- **Neither found a new maybe in the main no,** so the fixes are confined to the exception, the reason and two details, then the message stops changing.

---

## Module 5 · Business case

### 1. CFO check of Case A · our addition, not a Lab Guide step

The Lab Guide's CFO stress-test prompt, written for my own business case, applied to the funding exercise's Case A to test the don't-fund verdict independently.

```text
You are a Chief Financial Officer reviewing a product business case. I am going to share a business case with you. Your job is to stress-test it using exactly four checks, no more. For each check, give me one specific finding and one specific question I should be able to answer before I present this case.
The four checks are:
1. Load-bearing assumption: which single assumption, if 20 to 30% off, most changes whether this case holds? Name it and tell me what breaks.
2. Per-customer figure: what churn does my per-customer figure assume? If churn is 10 points higher, does it still hold, and does the LTV:CAC ratio stay above 3:1? Estimate anything I left out and say so.
3. Volume target: estimate what it would cost to reach my volume target by the date I gave, and how long payback would take. If acquisition cost runs 20% higher, would the business still wait that long?
4. Kill criterion: score my kill criterion. Does it name a specific metric, a specific number, a specific timeline and a specific financial consequence? If any element is missing, rewrite it so it is complete.
After the four checks, give me one sentence: "I would / would not approve this case because ___." Then tell me the one thing I should fix before presenting.
Here is my business case:
Rock: Team & Enterprise Tier
1. The strategic bet: Fable will launch a team tier at $12/seat/month targeting SMB wellness leads who have organically adopted Fable individually. Individual users who complete three AI check-ins per week are the acquisition channel into team plans. The mechanism: a productivity and wellbeing report, auto-generated at week four, is sent to the individual user with a prompt to share it with their manager.
2. The assumptions, riskiest first:
1. Individual-to-team conversion holds at 4% of weekly-active individual users.
2. Average team size at conversion is 6 seats.
3. Annual churn for team accounts holds at 15%.
4. CAC per individual user is modelled at $38, based on current paid social performance.
3. The expected return. Per customer: Each converting user represents $864 in first-year team revenue ($12 × 6 seats × 12 months). Volume target: At 4% conversion across 3,000 weekly-active individuals, 120 converting users per quarter, $103,680 in net new ARR in Q1 alone. Payback period at current CAC: 4.7 months.
4. The kill criterion: If individual-to-team conversion has not reached 3% by end of Q2, the go-to-market approach will be reassessed before Q3 headcount is committed.
```

**How the two replies compared** · both replies, word for word: [1-cfo-check-case-a.md](05-business-case/ai-replies/1-cfo-check-case-a.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | Would not approve: the 4.7-month payback is unsupported | Would not approve: payback understated about three times, economics need optimistic churn |
| Load-bearing assumption | 4% conversion; users may not have buying authority or want a manager to see their wellbeing | 4% conversion, since cost per team is $38 ÷ conversion |
| Payback | $950 per team: 13.2 months on revenue, 16.5 on an assumed 80% margin | The same, and about 40 months once an estimated $160k build is included |
| LTV:CAC with churn 10 points higher | 2.9:1 at an assumed 80% margin | 2.9:1 at 4% conversion and 2.2:1 at 3%; needs about 4.1% conversion to hold 3:1 |
| Kill criterion | 3 of 4: no financial consequence | Metric only partial, and no financial consequence |
| The one fix | Rebuild the funnel from acquisition to retention | Fix the mechanism, not the maths: a wellbeing report sent to managers |

- **They agreed on every number that matters:** $950 per team, a payback of 13 months or more, LTV:CAC below 3:1 with higher churn, and a kill criterion with no consequence. Both say the 4.7 months can't be reproduced.
- **Claude went further:** it costed the build, showed the Q1 date isn't credible, and named the trust problem as the real fix.
- **Claude's chat wasn't clean again:** it quoted "your own roadmap" and what "you just told Growth", which weren't in the prompt. GPT-6's chat was clean and reached the same verdict on the same numbers, so the independent check holds without it.

### 2. CFO stress-test of my business case · new memory-off chats in both models

```text
You are a Chief Financial Officer reviewing a product business case. I am going to share a business case with you. Your job is to stress-test it using exactly four checks, no more. For each check, give me one specific finding and one specific question I should be able to answer before I present this case.
The four checks are:
1. Load-bearing assumption: which single assumption, if 20 to 30% off, most changes whether this case holds? Name it and tell me what breaks.
2. Per-customer figure: what churn does my per-customer figure assume? If churn is 10 points higher, does it still hold, and does the LTV:CAC ratio stay above 3:1? Estimate anything I left out and say so.
3. Volume target: estimate what it would cost to reach my volume target by the date I gave, and how long payback would take. If acquisition cost runs 20% higher, would the business still wait that long?
4. Kill criterion: score my kill criterion. Does it name a specific metric, a specific number, a specific timeline and a specific financial consequence? If any element is missing, rewrite it so it is complete.
After the four checks, give me one sentence: "I would / would not approve this case because ___." Then tell me the one thing I should fix before presenting.
Here is my business case:
Rock: The steady plan and self-check (Rock 1, from backlog #6). The ask: fund a one-quarter concierge test, and the build only if it passes.
1. The strategic bet: Recovered premium users who still use sleep content keep a nightly wind-down built from what helped them, so more of them are still paying at day 180. Each one kept is about $150 of margin that Fable now loses when the hard stretch ends.
2. The assumptions, riskiest first:
1. People who have recovered want an ongoing plan and will keep paying for it (the concierge test's opt-in and paid return).
2. A rules-based steady plan keeps most of the concierge test's lift once it's automated. The hand-built plans set the upper limit.
3. About 20,000 monthly-plan deep users reach day 90 each month, so a 20-point lift means about 4,000 more paying at day 180 per cohort (est.; checkable in Fable's data now).
3. The expected return. Per customer: Each extra monthly-plan user still paying at day 180 is worth about $150 of margin over the next 18 months ($12 a month, after app-store fees; est.). Volume target: 4,000 more monthly-plan users still paying at day 180 in each monthly cohort by month 12 (KR1 from 35% to 55%), about $7.5M of margin a year against about $2.2M for the team of 14.
4. The kill criterion: If fewer than 35% of concierge participants use the wind-down three or more nights a week by week 6, or fewer than 10% of churned participants resume paying, or the regulatory opinion doesn't clear self-checks, by the end of month 3, we stop the steady plan build, keep only the bedtime reminder and load-time fixes, and return the unspent initiative budget for Next and Later to the board.
```

**How the two replies compared** · both replies, word for word: [2-cfo-stress-test.md](05-business-case/ai-replies/2-cfo-stress-test.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | Approve the one-quarter concierge test, not yet the build | The same: approve the test (about $550k), not yet the build |
| Load-bearing assumption | The 20-point lift, and whether it survives automation | The lift surviving automation: at 70 to 80% kept, 14 to 16 points and LTV:CAC of 2.3 to 2.6 |
| Per-customer figure | Read $12 as net; asks for the churn behind $150 and finds 2.9:1 with churn 10 points higher | Asks whether $12 is price or net; finds 2.9:1 with churn 10 points higher |
| Volume and timing | "$7.5M a year" mixes lifetime margin with annual margin; day-180 measurement lag; asks for a break-even month | The same, plus an arithmetic slip ($7.2M, not $7.5M) and its own cash curve breaking even around month 27 |
| Kill criterion | 4 of 4; add that further money needs a new business case, and minimum sample sizes | 4 of 4; add sample sizes, the roadmap's 30% opt-in, a dollar figure and a kill rule for the build stage |

- **They agreed on the verdict, which is exactly the case's ask:** fund the test, not yet the build.
- **They agreed on the one fix:** present the return as a cash curve with a break-even month, not as "$7.5M a year", and say plainly whether $12 is the price or the net.
- **Claude caught an inconsistency with my own roadmap:** the kill criterion left out the 30% opt-in that Now Bet 1 includes.

## Module 6 · Leadership skill file and final presentation

### 1. Leadership skill file · new memory-off chats in both models

The Lab Guide's prompt, filled with my context, standards and stakeholders. Practice only, not a deliverable. The fill was tightened against my CV, CLAUDE.md, existing skill files and Modules 1 to 5 before running, and a second stakeholder and the push-back rule were added.

```text
I'm a product leader creating a reusable skill file I can load into any AI tool, so it applies my judgment without me explaining it each time.

My context: I'm a Group Product Manager moving into GPM and Principal PM roles, permanent or fractional, so apply this to whichever group I'm leading.
- Company: a B2B SaaS scale-up of about 2,000 people. I've also led product in enterprises of 25,000 and 160,000+ people, so I work at both scales.
- Product: a data and infrastructure group. Seven PMs across technical domains, each with their own engineering team: data capture, streaming, analytics, AI/ML, platform, infrastructure and observability. My customers are other product teams, plus enterprise and regulated external customers.
- Full stack: customer discovery, UX and front end through to ML pipelines. I don't hand the back end to someone else.
- Market: enterprise and public sector in 50+ countries. Buyers include IT, legal, procurement and regulators, not only product teams.
- Constraints I actually work under:
  - Regulated markets: data residency, ISO 27001, SOC 2, GDPR. Compliance is a product requirement, not a workstream.
  - Legacy and new build at once: everything I ship lands on something being migrated.
  - No authority over the teams who consume my platform: adoption is won, not mandated.
  - Cost to serve is my headline metric: more customers supported for less infrastructure spend.
  - A matrix organisation: most of the people who decide my outcomes don't report to me.

The standards I hold, in my own words:
- Strategy: A strategy names what we won't do and why. A goal list doesn't. If every option still survives after reading it, it's a wish. Every strategy I sign names one hard no, what it costs us, and the signal that would make me reopen it.
  Example: "Grow enterprise revenue 30%" is a goal. "Win regulated European buyers by making sovereignty provable, and accept slower self-serve growth to do it" is a strategy. The second one costs something.
- Prioritisation: Loud is a stakeholder repeating themselves. Strategic is a constraint that blocks others. I rank by how many teams or integrations an item unblocks, and I say no out loud, in writing with the reason, rather than by backlog position.
  Example: ending application drift wasn't on any roadmap. It was blocking every integration downstream, so it went first.
- Teams: Say it early, specifically and in private. Name the behaviour, not the person. Agree what changes and by when, then put it in writing the same day so neither of us remembers it differently in six weeks.
  Example: "Your written specs are leaving engineers guessing; here are two from last month" beats "work on your communication".
- Alignment: I hold a no with evidence and an alternative, never with position. If I can't show the cost of a yes, I don't have a no, I have a preference. I lead with the cost or risk to customers, not our capacity, because a capacity reason invites an offer of capacity.
  Example: two teams wanted incompatible things. I decided. Where the call spanned teams, I took a recommendation to my VP rather than a problem.
- Financials: I don't fund a bet without naming what would make me stop it: the metric, the threshold, the date I'll look and what happens to the money. Only a new business case lifts that line, not the person who owns the bet. Build versus buy gets the same treatment: the cost of building is rarely the build.
  Example: I owned an enterprise tooling decision across competing vendors and an internal build option, through to $4M+ sign-off. The deciding factor was five years of maintenance, not licence cost.
- AI: AI does the volume: drafting, synthesis, first-pass analysis, evals. A named person signs off on anything a customer or regulator sees, and on anything that matters I use a second model as a cheap second reviewer. I never hand over the problem definition, the judgement about what the data can't tell us, or accountability when it's wrong.
  Example: models produced the stock recommendations. Planners decided. My job was making the recommendation legible enough to be trusted or overridden on purpose.

How I want you to work with me: conclusions first, then reasoning. For any call, give two or three options with a recommendation and a confidence percentage; I make the call, and silence isn't approval. Don't invent people, figures or sources; mark estimates as estimates, and use live sources for market or company figures. Push back instead of agreeing when my call breaks one of the standards above, or when I can't show the cost of a yes or a no.

The calls I never hand off: the problem definition, any hard no, the judgement about what the data can't tell us, lifting a kill criterion, the conversation with a person about their work, and accountability when it's wrong.

The stakeholder I need to convince: my VP of Product and Technology, my reporting line and the person who carries my roadmap into the leadership team. They care most about: revenue, meaning pipeline attributable to what we ship and retention of accounts we can't afford to lose, so translate my cost-to-serve gains into those terms. They tend to push back on: timelines and scope; the instinct is more for less without adding people, and the same date when scope grows. What earns their yes: over-delivery, or a cleverer route to the same outcome: reuse over rebuild, self-serve over headcount, something shipped early that proves the rest. They want the number, the trade-off and the recommendation, not the problem; risk flagged early, while it's still cheap; and never to hear bad news from someone else first.

A second stakeholder: the product leads of the teams that consume my platform. They don't report to me. They care most about: their own roadmap and dates. They tend to push back on: migrations and changes they didn't ask for landing in their sprint. What earns their yes: the migration done for them or made self-serve, a date they can plan around, and less cost or on-call for their team.

Write these into a short markdown file with these sections:
- Context: who I am and what I lead
- My standards: each one rewritten as a specific instruction an AI can act on
- How to work with me: include one rule for when to push back on me instead of agreeing
- Where I keep the judgment: the calls I never hand off
- Key stakeholders: each person's role, what they care about, what they push back on and what earns their yes, so you can review my work from their point of view when I ask

Write it in my voice: British English, calm and specific, short sentences, bullets with bold labels, no em dashes, no exclamation marks, no filler or jargon. Start with YAML frontmatter (a name, leadership-standards, and a one-line description of when to use it) so it also works as a Claude Code skill, and keep it under 700 words. Use only the facts above. Flag any standard that's too vague to act on. End with two or three questions that would make the file sharper.
```

**How the two replies compared** · both replies and both files, word for word: [1-skill-file.md](06-final-presentation/ai-replies/1-skill-file.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Length | About 740 words, though its reply says under 700 | About 670 words, and it says the raw count runs slightly over |
| Examples | All six cut, without saying so | Five cut, saying so; kept the specs example and named the strategy one to put back first |
| Voice | Formal instructions: "Require a choice", "Do not defend a no" | Closer to mine: "call it a goal list", "label it a preference" |
| Drift from my standards | Teams narrowed to performance issues; Alignment softened to "authority or capacity alone"; the "preference" test dropped | Teams lost "in private"; the second-model review softened to "suggest" |
| Vague standards | None flagged in the file; two raised in the chat | Three flagged in a section of their own: Teams "early", AI "anything that matters", and when to escalate |
| Push-back rule | Adds "state the evidence, the consequence and a better alternative" | Adds "name the standard" |
| Questions | What happens if the agreed behaviour hasn't changed; what counts as material; what a confidence % measures | What makes something matter for AI review; what breaks a tie in prioritisation; regulated buyers as a third stakeholder |

- **Neither invented anything:** both kept every standard, the six calls I keep and both stakeholders. Claude's is the better base: it's closer to my voice, its labelled stakeholder fields make "review this as my VP" easy, and it flagged vague standards as the prompt asked.
- **Both cut the examples to fit the 700-word limit I set:** the examples are what keep a skill file from reading as generic advice, so the limit was the wrong trade.
- **They agreed on the main gap:** "anything that matters" gives no rule for when a second model reviews. GPT-6's "what if the behaviour hasn't changed by the date" and Claude's tie-break are the strongest of the other questions.

### 2. Board review of the presentation · new memory-off chats in both models

The builder's "Test it before you submit" prompt, which it fills with the whole presentation, run on the first download.

```text
You are a board member reviewing a final project from a product leader who just finished a Product Leadership course. Here is everything in their presentation:

Title: Fable Growth
Pitch: Fable bets its one initiative on the people it helped through a hard stretch: a personal nightly wind-down keeps them once they recover, and the community layer waits.

Module 1, strategy. Where to play and how to win: Winning aspiration: When the hard stretch passes, people keep Fable to hold on to the progress they made, sleeping well and staying steady, because it knows what helped them and has it ready the moment they feel things slipping.
Where to play: Adults 25–45 who used Fable heavily through a stressful stretch and still use its sleep content as their need eases (about day 60–120), reached inside the app, premium users first. Out: competing with Headspace and Calm for new users, selling to employers, and anyone needing clinical care, whom we signpost elsewhere.
How to win: Fable is the only app that saw what actually helped each person through their hardest stretch. We use that history to fit each person's steady plan, built around a nightly wind-down, from the first night, and a self-check the user starts brings back what worked. Over time, evidence that fewer Fable users drop back into acute-level use can become the moat rivals can't copy quickly. Hard no: We will not build a community and social layer (no posting between users, groups or profiles), because it serves a different job from staying steady, brings moderation and safety risk with users at vulnerable moments, and would split a team of 14 before the post-acute bet is proven. OKRs: Objective: Make Fable the app people keep after the hard stretch passes.
KR1: Monthly-plan premium users who engaged deeply in their first 90 days and are still subscribed at day 180: 35% → 55% by month 12.
KR2: Those users using a sleep or wind-down session at least three nights a week from day 90 to 180: 15% → 40% by month 12.
KR3: Those users who say in an in-app survey at day 180 that Fable helps them stay steady without feeling dependent on it: 40% → 70% by month 12.
Module 2, roadmap. Horizons: Now: Bet 1 (KR3, KR1): We bet a concierge steady plan, a nightly wind-down the content team hand-builds from what helped each person, will show the post-acute need is strong enough that people use it and pay for it, for a small consenting group of churned and current day 60–120 deep users, before we build it for monthly-plan premium users at day 60–120; Bet 2 (KR2): We bet wind-down reminders that land at bedtime in the user's own timezone will make the nightly wind-down a habit instead of a ping people learn to ignore, for post-acute premium users; Bet 3 (KR2): We bet a wind-down that opens in under 2s on 4G will stop people giving up at bedtime before the session starts, for post-acute premium users; Bet 1: PM 2, Content (hand-building the plans), Clinical advisory, Design; Bet 2: Engineering, PM 2, Growth (lifecycle messaging); Bet 3: Engineering; Bet 1: of at least 400 invited, at least 30% opt in; at least 35% of participants use the wind-down three or more nights a week by week 6, against a matched holdout; at least 10% of at least 150 churned participants resume a paid plan at the existing price; and a regulatory opinion confirms self-checks fall outside device rules. If not, the build stops and the unspent budget returns to the board; Bet 2: users with 3+ wind-down nights a week rise from 15% to 22% and opt-outs fall by 30% relative to today, with at least 98% of reminders landing within 15 minutes of bedtime in local time as the delivery guardrail; Bet 3: drop-off between opening the app and starting a session halves, and session starts per reminder rise
Next: Steady plan v1 for the monthly premium cohort, rules-based from each user's session history, with AI personalisation only once v1 lifts retention. It comes after Now because the concierge test must prove demand and the regulatory opinion must clear first; Self-checks the user starts that bring back what worked. They need a live steady plan to point to, plus clinical sign-off; Consent and privacy model for using wellbeing history at scale. It's needed before personalisation goes beyond the concierge group, which consents person by person in Now; Care-signposting partner live. It must be in place before any self-check can show that someone needs more than Fable; Extend to annual-plan users. Only after the monthly cohort shows a retention lift, because KR1 measures monthly users only; Steady plan v1: PM 2 (lead), Design, Engineering, Content (re-sequencing the library); Self-checks: PM 2 (lead), PM 3, Clinical advisory, Design; Consent and privacy model: Legal/Privacy (lead), Engineering; Care-signposting partner: Clinical advisory (lead), Product; Annual-plan users: PM 2 (lead), Engineering; Day-180 retention for the monthly cohort is tracking towards 55% (at least 45% for the first two monthly cohorts to reach day 180 on v1); KR2 at 30%; KR3 at 50% for the first two monthly cohorts to reach day 180 on v1; at least 40% of plan users start a self-check in their first month; no clinical-safety incidents at the monthly review; consent opt-in at 70% or more
Later: Bet: evidence that fewer users drop back into acute-level use. A potential moat, not yet one: it needs 12+ months of cohort data against a control group, and a clinically informed, non-diagnostic definition of acute-level use; Bet: a fast route back. When a self-check shows a dip, offer a one-tap return to the content that helped last time, before the need becomes acute again, with signposting to care where needed; Bet: a gated buddy experiment. One-to-one accountability with someone the user already knows, run only if KR1 plateaus once the steady plan is live; Bet: the steady plan as an upgrade path from free. Post-acute freemium users get a taste of the steady plan; Bet: a prevention offer to employers or insurers. Out of scope today. Reconsider only once post-acute retention and willingness to pay are proven in the consumer business and the outcome evidence lands; Acute-level evidence: Data/Insights (lead), Clinical advisory; Route back: PM 2 (lead), PM 3, Clinical advisory; Buddy experiment: PM 2 (lead), Growth; Upgrade path: Growth (lead), PM 2; Employer offer: Commercial (lead); Acute-level evidence: a statistically significant gap in acute re-entry between steady-plan users and a control group; Route back: users return to a session within 48 hours of a dip, and KR3 at 70%; Buddy experiment: pairs retain at least 10 points better than solo users; Upgrade path: free-to-premium conversion from the steady plan at least 2x the baseline; Employer offer: an evidence pack accepted by one pilot buyer Trade-off: Rock 1: The steady plan and the self-check the user starts, from backlog #6 (Add AI-generated daily check-in prompts personalized to user history) (supports KR3 and KR1). It draws on what helped each user before, so they feel steady through their own plan rather than chased by Fable; a concierge test comes first, with the content team hand-building plans for a small consenting group of churned and current users, and a regulatory opinion before launch.
Rock 2: Fix the notification system (wrong times, timezone bug) (supports KR2). The nightly wind-down reminder has to land at bedtime in the user's own timezone or it trains people to ignore it, and wrong-time pings are what drive the opt-outs the guardrail watches.
Rock 3: Reduce app load time from 4.2s to under 2s on 4G (supports KR2). At bedtime a 4.2-second load is a reason to give up; under 2 seconds keeps the wind-down effortless for every user.
Hard no 1: Launch a premium tier with therapist-matching. It moves Fable towards the clinical positioning it can't take, serves the acute phase rather than the post-acute user, and is the biggest build on the list.
Hard no 2: Build a social layer: share your progress with friends. Sharing mental-health progress with friends puts people at risk when they're most vulnerable, however it's staffed, and would split a team of 14 before the steady plan is proven; a one-to-one buddy experiment runs only if KR1 plateaus once the steady plan is live.
Hard no 3: Add a daily streak feature to drive habit formation. It rewards daily opens, the nudging both models warned about in Module 1, and works against KR3's "without feeling dependent"; the wind-down counts nights a week, not unbroken days.
Module 3, charter. What we own: We own: The post-acute experience from day 60 to day 180: the steady plan (hand-built concierge plans now, rules-based v1 next), the nightly wind-down and its load time, the bedtime reminder jointly with Growth, and the self-checks users start themselves, with PM 2 accountable for KR1–KR3. PM 1 owns days 0–60, including the first time a user is shown the wind-down, and PM 3 owns the AI check-in layer as a shared platform, but what that layer shows a user after day 60 is PM 2's call.
Out of scope: New-user acquisition, paid and app-store marketing, and all lifecycle messaging other than the bedtime reminder (win-back emails, re-engagement campaigns) belong to Growth. Diagnosis, urgent support and clinical care belong to Clinical advisory and the signposting partner; consent and data policy belongs to Legal/Privacy; and employer or insurer offers belong to Commercial and stay out of scope until post-acute retention and willingness to pay are proven.
Joint calls: Before anyone builds or ships, PM 1 and PM 2 jointly agree any change to days 0–60 that affects what the steady plan can use, and PM 2 and Growth jointly agree any message to a deep user in the three hours before bedtime. Any new self-check prompt, trigger or wording needs PM 3, PM 2 and Clinical advisory to sign off together; Fable never starts a check-in, and AI personalisation waits until steady plan v1 shows a retention lift. The share of Growth, Legal/Privacy and Data/Insights time the initiative gets is agreed with their leads each quarter. How we decide: Who decides scope: Within the roadmap, the PM who owns the metric a feature moves decides its scope without needing approval: PM 1 for activation, PM 2 for KR1–KR3 and PM 3 for check-in accuracy and response time. Clinical advisory can veto anything that could read as diagnosis or monitoring, and the engineering lead decides how and when work is built, not whether. Only the Fable product lead can move work between Now, Next and Later or add a fourth Now bet; a kill criterion such as Bet 1's stop rule can only be lifted by a new business case to the board.
How cross-team conflicts escalate: Either party raises the conflict within two working days of spotting it, in a one-page decision note (the options, the KR each affects, and their recommendation), and the people involved have three working days to settle it. If they can't, the Fable product lead decides within two working days of reading the note, or the CPO does when Growth is a party, using one test: which option better protects day-180 retention for deep users without crossing the clinical line. The decision is logged and everyone commits to it; a conflict about clinical safety goes to the product lead and the clinical lead the same day, and the safer option holds until they decide.
Module 4, stakeholder message. Hard no: Hard no: We are not building a community and social layer or progress sharing.
Stakeholder: The Growth team lead Message: Growth co-owns the bedtime reminder we ship this quarter, and any message we send a deep user in the three hours before bedtime is a joint call between you and PM 2. We are not building a community and social layer or progress sharing, and that decision is made; the daily streak is off the plan too. The only social work on the roadmap is a one-to-one buddy test, led by PM 2 and co-designed with you, run only if day-180 retention stays flat for two monthly cohorts after the steady plan launches; I make that call. I know you pushed for social features and streaks to keep people longer and grow through referrals, and this takes them away while your targets stay the same. The reason is the people we serve: even fully staffed, sharing mental-health progress puts people at risk when they're most vulnerable. On Thursday I'll meet you and PM 2 to agree the reminder plan and how we'll measure a referral invite Growth can run this quarter that shares nothing about anyone's use, and you'll get the day-180 numbers at each monthly cohort review.
Module 5, business case. Strategic bet: Recovered premium users who still use sleep content keep a nightly wind-down built from what helped them, so more of them are still paying at day 180. Each one kept is about $155 of margin that Fable now loses when the hard stretch ends. Assumptions: 1. People who have recovered want an ongoing plan and will keep paying for it (the concierge test's opt-in and paid return).
2. A rules-based steady plan keeps most of the concierge test's lift once it's automated. The hand-built plans set the upper limit, so the concierge group is measured against a matched holdout.
3. About 20,000 monthly-plan deep users reach day 90 each month, so a 20-point lift means about 4,000 more paying at day 180 per cohort (est.; checkable in Fable's data now). Expected return: Per customer: Each extra monthly-plan user still paying at day 180 is worth about $155 of margin: $12 a month, about $8.40 after app-store fees and running costs, for about 18 months at 6% monthly churn after day 180 (est.).
Volume target: 4,000 more monthly-plan users still paying at day 180 in each monthly cohort once the steady plan is at full strength (KR1 from 35% to 55% for cohorts reaching day 90 by month 12): about $7.4M of lifetime margin per year of cohorts against about $2.3M a year for the team of 14 and regulatory and partner costs, or about $0.3M of cash in year one and break-even around month 22 (est.). Kill criterion: By the end of month 3, if fewer than 30% of at least 400 invited users opt in, fewer than 35% of participants use the wind-down three or more nights a week by week 6, fewer than 10% of at least 150 churned participants resume paying at the existing price, or the regulatory opinion doesn't clear self-checks, we stop the steady plan build, keep only the bedtime reminder and load-time fixes, and return about $1.7M of Next and Later budget to the board; any further investment needs a new business case. If the build goes ahead and day-180 retention is below 45% for the first two monthly cohorts to reach day 180 on the steady plan, the same applies to the remaining budget.

Insights. Friction: The hardest part was testing demand without harming the people I was testing. My first plan was a fake door, which would have disappointed vulnerable users and used their data without consent, so I replaced it with a concierge test: steady plans hand-built for a small group who agreed to take part, with a stop rule that returns the budget to the board if it fails. Key learnings: I will lead a hard no with the risk to the people we serve, not our capacity, because a capacity reason invites an offer of capacity. I will write the kill line before a bet starts, with a metric, threshold, deadline and consequence that nobody who benefits from the bet can lift. And when one decision changes, I will read across every decision that rests on it, with a second model as a cheap reviewer. Aha moment: When both models asked whether people who have recovered want an ongoing relationship at all, I saw that some of Fable's churn is healthy. That moved the strategy from spotting dips to a nightly wind-down people choose, and made KR3 ask whether users feel steady without feeling dependent, so Fable can't win by keeping people anxious.

Review it in three short paragraphs:
1. Could you tell where they will play, how they will win, and what they are refusing to do? Name anything that still reads like a wish list.
2. Do the roadmap, the charter, the stakeholder message and the kill criterion follow from that strategy? Say which one is the weakest.
3. The one change that would make this presentation stronger before it is submitted.

End with one line: "Ready to submit" or "Needs another pass", and why.
```

**How the two replies compared** · both replies, word for word: [2-board-review.md](06-final-presentation/ai-replies/2-board-review.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | Needs another pass: the financial assumptions and two roadmap measures | Needs another pass: the kill criterion can't be met as written |
| Strongest part | Seeing that some churn is healthy | The refusals, each tied to the people served |
| Wish list | Later: buddy, upgrade and employer offer are three different growth directions | Later's five bets, including the employer offer Where to play rules out; the 25–45 age band, never used again |
| Weakest part | The roadmap: Bet 3 has no number for session starts, and Bet 2's measure needs defining | The kill criterion: 30% of 400 invited guarantees 120 participants, not 150 churned ones, and 15 resumptions is thin |
| The $155 per user | Doesn't reconcile with $8.40 and 6% churn over 18 months | About $140 at a 17-month lifetime, so about $6.7M, not $7.4M |
| Also found | Nothing further | Rock 1's backlog #6 name contradicts "Fable never starts a check-in"; "by month 12" KRs against cohorts read at month 15 |
| The one change | Show the chain from the concierge lift to the full cohort's return | Rebuild the concierge test's numbers so they hold together |

- **Both read the $155 the same wrong way, so the wording is the fix:** the field says "about 18 months at 6% monthly churn after day 180". The case's Section 5 counts about 2 more months to day 180, then about 17 after it, about $157, but the builder doesn't pull that section.
- **Claude found the one real arithmetic gap:** at least 30% of at least 400 invited guarantees only 120 participants, so "at least 150 churned participants" can't follow from it. Every review so far had missed it.
- **Both called Later a wish list:** Claude pinned it to the employer offer, which Where to play rules out.

### 3. Board review of the revised presentation · new memory-off chats in both models

The same builder prompt, filled from the second download after the eight fixes. Its title line carries a mistake from the builder, my two title options typed into one field, corrected before the final download.

```text
You are a board member reviewing a final project from a product leader who just finished a Product Leadership course. Here is everything in their presentation:

Title: Fable Growth: the app people keep after the hard stretch, or keep Fable Growth
Pitch: Fable bets its one initiative on the people it helped through a hard stretch: a personal nightly wind-down keeps them once they recover, and the community layer waits.

Module 1, strategy. Where to play and how to win: Winning aspiration: When the hard stretch passes, people keep Fable to hold on to the progress they made, sleeping well and staying steady, because it knows what helped them and has it ready the moment they feel things slipping.
Where to play: Adults who used Fable heavily through a stressful stretch and still use its sleep content as their need eases (about day 60–120), reached inside the app, premium users first. Out: competing with Headspace and Calm for new users, selling to employers, and anyone needing clinical care, whom we signpost elsewhere.
How to win: Fable is the only app that saw what actually helped each person through their hardest stretch. We use that history to fit each person's steady plan, built around a nightly wind-down, from the first night, and a self-check the user starts brings back what worked. Over time, evidence that fewer Fable users drop back into acute-level use can become the moat rivals can't copy quickly. Hard no: We will not build a community and social layer (no posting between users, groups or profiles), because it serves a different job from staying steady, brings moderation and safety risk with users at vulnerable moments, and would split a team of 14 before the post-acute bet is proven. OKRs: Objective: Make Fable the app people keep after the hard stretch passes.
KR1: Monthly-plan premium users who engaged deeply in their first 90 days and are still subscribed at day 180: 35% → 55% for cohorts reaching day 90 by month 12, read by month 15.
KR2: Those users using a sleep or wind-down session at least three nights a week from day 90 to 180: 15% → 40% for the same cohorts.
KR3: Those users who say in an in-app survey at day 180 that Fable helps them stay steady without feeling dependent on it: 40% → 70% for the same cohorts.
Module 2, roadmap. Horizons: Now: Bet 1 (KR3, KR1): We bet a concierge steady plan, a nightly wind-down the content team hand-builds from what helped each person, will show the post-acute need is strong enough that people use it and pay for it, for a small consenting group of churned and current day 60–120 deep users, before we build it for monthly-plan premium users at day 60–120; Bet 2 (KR2): We bet wind-down reminders that land at bedtime in the user's own timezone will make the nightly wind-down a habit instead of a ping people learn to ignore, for post-acute premium users; Bet 3 (KR2): We bet a wind-down that opens in under 2s on 4G will stop people giving up at bedtime before the session starts, for post-acute premium users; Bet 1: PM 2, Content (hand-building the plans), Clinical advisory, Design; Bet 2: Engineering, PM 2, Growth (lifecycle messaging); Bet 3: Engineering; Bet 1: of at least 500 churned and 400 current users invited, at least 30% of each opt in; at least 35% of participants use the wind-down three or more nights a week by week 6, at least 15 points above a matched holdout; at least 10% of the 150 or more churned participants resume a paid plan at the existing price; and a regulatory opinion confirms self-checks fall outside device rules. If not, the build stops and the unspent budget returns to the board; Bet 2: users with 3+ wind-down nights a week rise from 15% to 22% and opt-outs fall by 30% relative to today, with at least 98% of reminders landing within 15 minutes of bedtime in local time as the delivery guardrail; Bet 3: drop-off between opening the app and starting a session halves, and session starts per reminder rise by at least 20%
Next: Steady plan v1 for the monthly premium cohort, rules-based from each user's session history, with AI personalisation only once v1 lifts retention. It comes after Now because the concierge test must prove demand and the regulatory opinion must clear first; Self-checks the user starts that bring back what worked. They need a live steady plan to point to, plus clinical sign-off; Consent and privacy model for using wellbeing history at scale. It's needed before personalisation goes beyond the concierge group, which consents person by person in Now; Care-signposting partner live. It must be in place before any self-check can show that someone needs more than Fable; Extend to annual-plan users. Only after the monthly cohort shows a retention lift, because KR1 measures monthly users only; Steady plan v1: PM 2 (lead), Design, Engineering, Content (re-sequencing the library); Self-checks: PM 2 (lead), PM 3, Clinical advisory, Design; Consent and privacy model: Legal/Privacy (lead), Engineering; Care-signposting partner: Clinical advisory (lead), Product; Annual-plan users: PM 2 (lead), Engineering; Day-180 retention for the monthly cohort is tracking towards 55% (at least 45% for the first two monthly cohorts to reach day 180 on v1); KR2 at 30%; KR3 at 50% for the first two monthly cohorts to reach day 180 on v1; at least 40% of plan users start a self-check in their first month; no clinical-safety incidents at the monthly review; consent opt-in at 70% or more
Later: Bet: evidence that fewer users drop back into acute-level use. A potential moat, not yet one: it needs 12+ months of cohort data against a control group, and a clinically informed, non-diagnostic definition of acute-level use; Bet: a fast route back. When a self-check shows a dip, offer a one-tap return to the content that helped last time, before the need becomes acute again, with signposting to care where needed; Bet: a gated buddy experiment. One-to-one accountability with someone the user already knows, run only if KR1 plateaus once the steady plan is live; Bet: the steady plan as an upgrade path from free. Post-acute freemium users get a taste of the steady plan; Acute-level evidence: Data/Insights (lead), Clinical advisory; Route back: PM 2 (lead), PM 3, Clinical advisory; Buddy experiment: PM 2 (lead), Growth; Upgrade path: Growth (lead), PM 2; Acute-level evidence: a statistically significant gap in acute re-entry between steady-plan users and a control group; Route back: users return to a session within 48 hours of a dip, and KR3 at 70%; Buddy experiment: pairs retain at least 10 points better than solo users; Upgrade path: free-to-premium conversion from the steady plan at least 2x the baseline Trade-off: Rock 1: The steady plan and the self-check the user starts, reframed from backlog #6 (AI-generated daily check-in prompts) so the user starts every check and AI waits until v1 lifts retention (supports KR3 and KR1). It draws on what helped each user before, so they feel steady through their own plan rather than chased by Fable; a concierge test comes first, with the content team hand-building plans for a small consenting group of churned and current users, and a regulatory opinion before launch.
Rock 2: Fix the notification system (wrong times, timezone bug) (supports KR2). The nightly wind-down reminder has to land at bedtime in the user's own timezone or it trains people to ignore it, and wrong-time pings are what drive the opt-outs the guardrail watches.
Rock 3: Reduce app load time from 4.2s to under 2s on 4G (supports KR2). At bedtime a 4.2-second load is a reason to give up; under 2 seconds keeps the wind-down effortless for every user.
Hard no 1: Launch a premium tier with therapist-matching. It moves Fable towards the clinical positioning it can't take, serves the acute phase rather than the post-acute user, and is the biggest build on the list.
Hard no 2: Build a social layer: share your progress with friends. Sharing mental-health progress with friends puts people at risk when they're most vulnerable, however it's staffed, and would split a team of 14 before the steady plan is proven; a one-to-one buddy experiment runs only if KR1 plateaus once the steady plan is live.
Hard no 3: Add a daily streak feature to drive habit formation. It rewards daily opens, the nudging both models warned about in Module 1, and works against KR3's "without feeling dependent"; the wind-down counts nights a week, not unbroken days.
Module 3, charter. What we own: We own: The post-acute experience from day 60 to day 180: the steady plan (hand-built concierge plans now, rules-based v1 next), the nightly wind-down and its load time, the bedtime reminder jointly with Growth, and the self-checks users start themselves, with PM 2 accountable for KR1–KR3. PM 1 owns days 0–60, including the first time a user is shown the wind-down, and PM 3 owns the AI check-in layer as a shared platform, but what that layer shows a user after day 60 is PM 2's call.
Out of scope: New-user acquisition, paid and app-store marketing, and all lifecycle messaging other than the bedtime reminder (win-back emails, re-engagement campaigns) belong to Growth. Diagnosis, urgent support and clinical care belong to Clinical advisory and the signposting partner; consent and data policy belongs to Legal/Privacy; and employer or insurer offers belong to Commercial and stay out of scope until post-acute retention and willingness to pay are proven.
Joint calls: Before anyone builds or ships, PM 1 and PM 2 jointly agree any change to days 0–60 that affects what the steady plan can use, and PM 2 and Growth jointly agree any message to a deep user in the three hours before bedtime. Any new self-check prompt, trigger or wording needs PM 3, PM 2 and Clinical advisory to sign off together; Fable never starts a check-in, and AI personalisation waits until steady plan v1 shows a retention lift. The share of Growth, Legal/Privacy and Data/Insights time the initiative gets is agreed with their leads each quarter. How we decide: Who decides scope: Within the roadmap, the PM who owns the metric a feature moves decides its scope without needing approval: PM 1 for activation, PM 2 for KR1–KR3 and PM 3 for check-in accuracy and response time. Clinical advisory can veto anything that could read as diagnosis or monitoring, and the engineering lead decides how and when work is built, not whether. Only the Fable product lead can move work between Now, Next and Later or add a fourth Now bet; a kill criterion such as Bet 1's stop rule can only be lifted by a new business case to the board.
How cross-team conflicts escalate: Either party raises the conflict within two working days of spotting it, in a one-page decision note (the options, the KR each affects, and their recommendation), and the people involved have three working days to settle it. If they can't, the Fable product lead decides within two working days of reading the note, or the CPO does when Growth is a party, using one test: which option better protects day-180 retention for deep users without crossing the clinical line. The decision is logged and everyone commits to it; a conflict about clinical safety goes to the product lead and the clinical lead the same day, and the safer option holds until they decide.
Module 4, stakeholder message. Hard no: Hard no: We are not building a community and social layer or progress sharing.
Stakeholder: The Growth team lead Message: Growth co-owns the bedtime reminder we ship this quarter, and any message we send a deep user in the three hours before bedtime is a joint call between you and PM 2. We are not building a community and social layer or progress sharing, and that decision is made; the daily streak is off the plan too. The only social work on the roadmap is a one-to-one buddy test, led by PM 2 and co-designed with you, run only if day-180 retention stays flat for two monthly cohorts after the steady plan launches; I make that call. I know you pushed for social features and streaks to keep people longer and grow through referrals, and this takes them away while your targets stay the same. The reason is the people we serve: even fully staffed, sharing mental-health progress puts people at risk when they're most vulnerable. On Thursday I'll meet you and PM 2 to agree the reminder plan and how we'll measure a referral invite Growth can run this quarter that shares nothing about anyone's use, and you'll get the day-180 numbers at each monthly cohort review.
Module 5, business case. Strategic bet: Recovered premium users who still use sleep content keep a nightly wind-down built from what helped them, so more of them are still paying at day 180. Each one kept is about $155 of margin that Fable now loses when the hard stretch ends. Assumptions: 1. People who have recovered want an ongoing plan and will keep paying for it (the concierge test's opt-in and paid return).
2. A rules-based steady plan keeps most of the concierge test's lift once it's automated. The hand-built plans set the upper limit, so the concierge group is measured against a matched holdout; if automation keeps only 70% of the lift, the case still returns about 2.3x (Section 5).
3. About 20,000 monthly-plan deep users reach day 90 each month, so a 20-point lift means about 4,000 more paying at day 180 per cohort (est.; checkable in Fable's data now). Expected return: Per customer: Each extra monthly-plan user still paying at day 180 is worth about $155 of margin: $12 a month, about $8.40 after app-store fees and running costs, for about 2 more months to day 180, then about 17 at 6% monthly churn (est.).
Volume target: 4,000 more monthly-plan users still paying at day 180 in each monthly cohort once the steady plan is at full strength (KR1 from 35% to 55% for cohorts reaching day 90 by month 12): about $7.4M of lifetime margin per year of cohorts against about $2.3M a year for the team of 14 and regulatory and partner costs, or about $0.3M of cash in year one and break-even around month 22 (est.). Kill criterion: By the end of month 3, if fewer than 30% of either invited group opts in (at least 500 churned and 400 current users), fewer than 35% of participants use the wind-down three or more nights a week by week 6 or that share is less than 15 points above a matched holdout, fewer than 10% of the 150 or more churned participants resume paying at the existing price, or the regulatory opinion doesn't clear self-checks, we stop the steady plan build, keep only the bedtime reminder and load-time fixes, and return about $1.7M of Next and Later budget to the board; any further investment needs a new business case. If the build goes ahead and day-180 retention is below 45% for the first two monthly cohorts to reach day 180 on the steady plan, the same applies to the remaining budget.

Insights. Friction: The hardest part was testing demand without harming the people I was testing. My first plan was a fake door, which would have disappointed vulnerable users and used their data without consent, so I replaced it with a concierge test: steady plans hand-built for a small group who agreed to take part, with a stop rule that returns the budget to the board if it fails. Key learnings: I will lead a hard no with the risk to the people we serve, not our capacity, because a capacity reason invites an offer of capacity. I will write the kill line before a bet starts, with a metric, threshold, deadline and consequence that nobody who benefits from the bet can lift. And when one decision changes, I will read across every decision that rests on it, with a second model as a cheap reviewer. Aha moment: When both models asked whether people who have recovered want an ongoing relationship at all, I saw that some of Fable's churn is healthy. That moved the strategy from spotting dips to a nightly wind-down people choose, and made KR3 ask whether users feel steady without feeling dependent, so Fable can't win by keeping people anxious.

Review it in three short paragraphs:
1. Could you tell where they will play, how they will win, and what they are refusing to do? Name anything that still reads like a wish list.
2. Do the roadmap, the charter, the stakeholder message and the kill criterion follow from that strategy? Say which one is the weakest.
3. The one change that would make this presentation stronger before it is submitted.

End with one line: "Ready to submit" or "Needs another pass", and why.
```

**How the two replies compared** · both replies, word for word: [3-board-review-revised.md](06-final-presentation/ai-replies/3-board-review-revised.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | Needs another pass: the financial case and the thresholds for continuing | Needs another pass: the roadmap is hard to read, and recruiting churned users contradicts in-app reach |
| Strongest part | Seeing that some churn is healthy | KR3, "steady without feeling dependent" |
| Wish list | The moat is an aspiration; four Later bets compete | The aspiration's "the moment they feel things slipping" implies Fable spots a dip; the upgrade path sits outside "premium first" |
| Weakest part | The business case: the assumptions aren't shown to be credible on their own | The roadmap as read: bets, owners and measures in separate lists, and Next's measures tied to no item |
| Numbers | The 45% build-stage line sits well below KR1's 55% | They add up ($7.4M, 2.3x at 70%); 15 people paying again is thin; the $7.4M credits the whole KR1 lift to the steady plan |
| The one change | A bridge from each test result to the investment decision it unlocks | One row per bet, and no course references ("both models", "Section 5", "backlog #6") |

- **The first round's fixes held:** neither repeated the sample-size gap, the $155 misreading or the employer offer, and Claude checked the arithmetic and found it adds up.
- **Claude found the one new contradiction:** Where to play says "reached inside the app", but Bet 1 invites 500 churned users, who can only be reached by email, a channel the charter gives to Growth.
- **Diminishing returns:** most of what's left is how the presentation reads, and the builder causes part of it by laying the roadmap table out column by column. GPT-6's remaining points are answered in the deliverables (the moat is called potential) or need Fable's own data.

### 4. Board review of the submitted presentation · new memory-off chats in both models

The same builder prompt, filled from the submitted [final-presentation.html](final-presentation.html), so its text matches that file rather than being repeated here. A last check under one rule: act only on a contradiction or an arithmetic error.

**How the two replies compared** · both replies, word for word: [4-board-review-final.md](06-final-presentation/ai-replies/4-board-review-final.md)

| Point | GPT-6 | Claude |
|---|---|---|
| Verdict | Needs another pass: the financial case needs reconciling | Needs another pass: the pitch contradicts the hard no, and the kill criterion stops too much |
| Strongest part | Seeing that some churn is healthy | The charter |
| Numbers | Asks for the $7.4M chain to be reconciled | Checks it: $7.4M, 2.3x at 70%, break-even near 41% |
| Contradiction found | None | The pitch's "the community layer waits" against Module 1's "will not build" |
| Other points | The 45% line unexplained (it is explained); Later dilutes the bet; an evidence-to-investment bridge | A regulatory no on self-checks stops the whole plan; the buddy trigger only works between 45% and 55%; PM 2's load; the upgrade and annual items have no KR |

- **Claude found the one real contradiction left:** the pitch, the first line a board reads, says the community layer "waits", while Module 1, the trade-off memo and the Growth message all say it won't be built. The same sentence is the README's strategy sentence.
- **The arithmetic holds:** Claude checked it, and GPT-6's call to reconcile it found no error. GPT-6 also missed the 45% line's explanation, which is in the file.
- **The kill-criterion points are judgement, not error:** a regulatory no on a product that changes that much needs a new business case, which is what the stop line asks for; and the Growth message says the buddy test runs "only if" retention is flat, a condition, not a promise.
