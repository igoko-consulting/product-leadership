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
