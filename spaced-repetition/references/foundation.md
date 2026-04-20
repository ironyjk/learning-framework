# Spaced Repetition -- Theoretical Foundation

## One-Line Summary

When you retrieve something **just before you're about to forget it**, retention duration grows exponentially. The algorithm computes the optimal interval; the human only performs the retrieval.

## Theoretical & Research Origins

- **Hermann Ebbinghaus (1885)** — *Über das Gedächtnis.* Self-experimentation with nonsense syllables. Discovered the forgetting curve: rapid forgetting immediately after learning, then gradual decay. With repeated study, the curve flattens (saving).
- **Cecil Alec Mace (1932)** — suggested the advantage of spaced-out review.
- **Sebastian Leitner (1972)** — *So lernt man lernen*. Paper-card box system. Correctly-answered cards move to boxes with longer intervals. (Atkinson 1972 is an independent theoretical study of spaced learning.)
- **Piotr Wozniak (1985~)** — SuperMemo. Released the SM-2 algorithm (1990) → the foundation for Anki, Mnemosyne, and RemNote.
- **FSRS (2022~)** — Free Spaced Repetition Scheduler. Based on a memory model (DSR: Difficulty, Stability, Retrievability), integrated into recent versions of Anki.
- Core empirical finding: **spacing effect** — for the same time investment, spaced learning > massed learning (Cepeda et al. 2006, a quantitative meta-analysis of 184 experiments).

## Core Concepts

### 1. Forgetting Curve
- The probability of remembering a newly learned item, R(t), decreases with time t.
- Common approximation: $R(t) = e^{-t/S}$ (S = stability)
- After review, S increases → subsequent decay is more gradual.

### 2. Interval Optimization
- Review too early: little effect (you still remember).
- Too late: it becomes relearning.
- **Optimal point: "just before" forgetting** — when retrieval effort is high, the increase in S is maximized.
- SM-2: interval multiplier (ease factor) ~2.5, restarts on recall failure.
- FSRS: estimates S and D individually per card and computes intervals to match a target retention rate (e.g., 90%).

### 3. Active Retrieval Is a Prerequisite
- SRS is not simply "scheduled rereading." The key is stating the answer *before* looking at the back of the card. (→ `active-recall`)
- Looking at the answer → pressing "Easy" without effort neutralizes SRS.

### 4. Card Atomicity
- One card = one fact. "Q: What year did the Korean War begin? A: 1950"
- Cards mixing multiple facts turn partial memory into full failure, or vice versa.
- **Minimum information principle** (Wozniak) — if it can be split, split it.

