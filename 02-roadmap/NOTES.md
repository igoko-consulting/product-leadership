# Module 2 notes: Turn Your Strategy into an Outcome Roadmap

Session 2, 16 Nov 2026. Sources: Module 2 slides and Lab Guide. Builds on: [Module 1's strategy and OKRs](../01-strategy/strategy-and-okrs.md). Output: [outcome-roadmap.md](outcome-roadmap.md).

## Rocks, pebbles and sand

| | What it is | Typical work |
|---|---|---|
| Rocks | Strategic bets that move the north star; if they don't ship, the strategy fails | New core capability, platform foundation, architecture bet |
| Pebbles | Customer-requested improvements and delight; they build trust and fill gaps | Key feature request, onboarding improvement, integration |
| Sand | Maintenance, tech debt and polish; necessary, but it fills every gap if allowed | Bug fixes, tech debt, UI polish, performance |

- **Put the rocks in first:** most teams fill sprints with sand and wonder why the rocks never ship. Stripe's rock was API reliability and docs, Notion's the block editor, Linear's speed. Missed: the categories describe the kind of work, not its role. Performance is sand for most products and was Linear's rock. The test is whether the strategy fails without it, which is why two of Fable's rocks are fixes.

## Choosing a prioritisation framework

| Framework | Use it when | How it scores |
|---|---|---|
| Impact vs. Effort | A first sort of a whole backlog | Four boxes: Do Now, Plan Carefully, Fill Gaps, Avoid |
| RICE | Impact vs. Effort leaves too many items in one box | (Reach × Impact × Confidence) ÷ Effort, confidence 50–100% |
| WSJF | Waiting has a cost | (Time criticality + Value + Risk reduction) ÷ Job size |
| Weighted scorecard | Several teams must agree | Agreed criteria and weights first, then every item scored the same way |

- **Impact vs. Effort with a correction:** score 1 to 5, then double effort and halve impact, because teams overrate one and underrate the other. Missed: a uniform correction doesn't change the ranking, only which items cross into Do Now. Its real use is stopping an overfull Do Now box.
- **RICE adds reach and confidence:** Missed: confidence is the easiest input to game. Tie it to the type of evidence (data, research, opinion) rather than to how sure the team feels.
- **WSJF prices delay:** Missed: Fable's WCAG gap is the WSJF case. Legal risk grows while it waits, so it ranks higher there than on Impact vs. Effort, which is why it gets a date outside the rocks.
- **A weighted scorecard settles cross-team arguments:** Missed: the weights are the strategy in disguise. Agree them before any item is scored, or each team tunes the weights to favour its own items.
- **The other tools:** MoSCoW for sprint and MVP scoping (Must Have overloads when strategy is unclear); Now/Next/Later for stakeholder communication (a wish list if not tied to OKRs); Feature ROI for financial cases (needs revenue estimates early products lack); Buy a Feature for alignment workshops (customers pick comfort over strategy); affinity grouping for discovery (too slow for single-feature calls).
- **Pick the framework for the decision:** Missed: all of them rank a list someone else wrote, and none asks whether the list holds the strategy's rock. Fable's backlog has no steady plan, only a check-in item that has to be reframed to fit. Checking the backlog against the strategy comes before scoring it.

## Building a roadmap that keeps trust

| View | For | Shows |
|---|---|---|
| Outcome-based | CPO or board | The bets and outcomes committed to, not features |
| Now/Next/Later | The team and stakeholders | Priority and confidence, without dates |
| Timeline | Engineering and operations | Release order, dependencies and dates |
| Opportunity-based | Product and design | Customer problems to explore, not set solutions |
| OKR-linked | Anyone checking against the strategy | Which OKR each piece of work moves |

- **One roadmap, several views:** each audience asks a different question: bets for the board, priorities for the team, dates for engineering. Missed: these are views of one source, not five documents. Keeping one source is what prevents the hidden and stale failures below.
- **Now/Next/Later sorts by certainty, not date:** Now is committed (up to three, each "We bet [action] will [outcome] for [who]", linked to an OKR); Next is planned (up to five, each with why it comes after Now); Later is possible (matters, but has no people or budget yet). Missed: a committed Now bet with no stop rule stays in Now forever. Module 5's kill criterion is that rule.
- **Four ways a roadmap loses trust:** hidden (fix: one version anyone can find), stale (fix: one owner, reviewed every sprint), over-promised dates (fix: a date only when you'd stake your credibility on it), feature factory (fix: every item a bet linked to an OKR before it gets people or budget). Missed: reviewing every sprint can churn a board-facing view as badly as staleness. The team view moves each sprint; the board view moves each quarter.

## Labs

### Lab 1 · Backlog audit

The Lab Guide's 14 Fable items, word for word with who asked, scored 1 to 5 for impact on the Module 1 objective ("Make Fable the app people keep after the hard stretch passes") and for effort, after the lab's correction. High is 3 or more. The item text keeps the course's spelling, since rocks and hard nos go into prompts as written.

| # | Item | Asked by | Impact | Effort | Quadrant | Why |
|---|---|---|---|---|---|---|
| 4 | Fix the notification system (wrong times, timezone bug) | Engineering | 4 | 1 | Do Now | The nightly wind-down depends on reminders arriving at the right time |
| 14 | Reduce app load time from 4.2s to under 2s on 4G | Engineering | 3 | 2 | Do Now | A slow load at bedtime is a reason to give up |
| 6 | Add AI-generated daily check-in prompts personalized to user history | Product | 4 | 3 | Plan Carefully | The core of the steady plan, if the user starts it |
| 11 | Add Apple Watch integration | 3 partnership requests | 3 | 4 | Plan Carefully | A wind-down without the phone, but only Watch owners benefit |
| 2 | Add a daily streak feature to drive habit formation | Growth team | 2 | 1 | Fill Gaps | Rewards daily opens, against KR3's "without feeling dependent" |
| 10 | Close the WCAG 2.1 accessibility compliance gap flagged in an audit | Legal | 2 | 2 | Fill Gaps | A legal commitment with a date, not a rock |
| 1 | Redesign the onboarding flow based on 40% drop-off data | Product analytics | 2 | 3 | Avoid | Helps new users, not post-acute ones |
| 3 | Build a social layer: share your progress with friends | User research | 2 | 4 | Avoid | The Module 1 hard no |
| 5 | Launch a premium tier with therapist-matching | CEO | 2 | 5 | Avoid | Crosses the clinical line and serves the acute phase |
| 7 | Localize the app into Spanish and Portuguese | Sales (LATAM) | 1 | 3 | Avoid | New markets |
| 8 | Build a web version (frequently requested in reviews) | Community | 1 | 4 | Avoid | The wind-down happens on a phone in bed |
| 9 | Create a "crisis mode" flow for acute anxiety moments | Clinical advisor | 1 | 3 | Avoid | Acute phase and clinical; the signposting partner covers it |
| 12 | Build a content library: guided meditations, articles, audio | Content team | 1 | 4 | Avoid | Module 1 chose to re-sequence the library, not add to it |
| 13 | Introduce "Fable for Teams", a B2B workplace wellbeing offer | Business development | 1 | 5 | Avoid | Employers are outside Where to play |

- **Rocks: #6, #4, #14.** #6 is the strategy's core capability, built as the self-check and steady plan the user starts. #4 and #14 are what the nightly habit breaks on: reminders at the wrong time and a slow load at bedtime. Missed: the course's jar slide calls bug fixes and performance "sand", so two of the three rocks are maintenance by its own definition. The defence is that the nightly habit is the strategy; Linear made speed its rock for the same reason. Apple Watch (#11) was the bolder third rock, turned down because it costs more and reaches fewer users.
- **Hard nos: #5, #3, #2.** One from each camp: the CEO's therapist-matching tier (the one that's hard to give up), user research's social layer (the Module 1 hard no), and the Growth team's daily streak (against KR3). Missed: Growth loses twice, which sets up Module 3's tension with the Growth lead but risks half-hearted execution, so the roadmap gives the Growth team a share of Rock 2 (see Lab 2).
- **Not chosen either way:** WCAG (#10) is a legal commitment to schedule with a date, outside the rock count. Fable for Teams (#13) was the alternative third hard no; it stays a Later candidate once outcome evidence exists.

### Lab 2 · Roadmap

- **The prompt:** run word for word in both models, filled from the Module 1 strategy and OKRs and the three rocks: [PROMPTS.md](../PROMPTS.md#module-2--outcome-roadmap). Replies: [1-roadmap.md](ai-replies/1-roadmap.md).
- **Chosen, Claude's roadmap:** Now tests demand before anything is built (a fake door for churned deep users plus the regulatory opinion, with a stop rule; the fake door later became a concierge test), alongside the two bedtime fixes; Next builds the steady plan, self-checks, consent model and signposting only once that passes. GPT-6's Now built the plan straight away, the gap both models had criticised in Module 1, and its Next and Later drifted towards structured journeys and new users. Missed: GPT-6's explicit day 90–120 transition is a good idea that Claude's "steady plan v1" only implies.
- **Two edits:** the Growth team co-owns Bet 2, the bedtime reminders, as lifecycle messaging, so the team that lost two hard nos is inside the bet; and Rock 1's memo line now leads with what it is, the steady plan and the self-check, because the backlog item's name describes the monitoring Module 1 ruled out. Missed: Growth inside the bet softens the cross-team tension Module 3's charter has to settle.
- **The three review questions:** every Now item reads as a bet, yes; each traces to an OKR, yes; a stranger would know the problem this quarter, mostly, since "post-acute" and "churned deep users" are jargon. Missed: the jargon matters more in Module 4, where the message goes to someone outside the team.
- **Reviews of the final roadmap, GPT-6's fixes:** both models reviewed the final table in the same chats ([replies](ai-replies/2-final-roadmap.md)), and all ten fixes were taken. GPT-6's: denominators and a paid rejoin for Bet 1, outcomes ahead of the delivery guardrail for Bet 2, a rules-based steady plan before AI personalisation, a stronger condition on the employer offer, and Now proving demand, Next behaviour, Later value. Missed: the rules-based first version quietly moves the "AI" out of backlog #6, which Module 5's business case should cost honestly rather than assume.
- **Claude's fixes:** a KR3 mid-point, one lead team per item, a signal for every Later bet, and a footnote that Growth, Legal/Privacy, Data/Insights and Commercial are shared services, not new hires. Between them the two removed the last clinical wording, "relapse-reduction" and "tips into crisis". Missed: shared services answer to other teams too, so Module 3's charter has to say how much of their time the initiative gets.
- **The visual:** Claude's one-slide version goes into Module 6, since [GPT-6's](ai-replies/3-visual-gpt6.png) drops the employer bet. Claude redrew it from the refined table, and one follow-up renamed a card title the redraw had left clinical. Final: [PDF](ai-replies/3-visual-claude.pdf) and [PNG for the builder](ai-replies/3-visual-claude.png); earlier versions: [v1](ai-replies/3-visual-claude-v1.pdf), before the ten fixes, and [v2](ai-replies/3-visual-claude-v2.pdf), before the concierge test. Missed: both models invented per-card owners in their first visuals, and a redraw that says it changed everything still needs checking line by line.
- **Aligned with Module 1 before Module 3:** Rock 1 supports KR3 and KR1, as Bet 1 does; Bet 1 separates who tests demand from who gets the product; the buddy experiment has one condition everywhere, only if KR1 plateaus once the steady plan is live. Missed: three conditions for one feature had crept in across two modules, which is what a terms list and a consistency pass are for.
- **Fake door swapped for a concierge test:** the fake door showed people who left after a hard stretch an offer for something that didn't exist, used their wellbeing history before any consent model, and couldn't fairly charge for an unbuilt feature. Now the content team hand-builds a nightly wind-down from each person's history for a small consenting group of churned and current day 60–120 users, which tests demand, nightly use and willingness to pay at once, and is the re-sequencing role Module 1 gave the content team. Missed: a concierge test doesn't scale, and hand-picked plans may beat what a rules-based v1 can do, so its results are an upper bound for sizing the build.
- **Owners named after Module 3:** where the roadmap said "Product", it now names PM 2 or PM 3 as the Module 3 charter decides, and the buddy experiment moved from Growth to PM 2, since it aims at KR1 in the post-acute experience PM 2 owns. Missed: the slide still says "Product" at team level, which holds, except the buddy card's lead order, updated separately.
- **Placeholders:** the success-signal thresholds (30% opt-in, 35% using the wind-down three or more nights a week, 10% paid return, 98% of reminders on time, opt-outs down 30% relative, KR3 at 50% by month 6) are starting points, not Fable data. Module 5 sets them against baselines.
