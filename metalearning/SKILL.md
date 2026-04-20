---
name: metalearning
version: "0.2.0"
description: "Metalearning — Barbara Oakley *Learning How to Learn* + Scott Young *Ultralearning*. Focused/diffuse modes, illusion of competence, MOC (map of content), learning project design. The upper layer for rapidly acquiring new fields."
---

# Metalearning

> Background and theory: Read references/foundation.md



## Layer Position

**L1 (upper-level design)** — The meta-layer that selects and allocates across all other layers. The 10% time principle (Young) — design must not replace learning itself. L1 excess = technique shopping and consuming YouTube study-method videos.

## When to Use

- **Designing self-study for a new field** — how to combine courses and tutorials
- **When learning keeps failing or stalling** — when the technique itself is the problem
- **When choice among multiple techniques is unclear** — the meta-layer integrates them
- **Before starting a learning project** — Ultralearning-style projects
- **Diagnosing your own learning** — where you're getting stuck

## Practical Protocol

### Young-style Metalearning Steps (1–3 weeks)
1. **Clarify motivation** — Why, how much, by when.
2. **Prior research** — How did experts in this field learn? Collect blogs, books, interviews, roadmaps.
3. **Determine concepts/facts/procedures ratio**:
   - E.g., frontend development = concepts (many) + procedures (many) + facts (few) → centered on deliberate practice + feynman
   - E.g., medical school preclinical = facts (many) + concepts (medium) → centered on SRS + active recall
4. **Set benchmarks** — Against existing curricula (university courses, well-known roadmaps).
5. **Revise = Emphasize / Exclude** — Remove what's unnecessary for your purpose and emphasize the core.
6. **Schedule design** — Total duration, weekly hours, feedback points.

### Oakley-style Learning Habits
- N Pomodoro sessions per day.
- Rest at the end of each session = time for diffuse mode.
- When hitting a hard problem, leave and allow diffuse (sleep, walk, shower).
- Weekly self-testing (retrieval tests).

### Learning Project Template
```
Project: [name]
Duration: [N months]
Total time: [estimated N hours]
Goal (success criterion): [measurable]
What (content):
  - Concepts: [list]
  - Facts: [list]
  - Procedures: [list]
Materials:
  - Primary textbook: [book/course]
  - Secondary materials: [blogs/videos]
  - People: [tutors/community]
Technique mix:
  - [allocation among active-recall / SRS / feynman / deliberate-practice, etc.]
Feedback channels:
  - [exams/code review/teacher/study group/AI]
Risk & Plan B:
  - [expected failure points and alternatives]
```

### Designing External Feedback Channels (Self-Directed ≠ Isolated)

The biggest cause of failure in self-directed learning = absence of feedback channels. Alone, blind spots solidify. Secure them *in advance* during the meta-design phase:

| Channel | Strengths | Weaknesses | Korean Context |
|---|---|---|---|
| **Teacher/coach/tutor** | Immediate, specific feedback; breaks stagnation | Cost, hard to find | 과외 (private tutoring), hagwons, private lessons. For certification exams, specialized instructor Q&A |
| **Study groups/community** | Retrieval pressure, peer questions, retention motivation | Level variance, management cost | Hagwon study groups, open chats, Discord. Particularly effective for civil service and certification prep |
| **Lecture videos/MOOC** | Systematic, repeatable, low cost | Passive consumption trap (rereading-style) | 공단기, EBS, 인프런, Coursera. *Require retrieval after watching* |
| **Past exams/mock tests** | Matches exam format, automatic feedback | Dependent on answer commentary | Korea's certification ecosystem is mature — 5 years of past exams is standard |
| **AI (Claude/GPT)** | Infinite patience, Feynman audience, question generation | Risk of factual errors; misuse amplifies illusion | See section below |
| **Self-recording and review** | Awareness of mumbling | Lacks external perspective | Presentations, lectures, coding sessions |
| **Field feedback (execution results)** | The truest signal | Delayed, costly | Real code, PRs, real exams, real performances |

**Principle**: Before starting a learning project, calculate "How many hours and how much does it cost to get one round of feedback?" The longer the feedback cycle, the longer the stagnation.

### How to Learn With AI (Feynman Audience-ification)

AI should be used as a *retrieval amplifier*, not a *rereading machine*.

**Good prompt patterns** (I retrieve → AI gives feedback):
- "I'll try to explain this concept. Point out where I get stuck or say something wrong: [my explanation]"
- "What did I miss from the concepts in Chapter 3 of [textbook]? Without showing me the TOC, I'll try to reconstruct it: [my reconstruction]"
- "I'll analyze why I got this problem wrong: [my analysis]. Turn the points I missed into questions for me."
- "Ask me 5 counterexamples or edge cases on this topic that I'm likely to miss." (*pretesting*)
- "I'll answer the blank in this card: [my answer]. Just judge if it's right, and give hints in stages."

