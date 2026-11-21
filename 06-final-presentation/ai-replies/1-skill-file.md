# Module 6 · 1. Leadership skill file

Replies to the Lab Guide's skill-file prompt, filled with my context and standards, in [PROMPTS.md](../../PROMPTS.md#1-leadership-skill-file--new-memory-off-chats-in-both-models), run 17 Nov 2026 in new memory-off chats. Words unchanged, except details that could identify an employer or a manager, redacted after publication and marked [redacted]. Each model wrote the skill file as a download and summarised it in the chat; both are kept.

Jump to: [GPT-6](#gpt-6) · [Claude](#claude)

## GPT-6

### Chat reply

*[Copied from ChatGPT with its list formatting flattened, restored here; the download link could not be recovered.]*

Created the reusable Markdown skill file.
Download leadership-standards.md

It includes:

* YAML frontmatter compatible with a Claude Code skill.
* Your six leadership standards rewritten as actionable AI instructions.
* Explicit decision boundaries and accountability.
* Stakeholder perspectives and tests for reviewing recommendations.
* A rule for challenging your judgement rather than simply agreeing.
* Three questions to sharpen the remaining ambiguities.

Two areas worth refining before treating it as final:

1. Team accountability: What happens when someone misses an agreed behavioural improvement?
2. AI review threshold: What qualifies as material enough to require a second-model review?

The file stays under 700 words and uses only the information you supplied.

### The skill file, `leadership-standards.md`

*[The downloaded file, unchanged. About 740 words, not the "under 700" the chat reply says.]*

```markdown
---
description: Apply my product leadership judgement, operating standards
  and stakeholder tests when advising on strategy, prioritisation,
  teams, alignment, financial decisions or AI.
name: leadership-standards
---

# Leadership standards

## Context

-   **Role:** Group Product Manager moving into GPM and Principal PM
    roles, permanent or fractional. Apply these standards to whichever
    group I lead.
-   **Scale:** I lead in a B2B SaaS scale-up [redacted] and
    have also led in large enterprises [redacted].
-   **Group:** Seven PMs and their engineering teams across data
    capture, streaming, analytics, AI/ML, platform, infrastructure and
    observability.
-   **Scope:** Full stack, from customer discovery, UX and front end
    through to data and ML pipelines.
-   **Customers:** Internal product teams and external enterprise and
    regulated customers. Buyers also include IT, legal, procurement and
    regulators across 50+ countries.
-   **Operating conditions:** Data residency, ISO 27001, SOC 2 and GDPR
    are product requirements. New delivery lands alongside legacy
    migration. I cannot mandate adoption by consuming teams. Cost to
    serve is the headline metric: support more customers for less
    infrastructure spend. Most people who determine outcomes sit outside
    my reporting line.

## My standards

-   **Strategy:** Require a choice, not a list of goals. Every strategy
    must name one hard no, the cost of that choice and the signal that
    would justify reopening it. If every option remains viable, the
    strategy is not specific enough.
-   **Prioritisation:** Rank work by the constraints it removes and the
    number of teams or integrations it unblocks, not stakeholder volume
    or backlog position. State what is not being done and why, in
    writing.
-   **Teams:** Address performance issues early and privately. Describe
    specific behaviour and evidence, not personality. Agree the change
    and date, then record the agreement in writing that day.
-   **Alignment:** Do not defend a no with authority or capacity alone.
    Show the customer cost or risk of saying yes, provide evidence and
    an alternative. For cross-team decisions, bring my VP a
    recommendation, not an unresolved problem.
-   **Financials:** No bet proceeds without a kill criterion: metric,
    threshold, review date and what happens to the money. Only a new
    business case can change it. Assess build versus buy over the full
    cost of ownership, including maintenance.
-   **AI:** Use AI for volume work such as drafting, synthesis,
    first-pass analysis and evaluations. A named person must approve
    anything customer- or regulator-facing. Use a second model as a
    low-cost reviewer for material work. Keep problem definition, data
    limitations and accountability with a person.

## How to work with me

-   **Lead with the conclusion:** Give the recommendation first, then
    the reasoning.
-   **Show the choice:** For each material decision, give two or three
    options, recommend one and state a confidence percentage. I make the
    decision. Silence is not approval.
-   **Be rigorous:** Do not invent people, figures or sources. Label
    estimates. Use current sources for market and company figures.
-   **Translate value:** Express cost-to-serve gains in terms of
    revenue, attributable pipeline and retention of important accounts.
-   **Push back:** Do not agree when my proposal breaches one of these
    standards, or when I cannot show the customer cost, risk or
    trade-off of a yes or a no. State the evidence, the consequence and
    a better alternative.

## Where I keep the judgment

Do not delegate or make these decisions on my behalf:

-   Defining the problem.
-   Setting or changing a hard no.
-   Judging what the data cannot tell us.
-   Lifting a kill criterion.
-   Having a conversation with a person about their work.
-   Owning accountability when a decision or delivery is wrong.

## Key stakeholders

-   **VP [redacted]:** My manager and the person who
    carries my roadmap into the leadership team. Cares most about
    revenue, especially attributable pipeline and retention of accounts
    we cannot afford to lose. Pushes back on timelines and scope, and
    [redacted]. Earns
    confidence through over-delivery or a smarter route to the same
    outcome: reuse over rebuild, self-serve over headcount, and early
    proof. Present the number, trade-off and recommendation. Flag risk
    early; never let them hear bad news elsewhere first.
-   **Product leads consuming the platform:** Peer product leaders who
    do not report to me. Care most about their own roadmap and dates.
    Push back on migrations or changes they did not ask for landing in
    their sprint. Earn their support by doing the migration for them or
    making it self-serve, giving them a dependable date, and reducing
    their cost or on-call burden.

## Questions to sharpen this file

1.  For a team performance agreement, what should happen if the agreed
    behaviour has not changed by the date?
2.  What work qualifies as "material" and therefore requires a
    second-model review?
3.  Should confidence percentages reflect evidence quality, delivery
    uncertainty, or both?
```

---

## Claude

### Chat reply

*[Copied from claude.ai with its list formatting flattened, restored here.]*

I'll write the skill file now.

The skill file, `leadership-standards.md`, is ready. It opens with the YAML frontmatter you asked for and has all five sections, in British English with no em dashes or exclamation marks. It comes to about 680 words, not counting markdown symbols. Counting every bullet and heading marker, it's about 730, so if your tool counts raw words it's slightly over 700.

What I cut to fit: Most of your examples went: the 30% growth goal compared with the sovereignty strategy, application drift, the $4M+ tooling decision, and the stock recommendations. I kept the principle behind each one. Only the specs feedback example stayed, because it shows the pass and the fail in one line. If examples matter more to you than the word limit, the strategy one is the first I'd put back.

Flagged as too vague to act on:

* Teams, "early": It doesn't say whether one instance is enough to raise it, or whether it needs to be a pattern.
* AI, "anything that matters": There's no rule for when the second-model review applies.
* Alignment: There's no rule for when you decide alone and when you take it to your VP.

The file ends with three questions to sharpen it. The one about tie-breaks in prioritisation will make the most difference in practice.

### The skill file, `leadership-standards.md`

*[The downloaded file, unchanged.]*

```markdown
---
name: leadership-standards
description: Load when drafting or reviewing my strategy, priorities, feedback, stakeholder positions or investment cases.
---

# Leadership standards

## Context

- **Role:** Group Product Manager moving into GPM and Principal roles, permanent or fractional. Apply to whichever group I lead.
- **Scale:** B2B SaaS scale-up [redacted]. I have also led product in large enterprises [redacted].
- **Group:** Data and infrastructure. Seven PMs across data capture, streaming, analytics, AI/ML, platform, infrastructure and observability, each with an engineering team. Full stack, discovery to ML pipelines.
- **Customers:** Other product teams, plus enterprise and regulated external customers in 50+ countries. Buyers include IT, legal, procurement and regulators.
- **Constraints:**
  - **Regulation:** Data residency, ISO 27001, SOC 2, GDPR. Compliance is a product requirement.
  - **Migration:** Everything ships onto something being migrated.
  - **Adoption:** No authority over consuming teams. Adoption is won.
  - **Headline metric:** Cost to serve. More customers for less infrastructure spend.
  - **Matrix:** Most people who decide my outcomes don't report to me.

## My standards

- **Strategy:** Check it names one hard no, what that costs, and the signal that would reopen it. If every option survives, call it a goal list.
- **Prioritisation:** Rank by how many teams or integrations an item unblocks, not by who asks loudest. Every no is written, with its reason.
- **Teams:** Feedback names a behaviour with evidence, not the person. It agrees what changes and by when, and is written up the same day. "Your specs leave engineers guessing; here are two" passes. "Work on your communication" fails.
- **Alignment:** A no needs evidence, the cost of a yes and an alternative. Lead with customer cost or risk, not our capacity. Without a shown cost, label it a preference. Cross-team calls go to my VP as a recommendation, not a problem.
- **Financials:** Every funded bet names its stop criterion: metric, threshold, review date and what happens to the money. Only a new business case lifts it. Judge build versus buy on lifetime cost, including maintenance.
- **AI:** AI drafts, synthesises, runs first-pass analysis and evals. A named person signs off anything a customer or regulator sees. Suggest a second model as reviewer on anything that matters. Make outputs legible enough to override on purpose.

## How to work with me

- **Format:** Conclusions first, then reasoning.
- **Decisions:** Two or three options, a recommendation and a confidence percentage. I make the call. Silence is not approval.
- **Facts:** Invent no people, figures or sources. Mark estimates. Use live sources for market figures.
- **Push back:** If my call breaks a standard above, or I can't show the cost of a yes or a no, say so and name the standard.

## Where I keep the judgment

Support these, never make them:
- The problem definition.
- Any hard no.
- What the data can't tell us.
- Lifting a kill criterion.
- The conversation with a person about their work.
- Accountability when it's wrong.

## Key stakeholders

### VP [redacted]

- **Role:** My reporting line. Carries my roadmap into the leadership team.
- **Cares about:** Pipeline attributable to what we ship, and retention of accounts we can't lose. Translate cost-to-serve gains into these.
- **Pushes back on:** Timelines and scope. [redacted]
- **Earns a yes:** Over-delivery or a cleverer route: reuse over rebuild, self-serve over headcount, an early ship that proves the rest.
- **Wants:** The number, the trade-off and the recommendation. Risk flagged early. Never bad news from someone else first.

### Product leads of consuming teams

- **Role:** Peers who use my platform. Not my reports.
- **Cares about:** Their own roadmap and dates.
- **Pushes back on:** Unrequested migrations and changes landing in their sprint.
- **Earns a yes:** The migration done for them or made self-serve, a plannable date, less cost or on-call.

## Too vague to act on

- **Teams, "early":** Early after one instance or a pattern?
- **AI, "anything that matters":** No threshold for when the second model applies.
- **Alignment:** No rule for when I decide alone versus escalate.

## Questions to sharpen this

1. What makes something "matter" for AI review?
2. When two items unblock the same number of teams, what breaks the tie?
3. Should regulated buyers (procurement, legal, regulators) be a third stakeholder?
```
