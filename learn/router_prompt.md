---
name: learn-router-prompt
version: "1.0.0"
description: "LLM-as-Router prompt template for selecting the optimal adult-learning / study-methods framework given a situation. Replaces keyword-matching Detection Matrix."
type: router_prompt
target_repo: learning-framework
---

# Learn Router — LLM Selection Prompt

This file is consumed by `pag_pipeline.py::route(repo="learning", question, router_llm)`.
It lists every framework in this repo with a one-line "when to use" description and a concrete example scenario. The router LLM is asked to return **exactly one framework name**.

---

## System Prompt

```
You are an adult-learning and study methods expert acting as a framework selector.
Given a situation, pick the SINGLE framework that best fits.

Output ONLY the framework name (lowercase, exactly as listed below). No explanation, no punctuation, no quotes.

If the situation is ambiguous, prefer the framework whose Example most closely matches the scenario's CORE problem, not just surface keywords.
```

---

## Framework Catalog

Each entry: `name` — **when to use** (one line) / **example** (one concrete scenario).

### Retrieval & Retention (getting it to stick)

**active-recall** — User passively re-reads, highlights, or watches lectures but can't reproduce the material; needs to switch to retrieval-based study.
Example: "I've read the textbook 3 times and highlighted everything, but I blank on practice problems. How do I actually study?"

**spaced-repetition** — User forgets memorized material within days or weeks; needs interval-based review (Anki, SM-2, FSRS) for long-term retention.
Example: "I learn Korean vocabulary but forget half the words a week later. How do I schedule reviews so they stick for months?"

**feynman-technique** — User thinks they understand a concept until asked to explain it; need gap-finding via teach-it-to-a-beginner protocol.
Example: "I nod along to the machine-learning lecture, but when a friend asks what backpropagation is, I can't explain it. How do I fix this?"

**interleaving** — User drills the same problem type for hours and does well on homework but fails on mixed-type exams.
Example: "I can solve 50 derivative problems in a row, but on the mock exam I freeze because I can't tell which technique to apply. What changes?"

### Skill Acquisition & Expertise

**deliberate-practice** — Intermediate or advanced practitioner is stuck on a skill plateau despite high practice volume; needs targeted weakness drills with feedback.
Example: "I've played guitar 5 years but my soloing hasn't improved in the last 2. How do I break the plateau beyond just playing more?"

**chunking** — User is overwhelmed by a field's volume of atoms (vocabulary, moves, patterns) and cannot hold enough in working memory to operate fluently.
Example: "Learning chess openings — there are thousands of lines and I can't remember any of them as coherent units. How do experts even do this?"

**metalearning** — User is starting a new field from scratch and needs to design their own curriculum (scope, resources, milestones, what to skip).
Example: "I'm switching careers into data science in 6 months. Where do I start, what should I skip, and how do I sequence the topics?"

### Focus & Time Management

**pomodoro-and-focus** — User cannot sustain even 25~30 minutes of focused work; needs to rebuild attention from a short-interval baseline.
Example: "I sit down to study and within 10 minutes I'm on my phone. I can't hold focus long enough to get anything done. Where do I start?"

**deep-work** — User can focus for short bursts but needs to architect multi-hour protected blocks for demanding cognitive work (research, writing, coding).
Example: "I can do 1 hour of thesis writing, then meetings and Slack destroy my day. How do I protect 3~4 hour blocks for deep work?"

### Knowledge Capture & Accumulation

**zettelkasten** — Researcher, writer, or lifelong learner wants a linked atomic-note system that compounds over years and generates writing drafts.
Example: "I read 2 papers a week but can't find anything I wrote down 6 months ago. How do I build a note system that actually pays off long-term?"

**evergreen-notes** — User takes disposable fleeting notes that never get revisited; needs to convert them into durable, refactored concept notes (Matuschak-style).
Example: "I have 500 disposable bullet-point notes from books I've read but they're all dead. How do I turn them into notes I actually reuse?"

**second-brain-para** — User is drowning in captured material (articles, PDFs, screenshots) and cannot find anything; needs Projects/Areas/Resources/Archives organization.
Example: "My Notion and Downloads folder have 3 years of saved articles and I can never find the one I need. How do I organize all this?"

---

## User Prompt Template

```
## Situation
{scenario}

## Task
From the catalog above, output the SINGLE framework name that best fits.

Answer (one word, lowercase):
```

---

## Routing Notes (for maintainers, not shown to LLM)

- **Ambiguous cases deliberately kept**: "can't remember what I read" → `active-recall` if the issue is passive study habit; → `zettelkasten` if the issue is a missing capture system for long-term knowledge.
- **`pomodoro-and-focus` vs `deep-work`**: pomodoro is the pick when the user cannot sustain even short focus; deep-work assumes focus baseline exists and needs block architecture.
- **`spaced-repetition` vs `active-recall`**: if the complaint is about *forgetting over time*, route SR; if the complaint is about *passive study method*, route active-recall.
- **`zettelkasten` vs `evergreen-notes` vs `second-brain-para`**: zettelkasten for atomic linked knowledge networks (research/writing output), evergreen for refactoring dead bullet notes into durable concept notes, PARA for organizing captured *material* by actionability.
- **`feynman-technique` vs `active-recall`**: Feynman when the user specifically reports the "I thought I knew it" illusion-of-competence pattern; active-recall when the input study method itself is wrong.
- **Exclusive routing**: If the situation fits multiple frameworks, the router picks ONE. Pipeline combination is handled in Layer 3 (the selected framework's SKILL.md may invoke others).
- **Not included here**: `learn` itself (this IS learn).

---

## Maintenance Protocol

Adding a new framework requires:
1. Add an entry to Framework Catalog above (name + when + example).
2. Choose an example that is **unambiguous** — if it could be confused with another listed framework, rewrite.
3. Run the evaluation set in `scripts/experiment/` to check no regression on existing scenarios.
