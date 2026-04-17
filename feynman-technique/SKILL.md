---
name: feynman-technique
version: "0.1.0"
description: "Feynman Technique — a method of revealing gaps in understanding by explaining to a beginner. 4-step protocol (Choose → Teach → Identify gaps → Simplify). ELI5 approach. The fastest tool to break the illusion of competence."
---

# Feynman Technique

## Layer Position

**L3 (Understanding)** — Together with chunking, this belongs to the understanding layer. Before moving to L4 (retrieval/retention), it verifies whether concepts have been reconstructed in one's own language. Failing at Feynman = a signal of insufficient understanding → return to source material or redesign `chunking`.

## One-Line Summary

**If you can't explain it, you don't understand it.** Explaining to a beginner in your own words automatically exposes gaps in understanding.

## Theory & Origin

- **Richard Feynman (1918~1988)** — Nobel laureate physicist, legendary lecturer. Emphasized the "art of explanation" as his own learning method. However, the systematization into a "4-step technique" was not by Feynman himself but by later figures (mainly Scott Young and productivity blogs).
- Feynman's own practice: "Notebook of Things I Don't Know About" — writing down what he didn't know and reconstructing from first principles.
- **ELI5 ("Explain Like I'm 5")** — the same intuition extended in internet culture.
- Cognitive science basis:
  - **Self-explanation effect** (Chi et al. 1994) — students who attempt self-explanation show a significant increase in depth of understanding.
  - **Protégé effect** (Bargh & Schul 1980, Chase et al. 2009) — people who "learn while thinking they'll teach" actually learn better *by the measure of real learning*.
  - **Generation effect** (→ `active-recall`) — self-generated explanations stick in memory more strongly than received explanations.

## 4-Step Protocol

### 1. Choose (Topic Selection)
- Select one concept/problem you want to understand. Write down only the title.
- If it's too big, break it down. Not "quantum mechanics" but "Heisenberg uncertainty principle."

### 2. Teach (Write as if Teaching a Beginner)
- On a blank page/document, *assume you are teaching someone* and explain.
- In **your own language**. When technical terms appear, provide a plain-language rendering alongside.
- Use examples, analogies, and simple drawings.
- The standard is whether a 12-year-old can understand it (ELI5 is an exaggeration; the 12-year-old standard is practical).

### 3. Identify gaps (Detecting Blocks & Hand-Waving)
- Mark *points where you get stuck*, *points where you wave your hands*, and *points where you hide behind jargon* during explanation.
- "Um...", "so roughly speaking", "I don't know the details but" — all gaps.
- Return to source material (books, lectures) and re-study only those gaps.

### 4. Simplify & refine
- If still complex, find simpler analogies and examples.
- Repeat. Multiple rounds of simplification increase the density of understanding.
- The finished explanation should be recorded/noted — it becomes review material later.

## Why It Works

- **Hand-waving detection** — reading gives a "I know" feeling; speaking exposes gaps. The illusion of competence is broken.
- **Active retrieval** — explanation is high-intensity retrieval (→ `active-recall`).
- **Restructuring** — to explain to someone, you must reconstruct order, causality, and examples. This process is deep processing.
- **Feedback loop** — when stuck, immediately return to source. Learning becomes targeted.

## When to Use

- Learning where conceptual understanding is central (math, physics, economics, programming concepts, medical mechanisms)
- "I think I know it but can't explain it" symptom
- Final check of high-difficulty concepts before exams
- Self-check before presentations, lectures, or writing
- Verifying understanding after finishing a book or paper

## Practical Tips

### Use a Fake Audience
- *Imagine* a real 12-year-old child, a non-specialist friend, or a non-technical workplace colleague.
- "How would I explain this to my parents?"
- If possible, try it with an actual person. Real reactions are the strongest feedback.

### Use Recording / Video
- Explaining out loud alone reveals hand-waving through hearing.
- Video is hard to rewatch out of embarrassment but is most effective. Even without watching, the act of recording itself creates tension.

### Structured Simplification
- If you can't simplify in one pass, try a 3-tier structure:
  1. "This is X" (definition)
  2. "Why is it needed" (problem)
  3. "How does it work" (mechanism)
  4. "One example" (concrete)

### Time Limit
- One 25-minute session per topic (→ `pomodoro-and-focus`). Not perfection, but exposure.

### Using AI as a Feedback Channel

When mobilizing actual 12-year-old friends or non-specialist colleagues every time is difficult, you can use AI (ChatGPT, Claude, Gemini, etc.) as a **trained fake audience**. But the key is not "ask AI to write the explanation" but **"have AI verify your own explanation."**

**Workflow A — Audience Simulation**
1. Assign the AI a role: "You are a 12-year-old student who knows nothing about this topic. Every time I explain, ask questions only about the parts you don't understand. Don't encourage; point out only the gaps."
2. Paste your explanation as-is.
3. The AI's list of questions = the "hand-waved points." Return to source material only for those parts.
4. Paste the second explanation and repeat.

