# Module 3 notes: Set the Habits That Make a Team Faster

Session 3, 16 Nov 2026. Sources: Module 3 slides and Lab Guide. Builds on: [Module 2's roadmap](../02-roadmap/outcome-roadmap.md). Output: [team-charter.md](team-charter.md).

## From PM to leader of PMs

| Stop | Start | Continue |
|---|---|---|
| Solving the problem yourself | Giving context others can act on | Staying close enough to see when someone needs help |
| Writing specs to prove you understand | Building your PMs' judgement | Caring about the product outcome |
| Measuring yourself by what you shipped | Naming what good looks like before work begins | Keeping your own product thinking sharp |
| Attending every product meeting | Measuring yourself by what your team produces | |

- **The hardest part is stopping habits that still feel like the job:** Missed: "keep your own product thinking sharp" and "stop solving the problem yourself" pull against each other. The line I hold is to think about the problem in the open, as questions, rather than hand over the answer, or PMs learn to wait for it.
- **The player-coach dial:** between the over-player (still doing the IC work, and the bottleneck) and the over-coach (so hands-off the team is alone) sit four modes, chosen per person and per task: Direct for a new person on a new task, Coach at someone's growth edge, Support on complex or unclear work, Delegate where they are strong and experienced. The same PM can need Direct on a new strategic problem and Delegate in their own area. Missed: this is situational leadership by task, and the usual failure isn't picking the wrong mode but not saying which one you're in, so Direct gets read as distrust. For Fable, PM 3 needs Support through the charter change, not Delegate.

## Leading people through performance

- **Four questions before giving feedback:** have I actually been clear; have I let this go on too long; is this their behaviour or a decision I made; am I doing this to help them or to ease my own discomfort? Missed: the third question applies to the charter. PM 3's layer becoming a shared platform is my decision, so any friction that follows is a clarity or system problem first, not a feedback one.

| What you see | Type | What to do |
|---|---|---|
| The behaviour continues though expectations are clear | Feedback problem | Specific, timely feedback with SBI |
| Expectations, ownership or decision rights were never explicit | Clarity problem | Write down what you expect and who decides |
| Expectations are clear and feedback lands, but something blocks them | System problem | Fix the blocker before addressing the behaviour |
| The gap remains after clear feedback, explicit expectations and removed blockers | Hiring mismatch | Talk about role fit, early and directly |

- **Diagnose before acting:** most situations that feel like feedback problems are clarity or system problems. Missed: the types stack over time. A clarity problem left long enough looks like a feedback problem to the person, who has been "failing" without knowing, so work through them in order: system, clarity, then feedback.
- **SBI, plus a question:** situation (specific and recent), behaviour (observed, not interpreted), impact (on the team, product or relationship), then an open question to invite their side, ideally within 48 hours. The two mistakes are withholding (they fill the silence with their own story) and blurting (months of frustration over a small incident). Missed: impact is the part most easily overstated. "Engineering spent two days on the wrong brief" is observable; "you damaged trust" is interpretation and starts an argument.
- **Five steps for a performance gap:** real-time SBI (most skipped), a separate state-of-the-relationship conversation (most feared), a written shared understanding of what changes, by when and with what support (most avoided), a check-in on a date agreed in the conversation (most delayed), and a formal PIP only as a last resort. Missed: in the UK and much of the EU, steps 3 to 5 sit inside a formal capability process, so HR should see the written understanding before a PIP, not at it.
- **Your strongest person is often the most at risk:** they take the hardest problems and rarely say they're struggling; watch for lower energy, shorter replies and less initiative. Recognise the specific behaviour as well as the outcome, in public, and give more scope before they ask. Missed: public recognition doesn't suit everyone. Asking how someone likes to be recognised costs one question.

## Creating the conditions for great work

| Structure | Example | Optimises for | Trade-off |
|---|---|---|---|
| Outcome-oriented | Spotify squads | Ownership and accountability | Work can be duplicated across teams |
| Feature-oriented | Amazon two-pizza teams | Speed and clear scope | Keeping the product coherent is harder |
| Platform + product | Airbnb platform team | Shared infrastructure, fewer dependencies | The platform layer moves more slowly |
| Small outcome team | Linear | Trust, few layers and speed | Coordination costs grow as teams are added |

- **Every structure is a bet:** choose it on purpose. Missed: Fable's charter makes a platform-and-product split, with PM 3's AI layer serving PM 1 and PM 2, so the trade-off to watch is the platform moving slower than retention needs. The joint sign-off on self-check wording is where that will show first.
- **Five decisions before hiring** (from Nikhil Singhal, Meta): direction (is the strategy clear enough to execute, or does this person help set it), growth stage (0-to-1 builder, 1-to-10 scaler or 10-to-100 optimiser), market (new insight or applying existing insight), team (the structure they join) and organisation (how influence really works). Missed: for Fable the stage question matters most. The steady plan is 0-to-1 work inside a 10-to-100 company, and a scaler hired now would optimise the wrong thing.
- **A charter specific enough to test:** four parts, What We Own, How We Decide, What Success Looks Like and How We Work, each written so a new PM could act on it on day one ("we own onboarding through day 30", not "the core app experience"). Missed: the lab asks only for the first two. For Fable, success already exists as the Module 1 OKRs, while How We Work is unwritten, and that is where the PM 3 tension will actually be lived.

## Labs

### Team charter

- **The tension to settle (from the Lab Guide):** I own the core Fable product across a team of 14. PM 1 owns onboarding, PM 2 owns retention, and PM 3 owns the AI check-in layer, which touches both. The Growth team also has a stake. Who owns what, and who decides when they overlap? Missed: the roadmap puts almost everything in retention and in PM 3's layer (the steady plan, self-checks, the route back), while onboarding (PM 1) has little in it, so the real overlap is PM 2 against PM 3, with Growth co-owning the bedtime reminders.
- **The prompt:** run word for word in both models, filled from the scenario, the Module 2 roadmap table and the tension: [PROMPTS.md](../PROMPTS.md#module-3--team-charter).
- **Chosen, Claude's charter with six edits:** it settles the overlap the tension asks about. PM 2 owns the post-acute experience and is accountable for KR1–KR3, PM 1 owns days 0 to 60, and PM 3's AI layer is a shared platform whose output after day 60 is PM 2's call. GPT-6's draft split "the post-acute experience" from "the broader retention lifecycle", which would start the arguments a charter should stop. Missed: making PM 3's layer a shared platform that PM 2 directs can feel like a demotion, so that conversation comes before the charter is shared.
- **The six edits:** the bedtime reminder is shared with Growth, as Module 2 decided; Fable never starts a check-in, as Module 1 decided; shared-service time is agreed with Growth, Legal/Privacy and Data/Insights each quarter, closing Module 2's gap; "I" becomes the Fable product lead, a named role; "crisis response" becomes "urgent support"; and conflicts with Growth go to the CPO, from GPT-6's draft, since the product lead can't overrule a peer team. Missed: both models drifted from earlier decisions in a draft that read well, which is why each line is checked against the modules before it is kept.
- **The three review questions:** every line names a team, role or product area, once "I" became the Fable product lead; What We Own says what is out of scope and which calls are joint; and the escalation path says who decides, how and by when (a one-page note, three working days to settle, then the Fable product lead or the CPO within two). Missed: a charter this specific needs revisiting whenever the roadmap moves work between PMs, or it goes stale like the roadmaps Module 2 warned about.
- **What Module 4 takes from it:** the Growth lead is the other side of this tension. They own lifecycle messaging and acquisition, share the bedtime reminder, and lost the daily streak and the social layer in Module 2, so the hard no for Module 4 goes to them.
- **Aligned before Module 6:** the product lead can no longer override a kill criterion; only a new business case to the board can lift one, as Module 5's case requires. Missed: it takes power from my own role on purpose, since the course asks for a kill line someone outside the team could enforce.
- **Aligned with Modules 1 and 2 before Module 4:** PM 3's layer is a shared platform, since "shared services" already meant the teams outside the 14; the employer offer stays out of scope until retention and willingness to pay are proven, the roadmap's own condition, instead of "not this year"; and the roadmap now names PM 2 or PM 3 wherever the charter decides the owner, including PM 2 leading the buddy experiment instead of Growth. Missed: once the roadmap names people, it doubles as a staffing plan, so every later roadmap change has to be checked against the charter as well.
