---
name: spaced-repetition
version: "0.2.0"
description: "Spaced Repetition — interval-based review learning rooted in Ebbinghaus's forgetting curve. SM-2 and FSRS algorithms. Anki and SuperMemo lineage. The strongest tool for memorizing terminology, facts, language vocabulary, medicine, and law. Managing the long-term retention curve."
---

# Spaced Repetition

> Background and theory: Read references/foundation.md



## Layer Position

**L4 (Retrieval & Retention)** — one body with `active-recall`. SRS = active recall + optimal intervals. Without L3 (understanding, feynman-technique) preceding it, the process is inefficient (do not card-ify before understanding).

## When to Use

- Factual memorization: **terms, definitions, formulas, foreign-language vocabulary, dates, classifications**
- **Medicine, law, certification exams** — where broad and accurate memorization is essential
- **Language learning** — vocabulary, grammar patterns, Chinese characters, word discrimination (though only partially effective for conversation and listening)
- **Long-term retention** — knowledge that must be learned once and maintained for years
- **The opposite of one-off cramming** — preventing post-exam evaporation

## Practical Application

### Card Design Principles (Wozniak's "20 rules")
- Minimum information principle: one card = one fact
- Do not card-ify before understanding: understanding must come before memorization
- Use cloze (fill-in-the-blank) format: "{{Photosynthesis}} converts light energy into chemical energy"
- Include context: short phrases or example sentences rather than isolated words
- Personalize: link to your own experience or imagery
- Mnemonic images can be used

### Daily Rhythm
- 10–20 new cards / 50–200 reviews per day (adjust by field and timeframe)
- Must be done daily — skipping accumulates, a 1-week gap = several days of recovery
- 15–30 minute sessions × every day is the standard

### When to Stop
- Continue reviewing even after finishing study of the topic — this is the key advantage
- Suspend or delete cards no longer needed. Managing card count is also a skill.

## Korean Context Examples

Preparing for the IFAT Munich 2026 expo — basic German vocabulary:
- "Wasseraufbereitung" — water treatment (front: English/Korean, back: German)
- "Anlage" — facility/plant (with example sentence)
- 15 new cards/day, 60 reviews/day. In 3 months, you retain 1,000 words.

Medical school clinical-phase exams:
- Anatomy, per muscle: origin, insertion, nerve — 3–4 cards per muscle
- Pharmacology, drug mechanisms — 5–10 cards per drug
- Managing a cumulative 8,000–15,000 cards is within the normal range. FSRS can handle it.

Civil service exam (Grade 9 Korean, Korean history, English):
- Korean history dates, figures, events: chunk-level cards (→ `chunking`). Per event: 3 cards for date, figure, background
- English vocabulary: the 2,000–3,000 high-frequency civil-service words → spread over 6 months with SRS
- Korean grammar: factual rules (phonological changes, etc.) are card-ifiable; reading comprehension should be handled separately via active recall
- Retention caveat: maintain the deck even after the exam, through promotion tests and the next exam cycle

Licensed Real Estate Agent exam (Parts 1 & 2):
- Civil code, public law, public-notice law — article numbers and keywords go into SRS (cloze format)
- Case law: *understand first* → after understanding, make a "one-line gist" card
- Starting 3 months before the exam: 20 new / 100+ reviews per day. Keep the deck small before then.

**Note**: *Building cards yourself* is the learning; *downloading* a deck is not. Pre-made decks, even when formally correct, are inefficient for review because they don't align with your own comprehension structure.

## Anti-Patterns

- **Studying = making cards** — the phenomenon of only creating cards but never reviewing. Cards are a *tool*, not the learning itself.
- **Card-ifying without understanding** — understanding must come before memorization for efficiency. SRS is a *retention* tool, not an *understanding* tool.
- **Cards that are too long** — an entire paragraph on one card. Retrieval failure rates spike.
- **Overusing "Easy"** — S increases only when retrieval was difficult. Pressing it anyway only stretches the interval without actual memorization.
- **Daily cramming** — SRS requires a daily rhythm. Cramming 3 hours on the weekend tangles the queue.
- **Everything in SRS** — applying SRS to concepts, relationships, judgment, and procedural skills is overreach. SRS is for facts and explicit knowledge.

## Limitations

1. **Cannot teach semantic understanding or inference** — only "what," not "why." Combine with other frameworks for conceptual learning.
2. **Bias toward context-independent knowledge** — cards carry thin context. They serve exams, but real-world application needs additional training.
3. **Dependent on motivation** — the constraint of doing it every day. Many people, after a 3-week gap, quit because of the recovery burden.
4. **Affected by emotion and stress** — sleep deprivation or anxiety increases retrieval failure rates. Condition shakes the curve.
5. **Algorithms are not perfect** — SM-2 is conservative. FSRS improves on it, but individual variance is large. Adjust after several months of data accumulate.
6. **Language learning is only partial** — strong for vocabulary and grammar, weak for conversation, listening, and pronunciation. Input/output training is required.

## Frameworks to Use Alongside

- **active-recall** — the *engine* of SRS. Every card is a retrieval exercise. The two frameworks are practically one body.
- **interleaving** — SRS naturally produces a mix of cards across topics. A built-in advantage over block learning.
- **feynman-technique** — if your understanding is too shallow to commit to a card, do Feynman first. Card-ify after understanding.
- **zettelkasten** — extracting the core claims of Zettel permanent notes into cards = a two-layer structure of understanding (Zettel) + retention (SRS).
- **chunking** — cards must be composed of meaningful chunks to distribute load.

## When This Framework Is *Wrong*

- Conceptual, relational, or inferential learning → `feynman-technique` / `zettelkasten`
- Procedural skills → `deliberate-practice`
- Non-exam, creative work → `zettelkasten` / `evergreen-notes`
- The root problem is focus or time availability → `deep-work` / `pomodoro-and-focus`

## Further Learning

- Ebbinghaus, H. (1885). *Über das Gedächtnis.* (English translation *Memory*, 1913)
- Cepeda, N. J., Pashler, H., et al. (2006). "Distributed practice in verbal recall tasks: A review and quantitative synthesis." *Psychological Bulletin.*
- Wozniak, P. "Twenty rules of formulating knowledge." supermemo.com
- Nielsen, M. "Augmenting Long-term Memory." (2018, essay)
- Anki manual + FSRS documentation

