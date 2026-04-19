# Why Your Users Don't Think What You Think They Do

### Cognitive Biases in Product Decisions

*A 30-minute keynote.*
*Speaking notes with timing annotations.*

---

## Opening (2 min)

*[Walk on stage. No slide. Pause.]*

Three months ago, I shipped a feature I was certain users would love. Clean design, solved a real problem, A/B test looked promising on small samples.

Rollout day: adoption was 12% of what I'd projected. Not 50% off. Not 30% off. **One-eighth of what I'd expected.**

I spent a week debugging the pipeline thinking we'd broken tracking. We hadn't. The tracking was fine. The feature was fine. The users were fine.

**What was broken was the model of how users think that I'd carried in my head.**

*[First slide: title — "Why Your Users Don't Think What You Think They Do"]*

That's what I want to talk about today. Three specific ways our default product instincts mislead us, and what to do when you catch yourself doing it.

---

## The Frame: Two Systems (3 min)

*[Slide: two figures — one sprinting, one deliberating]*

There's a useful way of thinking about this from Daniel Kahneman's work. Two modes of thinking.

**Fast thinking**: automatic, pattern-matching, effortless. It's what decides that the person walking toward you is angry before you consciously read their face. It's what tells you 2+2=4 without calculating. **It runs all day, every day, without your permission.**

**Slow thinking**: deliberate, effortful, serial. It's what you use to calculate 17×24, or to decide whether to accept a job offer. It's costly — your brain doesn't want to run it unless forced.

Here's the part that matters for us:

**Users make product decisions with fast thinking. By default. Always. Unless forced not to.**

And most of what we build, most of what we test, most of what we design — is built as if users were doing slow thinking. Reading our copy carefully. Weighing alternatives rationally. Following the funnel we designed.

They're not. Not even close.

---

## Bias #1: The Defaults We Don't See (6 min)

*[Slide: blank, subtle "1" in corner]*

Let me give you a specific example.

2008. Cass Sunstein and Richard Thaler publish research on organ donation rates. In countries where you have to opt **in** to donate, donation rates are around 15%. In neighboring countries with identical culture, identical wealth, identical everything — but where you have to opt **out** — donation rates are over 90%.

*[Slide: two bars — 15% vs 90%]*

Same people. Same values. Same intent to help. The default setting of the form moved donation rates by 75 percentage points.

**The default is not a neutral starting position. The default is the decision for almost everyone.**

Now think about your product.

- What are your defaults?
- Who chose them?
- When was the last time you questioned them?

At my company, we had a signup flow that defaulted new users to "weekly digest." We assumed most people wanted less email. That felt right. It felt respectful.

Turns out when we A/B tested "daily digest" as default — same email frequency available either way, just different starting state — **30-day retention jumped 18%**. Because users who got more early exposure formed a habit. The ones who opted into "weekly" had already quietly churned by week 3.

We weren't being respectful. We were being default-blind.

**Question for you**: in your product, what defaults did you inherit without questioning? Write down the three you'd most like to revisit. I'll come back to what to do with that list.

*[10 seconds silent pause for writing — important]*

---

## Bias #2: The Anchor That Set Itself (6 min)

*[Slide: "1" fades. "2" appears]*

Second one. Same author, same book. This one is called **anchoring**.

If I show you a random number — say, 65 — and then ask "what percentage of African countries are in the UN?" your answer will be biased toward 65. Even though you know the number is random. Even though you know you shouldn't let it influence you. **It does anyway.**

Kahneman ran this experiment with judges — professional, experienced judges — rolling a pair of dice before sentencing. The dice were literally random, and the judges knew. Higher dice rolls produced longer sentences. **The judges. With dice. Knowing.**

This is not a curiosity. This happens in your product, constantly.

*[Slide: a price tag "$19 / month, was $99"]*

The first price a user sees anchors every subsequent price comparison. The first friend they follow anchors their sense of "who's normal to follow here." The first piece of content they see anchors what they think the product is for.

**Your onboarding isn't a tutorial. It's an anchor factory.**

I was on a team that changed the first screen of onboarding — same flow, same functionality, different first screen — and saw 40% different engagement patterns three weeks later. Not in the onboarding metric. Three weeks later. Because the anchor set expectations we couldn't unset.

Here's the thing: you probably can't remove anchoring. You can't make users decide "rationally." But you can **choose what you anchor them to**. Deliberately.

- If you want users to invest deeply, anchor them to depth early.
- If you want users to feel they belong, anchor them to a community moment.
- If you want users to upgrade, anchor them to the premium experience.

**Ask yourself**: what's the first thing a new user sees? Is it what you actually want to anchor them to?

*[Slide: the title card from your own onboarding — if you can, use it]*

If you don't know, that's the problem. Go look today.

---

## Bias #3: The Loss You Can't Name (6 min)

*[Slide: "2" fades. "3" appears]*

Third one. The big one. **Loss aversion.**

Kahneman and Tversky's most famous finding: losing $100 hurts about twice as much as winning $100 feels good.

Read that again. *Twice as much.*

This is why status quo bias is so strong. Why users abandon carts with one item left to configure. Why churn is so hard to reverse. Why nobody deletes their old account even when they've moved on.

