# Generation Notes

Meta-information about how this example was produced, for transparency and instruction.

## Process Timeline

| Step | Duration | What happened |
|---|---|---|
| Book deep-read (D2B) | ~12 minutes | Kahneman's *Thinking, Fast and Slow* processed; 47 knowledge blocks extracted (23 Claims, 12 Concepts, 12 Methods) |
| User profile (Assessment) | ~8 minutes | Product manager bio entered + audience/goal/constraints provided |
| Course / keynote planning (Studio) | ~4 minutes | Studio selected 11 knowledge blocks (from 47) and proposed 3-topic structure |
| Keynote script generation (Courses + Prep) | ~14 minutes | Full keynote draft + timing annotations + slide suggestions |
| **Total Herline-side** | **~38 minutes** | |
| Human editing | ~45 minutes | See "Human Edits Applied" below |
| **Total end-to-end** | **~1 hour 25 min** | |

For comparison: drafting a talk of equivalent depth from scratch typically takes a subject-matter expert 15–25 hours spread over 2–4 weeks.

## Knowledge Block Selection

From the 47 blocks extracted, Studio chose to anchor the keynote on:

- **3 Claims** (loss aversion 2x asymmetry; default effects in organ donation; anchoring with judicial dice study)
- **3 Concepts** (System 1 / System 2 / anchoring)
- **3 Methods** (loss framing pattern; anchor-first design; default-audit exercise)
- **2 Bridge blocks** (framing effects; status quo bias) used for transitions

Unused knowledge blocks remained in the user's knowledge graph — they'll be available for future keynotes, courses, or pitch decks without re-processing the book.

## Human Edits Applied

The Herline-generated draft was coherent and deliverable. Human edits focused on:

1. **Opening hook adjustment** — raw draft opened with "I want to talk about cognitive biases" (functional but generic). Rewritten to start with the shipped-feature story that pulls audience in immediately.
2. **Personal voice injection** — roughly 8 sentences rewritten in the speaker's actual voice (more conversational, more "I was wrong" framing). Herline's default tone was solid but slightly too polished for this speaker.
3. **Product example grounding** — replaced two generic examples with ones from the speaker's actual product experience (signup default story; pricing anchor story). This is critical — Herline can't know the speaker's specific product history, so these always need human insertion.
4. **Timing compression** — original generation was ~3,400 words; trimmed to ~2,900 to fit the 22-minute speaking target with breathing room.
5. **Q&A seeding** — Herline generated the main keynote but not Q&A handling. Added the four seeded questions based on audience profile.
6. **Slide cues** — restructured a few slide suggestions to be more restrained (speaker preference: no bullet walls).

**Net edit ratio**: ~25% of words changed, ~40% of sentences touched at least once. The structure and knowledge selection were kept as Herline proposed.

## What Went Well

- **Anchoring on three ideas, not summarizing the book** — this is hard to do manually; Herline's Studio layer made this choice automatically based on the 22-minute constraint and audience
- **Specific research examples with numbers** (75pp donation gap, judicial dice study) — Herline's D2B extracted these with citation intact, meaning they're verifiable against the source
- **Commitment ask at the end** — Studio proposed this structure based on the user's stated goal of "end with a commitment I want people to make"

## What Needed Human Work

- **Voice / register** — the speaker's specific verbal style isn't knowable from Assessment alone
- **Product-specific examples** — Herline doesn't have access to the speaker's internal product decisions
- **Stage-craft decisions** (pauses, slide restraint) — these are speaker preferences, not content

## Lessons for Users Trying This

1. **Deep-read the book well before generating.** Herline's output quality is heavily dependent on knowledge block quality, which depends on the deep-read pass. Don't rush that step.
2. **Be specific in Studio's audience brief.** "For product managers" produces a generic talk. "For a company all-hands, 200 people, mixed disciplines, attention span 30 minutes" produces a calibrated talk.
3. **Budget 20–30% of total time for human editing.** The draft is usable; the polish is where your voice enters.
4. **Don't regenerate trying to get the perfect draft.** Accept the 80% output and spend your energy on the 20% that makes it yours.

## What This Example Is Not

- **Not** a demonstration of Herline's maximum capability — it's a deliberate, realistic showcase at professional but not overproduced quality
- **Not** suitable as-is for a different speaker — the personal edits make it specific to this use case
- **Not** a complete pipeline demo — it shows D2B → Studio → Courses → Prep but doesn't demonstrate Boost distribution

---

*See [input.md](input.md) for what was provided, [output-keynote.md](output-keynote.md) for the final deliverable, and [README.md](README.md) for how to read this example.*
