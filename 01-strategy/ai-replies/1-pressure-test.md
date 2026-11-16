# Module 1 · 1. Pressure test

Replies to the pressure-test prompt in [PROMPTS.md](../../PROMPTS.md#1-pressure-test), run 16 Nov 2026 in new chats with no memory. Words unchanged.

Jump to: [GPT-6](#gpt-6) · [Claude](#claude)

## GPT-6

*[Copied from ChatGPT with its formatting flattened: headings, lists and the table restored here; bold and italics could not be recovered.]*

### Chief Strategy Officer’s Review: Fable Growth Strategy

Overall verdict: The strategic direction is credible, but the central assumption is unproven. You have identified a plausible reason for churn and designed a product response. You have not yet demonstrated that users want the next product you are proposing.

Here is where I would challenge you at board level.

#### 1. The single biggest assumption you could be getting wrong

You assume that users who have resolved their acute stress want an ongoing relationship with Fable to maintain their wellbeing.

That is a significant leap.

Your evidence tells you:

- Users engage heavily when experiencing acute stress.
- Fable helps them resolve that stress.
- They subsequently stop using the product.

But it does not tell you:

- Whether they want to maintain an ongoing wellbeing routine.
- Whether they see value in preventing a future stressful period.
- Whether they want an app to monitor their emotional state.
- Whether they would pay to maintain something they currently perceive as resolved.

There is a fundamental distinction between a product people need during difficult periods and a product they value when life is going well.

Your strategy assumes the latter follows naturally from the former.

It might not.

In fact, your proposed AI check-ins could create an unintended problem: reminding people about a problem they believe they have already overcome.

My challenge: Validate the desire for ongoing engagement before investing in the technology that delivers it.

#### 2. The question a board member would ask

You claim Fable has a unique advantage because it knows what helped users through their hardest stretch. What evidence do you have that users actually value that accumulated history enough to keep paying for Fable once they no longer need it?

I would expect three things before approving the investment:

1. Evidence of demand: Have former users expressed a desire for ongoing support, rather than simply wanting to leave once they feel better?
2. Evidence of differentiation: Why would a personalised steady plan be meaningfully better than a recurring meditation routine available through Calm or Headspace?
3. Evidence of willingness to pay: Would users pay for this ongoing value, or would they expect it as part of a free wellbeing experience?

The third point matters particularly.

You are targeting premium retention, not simply engagement. Those are different commercial problems.

A user returning for a free meditation is not necessarily a user who will continue paying.

#### 3. Are your KRs outcomes or outputs disguised as outcomes?

My assessment:

| KR | Assessment | Challenge |
|---|---|---|
| KR1: Premium retention at day 180, 35% → 55% | Genuine outcome | Measures commercial retention, although the 20-point improvement needs a credible basis. |
| KR2: Weekly usage from day 90–180, 20% → 45% | Behavioural outcome | Measures sustained engagement, but weekly usage does not necessarily demonstrate perceived value. |
| KR3: Return to a session within 48 hours following an early dip, 25% → 60% | Proxy metric, potentially an output | Measures a response to a product-triggered intervention, not whether the intervention improves wellbeing or retention. |

KR1 is your strongest commercial outcome. KR2 is a useful supporting indicator. KR3 is your weakest.

The problem with KR3 is that it rewards a particular behaviour without establishing whether that behaviour is beneficial.

For example:

- Users might return because notifications successfully prompted them.
- They might return because they feel anxious about the check-in.
- They might complete a session without experiencing any lasting benefit.

You could hit 60% while making the product worse.

I would replace KR3 with something closer to:

KR3: Percentage of post-acute premium users who report that Fable helps them maintain their wellbeing, without feeling dependent on the app.

Establish a baseline and set a target following initial research.

This measures whether you are delivering the value proposition you claim to own.

#### 4. One thing you said you would not do, and why you should reconsider

You should reconsider ruling out community and social features entirely.

I am not advocating building another social network or introducing user-generated content.

Your concerns about moderation, safety and team capacity are entirely reasonable.

However, you may be dismissing an important retention mechanism too early.

Consider what happens after the acute phase:

During a difficult period, Fable provides individual support. Once that period passes, users may no longer have a compelling reason to return.

But maintaining positive habits is often easier when they are reinforced through shared experiences, accountability or a sense of belonging.

A lightweight social dimension could potentially provide that reinforcement.

For example:

- Shared meditation challenges.
- Optional accountability partnerships.
- Small, curated wellbeing programmes.

These need not involve public profiles, posting or open communities.

My recommendation: Keep community out of the initial product investment, but do not make it a permanent strategic prohibition.

Test whether social accountability improves sustained engagement before ruling it out.

There is an important distinction between rejecting a feature because it is not currently the best investment and rejecting an entire strategic avenue because of its implementation risks.

#### 5. Strategy or wish list?

This is a strategy in its choice of customer and competitive positioning, but still partly a wish list in its execution: you have identified what Fable should become, without proving that post-acute users want it, will pay for it, or value its proposed differentiation enough to stay.

---

### My overall board recommendation

I would support the strategic direction, but make the investment conditional on resolving one critical question:

Does the post-acute customer actually want Fable to become a long-term wellbeing companion?

Your proposed capabilities are sensible:

- Personalised steady plans.
- Reuse of existing content.
- Non-clinical AI check-ins.
- Privacy and clinical oversight.

But these are investments in a proposed solution, not evidence of a validated opportunity.

I would ask the team to establish demand before committing the full 14-person team.

One final observation: your strongest strategic insight is that Fable should not compete to help people recover from stress better than everyone else. It should compete to help people preserve the progress they have already made.

That is a much more interesting positioning, provided customers actually want it.

## Claude

*[Claude Opus 5.5 in claude.ai. Copied with its formatting flattened: headings and lists restored here; bold and italics could not be recovered.]*

### CSO review: Fable post-acute strategy

#### 1. Your biggest assumption that could be wrong

You assume that once people feel better, they will want to keep paying to stay steady.

- The churn you describe may not be a product gap. It may just be the job finishing well. People who feel fine rarely pay to prevent a problem they don't feel, which is why gyms, insurance and relapse-prevention products all struggle.
- The strategy depends on this demand existing, and you show no evidence for it. There's no test with users who have already churned, and no proof they'd value a "steady plan".
- The second weakest assumption is the moat. "Fable saw what helped" amounts to 90 days of session logs. An AI-native competitor can learn as much in a week of onboarding. Moving the history to another app is the user's choice, but the advantage is thinner than "start from zero" implies.

#### 2. The board question you can't yet answer

"If an AI check-in is designed to detect when someone is slipping, how is that not clinical monitoring, and who is liable when it misses someone who then comes to harm?"

- "Notices early when they're slipping" is the core of the whole strategy, and it sits right on the clinical line you say you won't cross. In the UK and EU, software that detects deterioration can count as a medical device. Calling the check-ins "non-clinical" and adding a signposting partner doesn't settle that.
- Until you have a regulatory opinion, your How to Win could be ruled out by your own first constraint.

#### 3. Outputs disguised as outcomes

- KR3 is an output. It measures how users respond to your own feature, using your own model's definition of a "dip". It says nothing about whether anyone is steadier. Also, the feature doesn't exist yet, so where does the 25% baseline come from?
- KR2 is half output. Weekly use can be pushed up with notifications, so you'd be measuring your nudge engine rather than user value. The opt-out guardrail helps but doesn't fix this.
- KR1 is an outcome, but it might not measure anything. If a large share of premium users are on annual plans, day-180 "retention" is prepaid inertia. Split it by plan type, or use renewal at month 12.
- The missing outcome is whether users are actually steadier. Two ways to measure it:
  - self-reported steadiness at day 180
  - fewer users dropping back into acute-level use

  Without one of these, you can hit all three KRs and still fail the Winning Aspiration.

#### 4. Reconsider the "hard no" on community

- Your stated competitor is the user deciding they don't need Fable. The strongest known defence against that is other people. Habits last socially: Strava, Peloton, Duolingo friend streaks. AI check-ins are the easiest thing for competitors to copy, and a user's social ties are the hardest.
- You've treated "community" as if it meant only posting, groups and profiles, which is the high-risk version. Lighter forms carry almost no moderation risk:
  - one-to-one accountability with someone the user already knows
  - shared streaks
  - gifting a sleep story
  - anonymous presence ("2,400 people are doing this breath session now")
- It also gets you referral-led growth, even though new-user acquisition is out of scope, and it brings the growth team inside the bet instead of leaving them outside it. With 14 people, that alignment matters.
- Suggestion: make it a gated experiment (one buddy mechanic, tested against KR1) rather than a permanent no.

#### 5. Strategy or wish list?

It's a strategy built around a wish: it makes real choices about who, when and what not, but the How to Win rests on unproven demand, a thin data moat and a check-in that may breach your own clinical constraint.

To make it board-ready, test these first:

- a fake-door test of the steady plan with churned deep users, to see whether they want it
- a regulatory opinion on dip detection
- the annual vs monthly mix behind KR1
- an LTV case: incremental ARR if KR1 hits, against the cost of 14 people for a year