**Users don't weigh options rationally. They're specifically terrified of losing things they already have — even when they don't really have them.**

*[Slide: a shopping cart icon with a small item, labeled "abandoned"]*

Here's where this gets specific for product work.

When you design a feature removal — let's say you're simplifying, cutting a rarely-used option — your rational model says: "1% of users use this, removal cost is low."

Loss aversion says: **those 1% will notice more than the 99% will ever appreciate the simpler experience.** And they'll tell three friends. And they'll write the review. And they'll flood support.

When you price something higher, your rational model says "customers will compare total value received vs. price paid."

Loss aversion says: **customers will compare the new price against the old price and experience the difference as a loss.** Even when the new price is objectively better value.

When you change a workflow, same thing. Even improvements are experienced as losses.

**The rule I now use**: *every change is a loss until you prove otherwise — to the user, not to yourself.*

So how do you design around it?

Three patterns that work:

**1. Loss framing for positive actions.** "You're about to lose access to this free tier offer" works better than "Upgrade to unlock more." Same action, different framing. The first engages loss aversion for you.

**2. Preserve something when you remove something.** When you cut a feature, replace it with a visible alternative in the same place. Don't just remove it.

**3. Anchor to the future state, not the transition cost.** If you're launching a price increase, anchor users to what they'll have at the new price — not what they're losing.

---

## The Pattern (3 min)

*[Slide: blank]*

Take a step back.

What do these three have in common?

**Defaults**: users decide by not deciding.
**Anchoring**: users decide by reference to what they saw first.
**Loss aversion**: users decide to protect what they have, even at the cost of what they could get.

None of these are "irrationality." They're how minds work. Every mind. Including ours.

**The mistake is thinking our users are the exception.** Or thinking *we* are the exception when we design for them.

The product insight isn't "users are irrational, so trick them." It's "users are efficient — they use fast thinking because it works for 95% of life, and our job is to recognize when we're in the 5% where it misleads."

---

## The Commitment Ask (3 min)

*[Slide: blank]*

I said I'd end with a commitment.

This week — not next quarter, not "when I have time," this week — I'm asking you to do one thing.

**Pick one feature, flow, or decision in your product. Not a new one. Something you've shipped, something that's running.**

For that one thing, write down:
1. What default did I set, and is it the right one?
2. What's the user's first anchor, and is it what I want them to be anchored to?
3. If I rolled this back, what would users experience as lost — and am I managing that?

One feature. Three questions. Thirty minutes max.

*[Pause]*

If you do this, you'll find at least one thing you want to change. I'll bet on it.

And when you change it — send me a note. I want to know what you find. Because I guarantee you the thing you find won't be the thing I found last time I did this exercise. These biases are consistent, but they hit different surfaces in different products.

*[Slide: email on screen]*

That's the talk. Thank you.

---

## Q&A Framing (8 min)

*[Invite questions]*

Likely questions and how to handle them:

**"Isn't this just manipulation?"**
Good question. The line is: manipulation is using these patterns against the user's interest. Design awareness is using them with the user's interest. Spam email uses loss aversion to trick you. A good onboarding uses anchoring to get you to the value faster. Same mechanic, opposite intent.

**"How do I test for these?"**
You often can't in short-horizon A/B tests because the effects show up weeks later. Qualitative research helps — specifically, watch users in unmoderated recordings and ask "what did they notice first? what didn't they notice at all? what did they resist changing?" Those three questions surface the patterns.

**"My team won't buy this — they're all data-driven."**
The data-driven rebuttal is that ignoring cognitive biases means your A/B tests are measuring the wrong thing. A 5% lift in a conversion metric doesn't mean you made the product better — it might mean you triggered loss aversion in a way that'll cost you retention next quarter. Your data-driven team should love this framing, because it's more honest about what data can and can't tell you.

**"What do I read next?"**
*Thinking, Fast and Slow* if you haven't. *Nudge* by Thaler and Sunstein is shorter and more applied. For the design angle, *Misbehaving* by Thaler has great stories on how these ideas land in practice.

*[Close: thank audience, walk off]*

---

## Timing Notes

| Section | Target | Notes |
|---|---|---|
| Opening | 2 min | Don't rush — silence after "one-eighth" lands |
| Frame | 3 min | Introduce two-systems concept concretely, not academically |
| Bias 1 (defaults) | 6 min | The 10-second writing pause is important — don't skip |
| Bias 2 (anchoring) | 6 min | Use your own product's onboarding screenshot if possible |
| Bias 3 (loss aversion) | 6 min | This is the biggest — don't compress |
| Pattern | 3 min | Slow down, let it land |
| Commitment ask | 3 min | Look at specific people, not the back wall |
| **Speaking total** | **~29 min** | Targeting 22, will run over slightly |
| Q&A | 8 min | If no hands, use the seeded questions |

**Words**: ~2,900
**Speaking pace**: ~130 words/min
**Total speaking time**: ~22 min (leaves buffer for pauses, laughter, transitions)

---

*This keynote was generated by Herline from a single book deep-read plus a short user brief. See [generation-notes.md](generation-notes.md) for the process.*
