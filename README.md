# Learning Framework

[한국어](README.ko.md) | **English**

---

A meta-router + framework collection for adult learning and knowledge management. Bundles 12 evidence-based frameworks from cognitive science and educational psychology research under a single routing layer.

## Design Principles

1. **Research over self-help narrative** — Starts from empirical research (Ebbinghaus, Roediger, Karpicke, Dunlosky, Ericsson, Bjork, Cepeda) rather than "habits of geniuses" or "the X rule." Claims with weak evidence (VAK learning styles, left/right brain, speed reading, the 10,000-hour rule, 1-minute memory techniques, etc.) are excluded or explicitly corrected.
2. **Principles, not tools** — No promotion of specific apps (Obsidian, Notion, Anki, Logseq, Roam). Tools are mentioned neutrally as needed.
3. **No single silver-bullet framework** — Assumes knowledge capture (Zettelkasten), retention (Spaced Repetition), and comprehension verification (Feynman) need to be *combined*.
4. **Anti-pattern warnings included** — Explicit notes on when each framework misleads or causes harm.
5. **Desirable difficulty throughout** — Bjork: comfortable studying (highlighting, re-reading, consuming summaries) is usually less learning. Subjective ease and actual learning outcomes are inversely correlated.
6. **Self-directed ≠ isolated** — Coaches, study groups, AI, and online courses are integrated as external feedback channels. Flying solo solidifies blind spots.
7. **Korean learning context built-in** — Korean exam culture (수능 CSAT, 공무원 civil service, 자격증 certifications: licensed real estate agent, CPA, PMP), 회독 (multi-pass reading), 오답노트 (error notebooks), N수 (retaking exams), and 인강 (online lecture) culture are used as examples throughout.

## Structure

```
learning-framework/
├── SKILL.md                   # Meta-router — situation → framework selection
├── zettelkasten/              # Luhmann atomic notes & linking
├── second-brain-para/         # Tiago Forte PARA · CODE
├── evergreen-notes/           # Andy Matuschak concept-oriented, continuously edited
├── spaced-repetition/         # Ebbinghaus forgetting curve · SM-2
├── active-recall/             # Roediger & Karpicke testing effect
├── feynman-technique/         # Verify understanding through explanation
├── interleaving/              # Bjork mixed-topic practice
├── deliberate-practice/       # Ericsson intentional practice
├── chunking/                  # Miller chunking · expert perception
├── deep-work/                 # Cal Newport focused work
├── pomodoro-and-focus/        # Cirillo 25/5 + attention residue
└── metalearning/              # Oakley + Young meta-learning
```

## Usage

```
/learn <situation description>
```

The meta-router classifies goal (exam / skill / knowledge accumulation) and constraints (time, tools), selects 1–3 relevant frameworks, and executes/synthesizes via the Skill tool.

> 💡 **Short name**: after [wrapper setup](https://github.com/ironyjk/claude-frameworks-marketplace#short-command-setup-optional), callable as `/learn`

## Out of Scope

- Children's and adolescent education (→ `parenting`, `udl`, `pbl`, etc.)
- Communication and negotiation learning (→ `howtotalk`)
- Psychotherapy and emotional learning (→ `counsel`)
- Organizational learning and team skills (→ `team-topologies`)

This repo focuses on adults learning independently, accumulating knowledge, and building expertise.

## Meta

- `last_verified: 2026-04-17`
- `valid_until: 2027-04-17` — Cognitive science and educational psychology evidence has a long lifespan; 1-year re-verification cycle. Korean exam system changes (수능 CSAT, civil service, CPA reform) trigger immediate updates.

## Disclaimer

This repo is a learning-design support tool. Licensing exams, professional certifications, and clinical domains (medicine, law, etc.) may require additional strategies beyond what is covered here.

## Attribution & Trademarks

This project implements evidence-based learning frameworks for educational purposes. The following trademarks are acknowledged:

- **Pomodoro Technique®** is a registered trademark of Francesco Cirillo (cirillocompany.de).
- **Building a Second Brain™** and **PARA** are trademarks of Tiago Forte / Forte Labs.
- **Ultralearning** is a methodology by Scott H. Young.

All other framework names reference published academic works and are used descriptively.

This project is not affiliated with, endorsed by, or sponsored by any of the above trademark holders.

## License

CC-BY-NC-4.0 — see [LICENSE](LICENSE) for details. Commercial licensing: ironyjk@gmail.com
