# Module 2 · 2. Final roadmap

Replies to the final-roadmap message in [PROMPTS.md](../../PROMPTS.md#2-final-roadmap--same-chat-as-each-roadmap), run 16 Nov 2026 in the same chat as each roadmap. Words unchanged.

Jump to: [GPT-6](#gpt-6) · [Claude](#claude)

## GPT-6

*[Copied from ChatGPT with its formatting flattened: headings, lists and the table restored here; bold and italics could not be recovered.]*

This is materially stronger than the previous roadmap. It now reads like a product leader making investment decisions rather than a team translating a strategy into features.

Most importantly, you have introduced explicit validation gates, measurable thresholds and conditions for stopping or expanding investment.

I would make five final observations before taking it to the board.

#### 1. Now: Bet 1 is your strongest strategic decision

We bet offering churned deep users a personal steady plan built from what helped them will show the post-acute need is strong enough to bring them back.

This is the right first bet.

You are testing the most important assumption before committing engineering resources: whether customers actually want Fable after their acute need has passed.

I particularly like:

- Targeting churned deep users rather than assuming current users represent future demand.
- Testing willingness to return, not simply willingness to click.
- Making the regulatory opinion a prerequisite.
- Explicitly committing to stop if the evidence is insufficient.

One challenge: Your 15% click-through and 5% rejoin targets need denominators.

Specify:

- 15% of eligible users exposed to the offer click through.
- 5% of eligible users exposed to the offer actually rejoin.

Otherwise, the results could be presented favourably using different denominators.

Also, a fake-door click measures interest, not willingness to pay. Rejoining is a stronger signal, but ideally distinguish users who resume a paid subscription from those who simply reactivate.

#### 2. Now: Bet 2 risks confusing delivery reliability with customer outcomes

We bet wind-down reminders that land at bedtime in the user’s own timezone will make the nightly wind-down a habit.

The logic is sound, but 98% delivery accuracy is an operational metric, not evidence of habit formation.

You have correctly included the more meaningful measures:

- Opt-outs fall 30%.
- Three or more wind-down nights increase from 15% to 22%.

I would retain all three, but distinguish the delivery guardrail from the customer outcome.

One further challenge: a 30% reduction in opt-outs is relative or absolute? Make that explicit.

#### 3. Next: Your sequencing is good, but there is a missing investment decision

You have correctly established the dependencies:

1. Validate demand.
2. Clear regulatory boundaries.
3. Establish consent and privacy.
4. Build the steady plan.
5. Introduce user-initiated self-checks.
6. Expand to annual subscribers.

However, I would challenge one assumption:

Why does the steady plan need to be AI-powered?

Your strategy is about using historical experience to create personal relevance. That does not automatically require generative AI.

A rules-based recommendation using previous session preferences might deliver most of the value with considerably less complexity and risk.

With 14 people and one major investment, I would prioritise proving the experience before investing in sophisticated personalisation.

#### 4. Later: The relapse-reduction moat needs more careful framing

This is the most strategically interesting part of your roadmap:

Show that fewer Fable users drop back into acute-level use. This is the moat.

I agree with the ambition, but I would not yet call it a moat.

There are two problems:

First, causation. Users who adopt steady plans may already be more motivated, healthier or more engaged. A simple comparison against non-users would not establish that Fable caused the difference.

You need a suitable control group.

Second, measurement. How are you defining acute-level use?

More sessions could indicate someone is experiencing greater distress, but could also indicate healthy engagement.

You need a clinically informed, non-diagnostic definition before using this as a strategic success measure.

I would describe this as a potential source of defensibility, contingent on longitudinal evidence.

#### 5. Your roadmap has one potentially premature bet

A prevention offer to employers or insurers.

I would keep this in Later, but challenge whether it belongs in this initiative at all.

Your strategy explicitly excludes employer sales.

Reintroducing it six months later risks creating strategic drift before you have demonstrated that the core consumer proposition works.

I would make the condition stronger:

Only reconsider B2B distribution after demonstrating incremental post-acute retention and willingness to pay in the consumer business.

---

### Final assessment

| Dimension | Assessment |
|---|---|
| Strategic alignment | Strong |
| Outcome orientation | Strong |
| Sequencing and dependencies | Strong |
| Validation before investment | Very strong |
| Measurability | Good, with denominator and baseline refinements needed |
| Competitive differentiation | Promising, not yet proven |
| Resource discipline | Strong |

#### My one recommended change

Make the distinction between proving demand, proving behaviour and proving commercial value explicit.

Your roadmap currently moves between these three without always distinguishing them.

- Now: Do people want the proposition enough to return?
- Next: Does the proposition change their behaviour and improve retention?
- Later: Does sustained use create measurable customer value and a defensible advantage?

That is the investment logic I would want to see.

Board-level verdict: This is now a credible, staged product strategy. It makes a clear initial bet, establishes conditions for further investment and avoids committing the team to building an unvalidated solution.

The most important thing is that you have given yourself permission to stop. That is often the clearest sign of strategic leadership.

## Claude

*[Claude Opus 5.5 in claude.ai. Copied with its formatting flattened: the list is restored here; bold and italics could not be recovered. Claude returned its visual in the same reply: [3-visual-claude.pdf](3-visual-claude.pdf).]*

This is ready to submit. Adding Growth to Bet 2 is a good change: the growth team gets a real role in the bet, which helps settle the internal disagreement.

A few things a sharp reviewer could still pick up:

- Teams outside your 14. Growth, Legal/Privacy, Data/Insights and Commercial aren't in the team you were given (product, design, engineering, content, clinical advisory). Add a footnote saying whether they're borrowed, shared services or future hires. Otherwise the plan looks like it needs more people than the board approved.
- "Tips into crisis" in the Later fast-route bet. This wording suggests Fable detects crises, which is the clinical line you've avoided everywhere else. Try "before the need becomes acute again, with signposting to care where needed."
- No KR3 signal until Later. KR3 is the outcome that proves the strategy works, so give it a mid-point read in Next, for example 50% at month 6.
- Shared owners in Next and Later. One list of teams covers five items, so nobody owns any single one. Even putting one lead team per item would fix that.
- Two Later bets have no success signal. The fast route back and the employer offer have nothing to measure against. One line each is enough, for example "dip-to-session return within 48 hours" and "evidence pack accepted by one pilot buyer."

None of these change the plan. They close gaps a board member would find in the first five minutes.
