---
name: chunking
version: "0.1.0"
description: "Chunking — Miller's 7±2 short-term memory constraint, expert chunk perception, and chunk-size calibration in learning design. Meaningless individual items → meaningful chunks = expanded processing capacity. The core representational unit of expertise."
---

# Chunking

## Layer Position

**L3 (Understanding · Representation)** — alongside feynman-technique in the understanding layer. Individual elements → meaning units → higher-order schemas. The representational unit that determines the quality of L4 (retrieval) and L5 (transfer).

## One-Line Summary

**Human working memory is small** (~7±2 items). But when organized into *meaningful bundles (chunks)*, a single "item" becomes a rich informational package. This is precisely the representational difference that separates experts from novices.

## Theoretical / Research Origins

- **George A. Miller (1956)** — "The Magical Number Seven, Plus or Minus Two." *Psychological Review.* Proposed the 7±2 working memory limit. However, Miller himself warned that "the exact number is not what matters — what matters is that it is *finite*."
- **Nelson Cowan (2001)** — *Behavioral and Brain Sciences.* Reanalysis suggested the actual capacity is closer to **4±1** chunks. The current academic mainstream view.
- **Chase & Simon (1973)** — Chess expert vs. novice experiments. Experts overwhelmingly outperformed on real game positions, but the gap *shrank dramatically* with randomly arranged pieces (though follow-up research showed some slight advantage remained). Conclusion: expert superiority derives not from general memory but from *chunk-based pattern perception*.
- **Gobet & Simon (1996)** — Estimated that expert chess players hold roughly 50,000 chunks in long-term memory (template theory).
- **Ericsson & Chase (1982)** — Even ordinary people, through training, expanded digit-memory capacity from 7 to 80+ (subject SF). However, such training is confined to the specific domain.

## Core Concepts

### 1. Working Memory
- The *one-shot capacity* of information that can be consciously handled. The bottleneck for processing and learning new information.
- 7±2 (items) or 4±1 (chunks) — *finiteness* matters more than the number.
- Vulnerable to fatigue, stress, and sleep deprivation.

### 2. Chunk
- *A unit with meaning*. Examples:
  - Meaningless digits `1-9-4-5-0-6-2-5` (8 items)
  - Chunked `1945` (Korean Liberation) + `0625` (Korean War) (2 chunks)
- Same information, different representation. Capacity expanded 4×.

### 3. Expert Perception
- Novice: individual elements (a single chess piece, a single line of code, a single patient symptom)
- Expert: patterns and schemas (this position is the 'Ruy Lopez opening,' this code is the 'Singleton pattern,' this symptom cluster is 'heart failure')
- Experts *already see in chunks at the perceptual stage*. Pre-inference.

### 4. Long-Term Memory Offloading
- Chunks are *templates* stored in long-term memory. Working memory references them.
- Learning = the process of building new templates in long-term memory + raising retrieval speed.

### 5. Cognitive Load Theory (Sweller)
- Intrinsic load (essential complexity of the task) + extraneous load (unnecessary elements) + germane load (cognition spent on schema formation)
- Learning design reduces extraneous load + supports germane load.

## When to Use

- **Entering a complex topic** — split into chunks and build progressively
- **Acquiring a new field** — reverse-engineer the expert's chunks
- **Designing learning materials / lectures**
- **Memory training** (digits, words, cards)
- **Interpretation training for code, formulas, sheet music**

## Practical Application

### 1. Learner Perspective: Chunk Construction
- When encountering a new topic, build the hierarchy *elements → chunks → higher-order chunks*.
- Example: Learning programming
  - Level 1 elements: variables, functions, conditionals
  - Level 2 chunks: loop patterns, error handling
  - Level 3 chunks: design patterns (Observer, Factory)
  - Level 4 chunks: architecture patterns (MVC, Event Sourcing)
- Higher-order chunks contain lower ones. Expand only one layer at a time.

### 2. Reverse-Engineering Expert Chunks
- Observe which units experts in the field perceive in.
- Asking "How do you see this position?" reveals chunk naming.
- Textbook tables of contents often hint at the chunk hierarchy.

