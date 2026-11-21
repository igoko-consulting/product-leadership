# Module 1 notes: strategy and OKRs

16 Nov 2026. Sources: module 1 of Product School's Product Leadership course. Scenario: [README](../README.md#the-scenario-fable-growth). Output: [strategy-and-okrs.md](strategy-and-okrs.md). Each point ends with my own critique, marked "Missed:".

## From PM to product leader

- **Four shifts:** bets over features (where to compete, not what to ship); direction over execution (setting the plan, not running someone else's); insights over analysis (choosing which questions are worth answering); scope over ownership (deciding across teams, not within one area). Missed: the shifts are less clean in practice. A group PM still executes the CEO's plan and still ships; what changes is being accountable for the trade-offs between teams, and for the people making them, which Module 3 picks up.
- **The strategy hierarchy:** vision (who we serve, what problem, why now) sets strategy (how we create value, stand out and make money), which sets the roadmap (what, which team, by when), which sets execution. Vision rarely changes; execution changes weekly, and what it learns feeds back up. Missed: the feedback loop is where most organisations break. The roadmap moves weekly while the strategy is reviewed yearly, so the two drift apart without anyone deciding they should. A strategy needs its own revisit trigger.

## Testing the vision

| Test | Question | Course example |
|---|---|---|
| Market timing | Why now: what changed in the last two or three years? | Zoom launched in 2013 and became the default in 2020 |
| Competitive position | Why us: what do we understand that competitors missed? | Figma built for designers, PMs and engineers in one browser file |
| Org readiness | Why us, now: can this team start today? | A 12-person team can own one city, not the world |

- **All three, not one:** a vision that passes "why now" but fails "why us, now" is someone else's opportunity. Missed: the "why now" examples are hindsight, and Zoom's timing was as much luck as insight. A forward-looking answer names the change and the signal that shows it is happening, not an analogy.

## Six steps to a strategy

- **Vision, insights, challenges, approaches, accountability, share early:** one sentence on what every team optimises for; a point of view from competitors, gaps and shifts; the real obstacles; where to play, how to win and what not to do; OKRs with owners and review dates; and sharing before it feels finished. Missed: step 3 is the one most strategy decks skip. It is Rumelt's diagnosis in *Good Strategy Bad Strategy*, and the course's line that a strategy is only as good as its diagnosis comes from the same place. If the challenge isn't uncomfortable to say aloud, it probably isn't the real one.

## The Playing to Win cascade

| Choice | What it decides |
|---|---|
| Winning aspiration | What winning looks like for the customer |
| Where to play | Segment, geography, channel and use case, and the ones left out |
| How to win | The advantage competitors can't easily copy |
| Capabilities required | What we must be excellent at, and whether we build, buy or partner |
| Management systems | The metrics and reviews that keep it on track each quarter |

- **Each answer supports the one above:** if two contradict, the strategy has a gap. Where to play should name a specific user with a specific job in a specific moment, not a market; if an answer runs to paragraphs, no choice has been made. Missed: the course runs the cascade top-down, as a form. Lafley and Martin describe it as a loop: where to play and how to win are set together, and capabilities often cut the aspiration back. Expect to rewrite the aspiration after the capabilities row.
- **Figma versus Adobe XD:** Figma's five choices reinforced each other around one shared browser file, with free viewer seats widening the team that used it. XD's aspiration was keeping designers inside Creative Cloud, and each capability was added to catch up; Adobe stopped developing it in 2023. Missed: XD wasn't only an incoherent strategy losing on merit. Adobe had agreed to buy Figma in 2022, so XD's end was also a corporate call made around a deal that regulators later blocked. Coherence explains Figma's win; it doesn't fully explain XD's exit.
- **Two more lenses:** Jobs to be Done (what progress is the customer trying to make, functionally, socially and emotionally) when a team argues over features or personas; platform versus product (win alone, or let others build on us) when deciding how open to be. Missed: JTBD is most useful inside the cascade, not beside it. It is how to write a where-to-play answer that names a job and a moment rather than a demographic.

## From strategy to execution

- **OKRs measure outcomes, not delivery:** "ship the readiness model by Q2" says the team shipped; "race-week retention 34% → 62%" says athletes changed behaviour, which is what the strategy promised. The chain runs strategy → OKRs → roadmap → execution. Missed: the course's own example KR2, "readiness-model opens per user 1.2 → 4.5", sits closer to activity than outcome. Opens can rise because the model confuses people. Pairing a usage KR with a quality or guardrail KR closes that gap, and it is exactly what the pressure-test's "outputs disguised as outcomes" question is looking for.
- **Deciding with incomplete data:** name what is known (undisputed facts, everything else an assumption); sort the unknowns into those research can answer soon and those to accept; check reversibility and match effort to it; make a provisional bet and name the metric, signal or date that would reopen it. Missed: this is one-way and two-way doors with a trigger attached, and the trigger is the step people skip. It is also Module 5's kill criterion in early form, minus the financial consequence.
- **The six-question check:** clear enough that a new PM knows what we will and won't do; names the real challenge; makes a hard bet by saying no to something valuable; cascades into each team's OKRs; actions that would suffer if one were removed; and funded, with budget and people moving. Missed: "is it funded" is the one a product leader often can't answer alone, and it is the first question a board asks. A strategy that fails it is a proposal.

## AI as a strategy co-pilot

- **Three uses:** monitoring competitors' moves as they happen; synthesising market, competitor and customer signals; and stress-testing the strategy by having AI argue as the CFO or the biggest competitor. The call stays with me. Missed: a model told to be sceptical will always find something, so the value is in which challenge I accept and why, which is what the lab's last step asks for. Running two models with the same prompt shows which challenges are the prompt's framing and which are real.

## Labs

### Lab 1 · One-page strategy

- **Chosen, stay steady:** Fable keeps users after the hard stretch by turning what helped them into a steady plan and check-ins that spot an early dip (revised after the pressure-test: see Lab 2). It answers the brief's real competitor, the user deciding they don't need Fable, with the one thing only Fable has: their history. Missed: it assumes recovered users want ongoing support at all. Some of this churn may be healthy, and the pressure-test should go there first.
- **Rejected, come back first:** accept low use between hard stretches and let premium pause rather than cancel. Missed: it may be the more honest read of how people use wellness apps, but a pause option strains the existing subscription model and gives up revenue between stretches.
- **Rejected, a daily habit for everyone:** it fights Headspace and Calm on their own ground and reads as a wish list.
- **Hard no, the community and social layer:** no posting between users, groups or profiles. It serves connection rather than staying steady, brings safeguarding work a team of 14 can't staff, and would split the team before the bet is proven. Module 4 later led with the risk to people instead, since a capacity reason invites an offer of capacity. It also sets up Modules 3 and 4, where the Growth team is one side of Module 3's tension and the Module 4 stakeholder. Missed: social ties are the strongest general retention lever, so a one-to-one buddy experiment runs only if KR1 plateaus once the steady plan is live (Module 2's Later column).
- **Not the hard no, but still a no, CBT programmes:** a multi-week course ends, recreating the 90 to 120 day cliff, and sits close to treatment. Short CBT-informed exercises can live inside steady plans, which keeps the clinical team involved. The content team's role becomes re-sequencing the existing library rather than adding to it.

### Lab 2 · OKRs and pressure-test

- **First OKRs:** KR1 was the money (day-180 premium retention of users who engaged deeply in their first 90 days), KR2 the behaviour (weekly use from day 90 to 180), KR3 the "notices early" half of how to win (returning within 48 hours of a check-in dip). Missed: the scenario gives no retention figures, so every baseline is my estimate.
- **What the pressure-test found:** both models' first point was the one I had flagged: recovered users may not want, or pay for, an ongoing relationship. Claude added that detecting when someone is slipping could make the check-in a medical device, against the first constraint. In the harsher round, both found nothing to open Fable for on an ordinary day, while rivals own sleep as a nightly habit. Comparison: [PROMPTS.md](../PROMPTS.md#module-1--product-strategy-and-okrs); replies: [pressure test](ai-replies/1-pressure-test.md), [harsher follow-up](ai-replies/2-harsher-follow-up.md).
- **What changed:** the steady plan is built around a nightly wind-down, for post-acute users who still use sleep content; a self-check the user starts replaces dip detection; KR1 counts monthly plans only, since annual plans are prepaid; KR2 counts nights with a wind-down; KR3 asks whether users feel steady without feeling dependent. Missed: leaning on sleep moves Fable onto Calm's strongest ground. The defence is a plan that is personal from the first night.
- **What I defended:** the hard no, since neither model argued for posting, groups or profiles, and the focus on existing users. Missed: three of the four replies named social ties as the hardest thing for a rival to copy, so a one-to-one buddy experiment became a gated Later bet in Module 2, run only if KR1 plateaus once the steady plan is live.
- **Later changes from Module 2:** the capabilities now say rules-based first and AI only once it lifts retention; How to win calls the acute-level evidence a moat it can become, not one it has; the KRs are dated month 12. Missed: each change came from a model's review of the roadmap, which shows a strategy worth revisiting after the plan beneath it is drawn.
- **Changes from the Module 6 board review:** the KRs now name their cohorts (those reaching day 90 by month 12, read by month 15), since "by month 12" read as a month-12 result; and Where to play dropped the 25–45 age band, which is Fable's whole market rather than a choice and never appeared again. Missed: GPT-6 read the age band as useful context, so dropping it was the closer of the two calls. The second review changed the aspiration's "the moment they feel things slipping", which implied Fable spots a dip, to "the moment they reach for it", and Where to play now says churned deep users are reached only by a Growth email inviting them to the concierge test. Replies: [first review](../06-final-presentation/ai-replies/2-board-review.md) · [second review](../06-final-presentation/ai-replies/3-board-review-revised.md).
- **Carried forward:** the demand test and the regulatory opinion became Module 2's Now Bet 1, with a stop rule; the demand test started as a fake door and became a concierge test. Module 5 gets the monthly versus annual plan mix, and an LTV case against the cost of 14 people for a year.
