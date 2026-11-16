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