**Bad prompt patterns** (AI reads → I reread):
- ✗ "Summarize this chapter for me" (AI retrieves, I consume)
- ✗ "Explain this concept simply for me" (AI replaces Feynman)
- ✗ "Organize this book for me" (hover reading)
- ✗ "Make 100 flashcards for me" (the card-making process itself is the learning, and it's being stripped away)

**Principle**: *I retrieve, AI grades.* If AI retrieves and I only watch, it reverts to Dunlosky low utility. Explicitly instruct the AI: "I'll answer first, you only judge."

**Limits**:
- AI can make factual errors and hallucinate. High-stakes domains (medicine, law, certification statutes) *must* be cross-checked with official sources.
- A conversation with AI that ends in one session without spacing has weak retention. Must be combined with SRS.
- It's risky when AI keeps saying "great job." Specify strict-judgment mode ("Don't be lenient, point out specific gaps").

## Korean Context Examples

**Frontend → Backend transition (6 months)**:
- Why: Expand capability to full-stack, raise market value
- What: Concepts (many — HTTP, DB, system design) + procedures (many — language, framework) + facts (medium — API syntax)
- How: *Designing Data-Intensive Applications* + real project + System Design interviews + mentor code review
- Mix:
  - Concept understanding → feynman + evergreen-notes
  - Syntax/libraries → active recall + writing real code (directness)
  - System design → deliberate practice (2 design sessions + feedback per week)
  - Focus blocks → deep-work rhythmic

**IFAT Expo Preparation (1 month)**:
- Why: Water treatment equipment market research
- What: Facts (company/product info) + concepts (water treatment technology principles) + procedures (expo questioning)
- Mix:
  - Basic German vocabulary → SRS
  - Water treatment technology principles → feynman + paper notes (zettelkasten light)
  - Meeting scenarios → deliberate practice (mock meetings + feedback)

## Anti-patterns

- **Technique shopping** — Trying a new technique every week, never settling. Metalearning is a tool, not a collection.
- **Eternal map-drawing** — Ignoring the 10% principle, only preparing and never starting.
- **YouTube study-methods only** — Watching 100 study-method videos is not studying. A meta-version of illusion of competence.
- **Expecting one book to solve it** — Just reading *Learning How to Learn* or *Ultralearning* changes nothing. Knowledge without execution.
- **Tool-setup fatigue** — 3 days setting up Obsidian plugins, downloading an Anki deck and abandoning it, burning a weekend on a Notion dashboard. The pattern where tool setup becomes an excuse to avoid learning.
- **Internalizing wrong "laws"**:
  - "10,000-hour rule" — Ericsson himself refuted Gladwell (→ `deliberate-practice`)
  - "Learning styles" (VAK: visual/auditory/kinesthetic) — Pashler et al. (2008) *Psychological Science in the Public Interest* critical review concluded *there is no empirical evidence supporting the "meshing hypothesis"*
  - "Right-brain/left-brain types" — Nielsen et al. (2013) fMRI study of 1,011 subjects found no left-right brain preference
  - "Speed reading" — Rayner et al. (2016) *Psychological Science in the Public Interest* — no empirical evidence for reading fast while maintaining comprehension. Speed↑ trades off with comprehension↓.
  - "1-minute / 60-second memory method," "secrets of geniuses" — popular-book and YouTube exaggerations
  - **Korean-specific misconceptions**:
    - "The CSAT (수능) is about memorization" — Actually it's about pattern identification, procedures, and retrieval under time pressure. Interleaving and retrieval are the core.
    - "Work through a problem book 10 times" — Dunlosky low utility. Rereading only increases familiarity.
    - "Waking up at 4 a.m. is the secret of success" — No basis. Individual chronotypes vary widely, and sleep deprivation impairs cognition.
    - "Only med students use Anki" — Domain-agnostic. Valid for all learning that requires factual memorization.
    - "If you don't use Zettelkasten, you're not a real intellectual" — Fetishization of tools and systems. Luhmann's individual case doesn't transfer to everyone.
    - "Just finish the lecture videos" — Passive consumption. Without retrieval, no retention.
- **Talent dichotomy** — "I don't have a math brain" — a fixed mindset. Oakley herself is a counterexample (engineering major in her 40s). → See `growth-mindset`.

## Limits

1. **Meta-knowledge cannot replace actual learning** — Knowing without doing is useless. In the end, time and repetition.
2. **Differences across fields** — Meta-principles are common but specific techniques are field-specific. Medical school, music, language, programming all differ.
3. **Beware of self-deception** — The illusion that "I understood" while reading meta-theory. *Actual behavior* is the indicator.
4. **Young's anecdotal evidence** — Cases in *Ultralearning* are dramatic, but caution about generalization. Background, time, resources differ.
5. **Oakley's popularization of neuroscience** — Some concepts (mentions of misconceptions like left/right brain) require care. She has since corrected these more accurately.
6. **Being absorbed only in meta-learning** — Studying study methods can become avoidance of learning.

## What to Combine This Framework With

- **All other frameworks** — Metalearning is the *upper layer*. Its role is to select the combination.
- **deliberate-practice** — Young's Directness, Drill, and Feedback mesh with Ericsson.
- **active-recall + spaced-repetition** — The basic engine for retaining facts and concepts.
- **feynman-technique** — Concept understanding and breaking illusion.
- **zettelkasten / evergreen-notes** — Accumulating learning outputs.
- **deep-work / pomodoro-and-focus** — Time and environment layers.

## When This Framework Is *Wrong*

- If the problem is not technique but focus, sleep, or health → start from basic lifestyle
- If you're mid-practice of a concrete skill → go straight to `deliberate-practice`
- If the exam is imminent (≤ 2 weeks) → go straight to SRS + active recall, postpone meta-design
- For comprehension gaps → `feynman-technique` immediately

## Further Reading

- Oakley, B. & Sejnowski, T. (2014). *Learning How to Learn.* + Coursera MOOC of the same name.
- Oakley, B. (2017). *Mindshift.* (Research on learner transitions)
- Young, S. (2019). *Ultralearning.*
- Young, S. *Learn More, Study Less.* (Early practical book)
- Dunlosky, J. et al. (2013). "Improving Students' Learning With Effective Learning Techniques." *Psychological Science in the Public Interest.* (Technique-comparison meta-analysis)
- Brown, P. C. et al. (2014). *Make It Stick.* (Popular edition of cognitive science)