**Workflow B — Misconception Hunter**
1. Assign the AI a role: "You are an expert on this topic. In the explanation below, find incorrect concepts, inaccurate analogies, and missing premises. Don't use praise; list only errors."
2. The AI generally reacts with "that's a good explanation" excessively, so you must **explicitly request critical mode** for it to work.
3. Distinguish between grounded criticism and AI hallucination — reconfirm with source material/textbooks. (Use under the premise that AI sometimes gets it wrong.)

**Workflow C — Dunning-Kruger Prevention**
1. After finishing the explanation, ask the AI: "Generate 10 follow-up questions that naturally arise from hearing this explanation."
2. If you can't immediately answer 3 or more of these 10, depth of understanding is insufficient — relearn that range.

**Cautions:**
- AI is **not a complete substitute for a human audience.** The repeated "but why is that?" from a real non-specialist is still the strongest. Position AI as an *always-available auxiliary check loop*.
- If things drift toward AI *writing the explanation for you*, both the generation effect and self-explanation effect become void. The explanation must be written by you first.
- No tool brand dependence — prompt principles are the same across any LLM.

## Korean-Context Example

**Topic**: "Bayesian update"

**First explanation attempt**:
"Multiply the prior by the likelihood and normalize to get the posterior... um, what was normalization again?"
→ Gap found: Can't explain the meaning of the denominator (marginal likelihood).

**Return to source** → Reread the textbook's interpretation of the denominator.

**Second explanation (simplified)**:
"I was thinking the probability of rain is 20% (prior). But the sky is dark (evidence). The probability that the sky is dark on rainy days is 80%, and on non-rainy days is 30%. So having observed it's dark now, recalculate the probability of rain: (0.2 × 0.8) / (0.2 × 0.8 + 0.8 × 0.3) ≈ 40%. My belief has been updated from 20% → 40%."

→ Reconstructed with numbers, examples, and own language. The denominator is understood as "total possibility of darkness."

## Anti-Patterns

- **"Pretending to understand" explanation** — explanation covered up with jargon. Hiding the blocks. The exact opposite of Feynman.
- **Textbook sentence copy-paste** — reciting memorized sentences. Violates the own-language principle.
- **Skipping because no listener** — a real or imagined audience must be present for hand-waving to emerge.
- **Perfection in one pass** — the first explanation is normally messy. Repetition and refinement are the core.
- **ELI5 exaggeration** — trying to explain specialist concepts to an actual 5-year-old causes distortion. The 12-year-old / non-specialist standard is practical.
- **Analogies without depth** — if the analogy has a different structure than the original concept, it induces misunderstanding. Classical misunderstandings like "electrons are in planetary orbits."

## Limitations

1. **Unsuitable for factual memorization** — years, terms, and formulas are more efficiently handled by SRS. Feynman is an *understanding* tool.
2. **Partial for procedural skills** — explaining how to ride a bicycle doesn't teach how to ride one. Skills belong to `deliberate-practice`.
3. **Mistaking shallow understanding for deep understanding** — smooth explanation can still be Dunning-Kruger. Expert review is needed.
4. **No feedback when done alone** — questions from a real audience or tutor are the strongest signal.
5. **Topic selection bias** — tendency to choose only what's *easy to explain*. Training to deliberately choose difficult concepts is needed.
6. **Fatigue** — high-intensity cognitive activity. 25~40 minutes per session is the limit.

## What to Use Alongside This Framework

- **active-recall** — Feynman = high-difficulty free recall. Same family.
- **zettelkasten / evergreen-notes** — writing a permanent note is itself a Feynman process. Output remains.
- **metalearning** — the standard tool of Scott Young's *Ultralearning* projects.
- **spaced-repetition** — after understanding via Feynman, turn core claims into cards.
- **deliberate-practice** — if you repeatedly practice the act of explaining itself, the teaching skill itself improves.

## When This Framework Is *Wrong*

- Factual memorization → `spaced-repetition`
- Sports, instruments, performance, coding execution → `deliberate-practice`
- Can't focus in the first place → `deep-work` / `pomodoro-and-focus`
- Organization/arrangement is the problem → `second-brain-para`

## Further Reading

- Chi, M. T. H. et al. (1994). "Eliciting self-explanations improves understanding." *Cognitive Science.*
- Chase, C. C. et al. (2009). "Teachable agents and the protégé effect." *Journal of Science Education and Technology.*
- Young, S. (2019). *Ultralearning.* (Applies the Feynman technique at project scale)
- Gleick, J. (1992). *Genius: The Life and Science of Richard Feynman.* (Biographical background)
- "The Feynman Technique" — *Farnam Street* blog (popular summary, but note the 4-step formulation is a later addition)
