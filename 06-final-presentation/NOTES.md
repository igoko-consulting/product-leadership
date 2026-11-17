# Module 6 notes: Lead the Team That Builds with AI

Session 6, 17 Nov 2026. Sources: Module 6 slides and Lab Guide, my CV, my CLAUDE.md and existing skill files. Builds on: the decisions in Modules 1 to 5. Output: [leadership-skill-file.md](leadership-skill-file.md) (practice), then the final presentation.

## From AI user to AI leader

| Stage | What the leader does | Course example |
|---|---|---|
| Personal productivity | Uses AI to move faster on their own work | A rough idea becomes a PRD draft in minutes |
| Team capability | Sets how the team adopts, checks and trusts AI | Every PM writes PRDs to the same prompt, so quality holds |
| Org advantage | Makes AI bets that compound across the organisation | PRDs feed one shared source of truth |

- **Most of a leader's impact is in Stages 2 and 3:** using AI well yourself is table stakes; setting the standard the whole team's AI use meets is the leadership work. Missed: Stage 3 needs a shared system someone maintains. In a matrix organisation that system has no natural owner, so it decays unless it is run like a product with its own owner.
- **Where AI earns its place:** five areas where one standard for everyone beats each PM's own habit. A strategy pressure test run the same way; a hard cut built so whoever holds the line can defend it; AI themes the feedback but the leader still has the conversation; pre-reads and objections built the same way; business cases stress-tested before finance finds the weak point. Missed: a shared prompt raises the floor, not the ceiling, and the strongest PM's work can get worse when forced into the template. My version in this repo is the same prompt in two models, not one prompt for everyone.

## Leading a team that builds with AI

| Condition | The action | Course example |
|---|---|---|
| Norms | A one-page rule for which tasks ship on AI output alone and which need a person's review | A dealership chatbot agreed to sell a car for one dollar; nobody had set what it could commit to |
| Risks | Name one skill AI won't absorb, and have the team do those reps by hand | A team's prompt slipped when the model changed, and nobody could spot it any more |
| Culture | One name against every AI-assisted deliverable | A tribunal made Air Canada honour a refund policy its chatbot invented |

- **Set the conditions, then step back:** a team that knows the rules doesn't need the leader reviewing every output to stay safe. Missed: the eroded-skill case is also an argument for evals. A regression test on the prompt would have caught the model change; manual reps fade, tests don't.

## Governing AI bets

| Path | Choose it when | The moat test |
|---|---|---|
| Build | The capability is close to what makes you different | Name the data, talent or context a competitor starting today couldn't assemble |
| Buy | It's table stakes and moving now matters more than owning it | Name the first-mover advantage a later buyer of the same tool can't take back |
| Partner | Your edge is integrating depth you can't build | Name what your integration gives customers that the partner alone can't |

- **Four costs that change after you commit:** infrastructure grows with usage, so success raises the bill; the vendor's pricing, uptime and roadmap become your risk; models change under you, so a capability that cleared the bar can slip below it; and if your usage trains the vendor's model, you fund a capability rivals can rent. Missed: this is build versus buy from my skill file in AI form. For AI, the cost of buying is rarely the licence. Fable's "rules-based first, AI only once it lifts retention" (Module 1) avoided all four until the lift is proven.
- **Kill criteria for AI bets:** Module 5's four steps, harder to keep because demos excite and models keep changing. A metric and a target, not a demo; the threshold and read date in writing before launch; a fixed review window that asks whether you'd still fund it today; and the number that ends it, with who must agree, decided in advance. Missed: "would you still fund it today" can become a way to keep a bet alive. The stop line has to stay fixed, which is why Fable's can only be lifted by a new business case to the board.
- **Trust, explainability and bias are product questions:** when it is confidently wrong, does the product catch it or the user; can we trace why it did something, or only that it did; who does it work worse for, and would our metrics show it. Missed: for Fable these sit in the self-check. A confident wrong read of someone's state is the medical-device risk the Module 1 pressure test found, which is why Fable never starts a check-in. Averages also hide bias, so the KR cohorts need cutting by plan type and age.

## Labs

### Leadership skill file (practice)