### 3. Designer Perspective: Chunk-Size Calibration
- Keep new elements presented at once to 4–5 or fewer.
- Break examples, exercises, and explanations by chunk.
- Introduce the next chunk only after mastering the previous one ("scaffolding").

### 4. Integrating Practice
- Master individual chunks → practice combining chunks → fluid execution.
- The "part → whole" training order is generally effective, but for highly complex skills, *starting within context from the beginning* may be better (Whole-Part-Whole).

### 5. Developing Notation
- Externalize chunks with personal abbreviations, icons, and diagrams.
- Note headings and formatting mark chunk boundaries.

## Korean Context Examples

**Memorizing Korean history dates**:
- Un-chunked: "1592 1598 1623 1636 1645 1876 1894 1905 1910 1945 1948 1950 1953 1960..."
- Chunked: "Imjin War (1592–1598) → Injo Restoration (1623) → Byeongja War (1636) → Port Opening (1876) → Gabo Reform (1894) → Eulsa Treaty (1905) → Japanese Annexation (1910) → Liberation (1945) → Government Established (1948) → 6·25 (1950–1953) → 4·19 (1960)..."
- Chunks are *event names*. Bundle 4–5 chunks into higher-order narratives (Late Joseon / Enlightenment Era / Japanese Occupation / Modern).

**Memorizing herbal medicine (本草)**:
- Brute-forcing 300+ medicinal herbs = impossible
- Chunk by efficacy groups: exterior-releasing herbs, heat-clearing herbs, purgatives, wind-expelling herbs... and further subdivide within each group.
- Experts reason in three tiers: "this symptom → which group → which herb."

## Antipatterns

- **Obsessing over the number 7** — Miller himself emphasized *finiteness* over the number. The latest research says 4±1.
- **No chunking, all at once** — If a lecture or textbook dumps 20 new elements at once, learning becomes impossible. Extraneous load accumulates.
- **Memorizing chunks without knowing their interior** — Knowing only the terminology. Must verify by descending to the elements inside the chunk (Feynman).
- **Transplanting chunks across fields** — Chunks from one field are valid only in that field. A chess expert cannot chunk-perceive a Go position (Chase & Simon).
- **Bragging about learning speed** — "100 words per day" is extraneous-load overkill. Actual retention is low.

## Limitations

1. **Oversimplification of chunk numbers** — Miller's 7±2 is not Magic. Context, training, and individual differences are large.
2. **Domain-dependent** — Chunks form within the field. They do not generalize.
3. **Long training period** — Thousands to tens of thousands of expert chunks accumulate over years or decades.
4. **Limits of conscious control** — Chunk formation is largely implicit and unconscious. Design only shapes the environment.
5. **Chunk ≠ Understanding** — One may be strong in pattern recognition but ignorant of mechanisms. Only part of expertise.

## What to Use Alongside This Framework

- **deliberate-practice** — Deliberately practice one chunk at a time → automate → form higher-order chunks.
- **spaced-repetition** — Turning chunks into cards reinforces retrieval.
- **active-recall** — Chunk-unit retrieval training.
- **feynman-technique** — Whether you can explain the interior of a chunk is the verification of understanding.
- **metalearning** — When designing the learning of a new field, start by mapping the chunk structure.

## When This Framework *Is Wrong*

- The trap of memorizing chunks without understanding → `feynman-technique`
- Chunks that don't retrieve → `active-recall` / `spaced-repetition`
- Skill execution problems → `deliberate-practice`
- Focus problems → `deep-work` / `pomodoro-and-focus`

## Further Reading

- Miller, G. A. (1956). "The Magical Number Seven, Plus or Minus Two." *Psychological Review.*
- Cowan, N. (2001). "The magical number 4 in short-term memory: A reconsideration of mental storage capacity." *Behavioral and Brain Sciences.*
- Chase, W. G. & Simon, H. A. (1973). "Perception in chess." *Cognitive Psychology.*
- Gobet, F. & Simon, H. A. (1996). "Templates in chess memory: A mechanism for recalling several boards." *Cognitive Psychology.*
- Sweller, J. (1988). "Cognitive load during problem solving: Effects on learning." *Cognitive Science.*
- Ericsson, K. A. & Chase, W. G. (1982). "Exceptional memory." *American Scientist.*