- **How the prompt was filled:** the Lab Guide's prompt with my context, standards and VP, checked against my CV, CLAUDE.md, existing skill files and Modules 1 to 5 before running. The Booking.com timing was fixed and the doubled full stops removed. My three calls: keep all six standards (70%), add the leads of the teams that use my platform as a second stakeholder (65%), and push back when my call breaks one of my standards or I can't show the cost of a yes or a no (75%). Prompt and comparison: [PROMPTS.md](../PROMPTS.md#1-leadership-skill-file--new-memory-off-chats-in-both-models). Missed: the Lab asks for two or three standards, and six makes a longer file to keep current.
- **What the models did:** both kept every standard, the six calls I never hand off and both stakeholders, and neither invented anything. Both cut the examples to fit the 700-word limit I set. Claude flagged three vague standards as asked; GPT-6 flagged none in its file and said it was under 700 words when it was about 740. Replies: [both files and chat replies](ai-replies/1-skill-file.md). Missed: a model told to meet a word limit cuts the specific before the generic, which is the opposite of what a skill file needs.
- **The final file, Claude's base with the examples back:** [leadership-skill-file.md](leadership-skill-file.md), about 870 words. Added GPT-6's push-back wording ("state the evidence, the consequence and a better alternative"), restored "in private" to Teams, and put back all six examples, one line each. Missed: a longer file costs a little context every time it loads; the examples are worth it.
- **The gaps closed:**
  - Teams, "early": the first time it affects someone else's work (60%).
  - Unchanged by the agreed date: one more conversation, then a formal one, said up front (55%).
  - Second-model review: anything a customer, regulator, my VP or the leadership team sees, or any decision with money or a kill criterion attached (75%).
  - Escalation: I decide within my group; a call that changes another group's roadmap, dates or costs goes to my VP as a one-page recommendation within two working days, as in my Module 3 charter (70%).
  - Prioritisation tie-break: lower cost to serve, then account revenue at risk (60%).
  - Confidence percentage: how likely the recommendation is to hold, with the weakest evidence named (75%).

  Missed: regulated buyers as a third stakeholder waits until a role gives me a named buyer (60%), though they are often the hardest people to convince in my markets.
- **What the course added to my standards:**
  - Strategy's signal that would reopen it comes from the Module 1 revisit trigger and Fable's plateau rule.
  - Every no in writing comes from the Module 2 trade-off memo.
  - Leading with risk, not capacity, comes from the Module 4 revision.
  - A stop line only a new business case can lift comes from Module 5.
  - The second-model reviewer is the habit behind [PROMPTS.md](../PROMPTS.md).

  Missed: the file is written for my real role, not Fable. Fable was the practice ground that sharpened it.
- **Kept here, not installed:** it doesn't replace my existing skill files or CLAUDE.md. Missed: to do its job it has to live where the tools load it, such as a Claude Code skill folder or a Claude Project, which is a separate step.

### Final presentation

The builder pulls the five deliverables from this repo; the cover and the three reflection fields are typed in. A pre-pull check found every template label present and no blanks in all five files. The builder has no image field, so the [roadmap visual](../02-roadmap/ai-replies/3-visual-claude.png) stays in the repo rather than the presentation.

- **Working title, the Module 1 objective (65%):** "Fable Growth: the app people keep after the hard stretch". The builder's example title used "crisis", which this repo never uses in its own words. Missed: it names the goal, not the bet; the pitch carries the bet.
- **One-line pitch, the README's strategy sentence (70%):** "Fable bets its one initiative on the people it helped through a hard stretch: a personal nightly wind-down keeps them once they recover, and the community layer waits." Missed: it leaves out that the bet is tested by hand before it's built, which is what makes it fundable.
- **Name and cohort:** "Martin Cook · Product Leadership 2026.1 · November 2026". Missed: the cohort's name on the platform may differ from the course code.
- **Friction, testing demand without harming the people being tested (55%):** the first plan was a fake door, which would have disappointed vulnerable users and used their data without consent; the concierge test replaced it, with hand-built steady plans for a small group who agreed to take part and a stop rule that returns the budget to the board. Missed: keeping five modules consistent was the other real friction, since tightening Module 5's kill line quietly broke Module 3's charter.
- **Key learnings (65%):** lead a hard no with the risk to the people we serve, not capacity, because a capacity reason invites an offer of capacity; write the kill line before a bet starts, with a metric, threshold, deadline and consequence nobody who benefits can lift; and when one decision changes, read across every decision that rests on it, with a second model as a cheap reviewer. Missed: testing demand the cheapest honest way, and defining every metric by its cohort and read date, are habits this course built too.
- **Aha moment, healthy churn (60%):** when both models asked whether people who have recovered want an ongoing relationship at all, I saw that some of Fable's churn is healthy. The strategy moved from spotting dips to a nightly wind-down people choose, and KR3 now asks whether users feel steady without feeling dependent, so Fable can't win by keeping people anxious. Missed: the sharper line was Module 4's, that a capacity reason invites an offer of capacity, but it changed how I communicate, not the strategy.
