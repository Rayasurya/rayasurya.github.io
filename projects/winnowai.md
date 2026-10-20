# WinnowAI: A multi-agent AI workspace that drug-safety scientists can follow, question and sign off on.

- When: 2026
- Type: AI product design, working prototype (version 8)
- Case study: https://rayasurya.com/projects/winnowai/
- Prototype: https://rayasurya.com/winnow/
- Slides (PDF): https://rayasurya.com/decks/winnowai.pdf

**The domain.** In pharmacovigilance, scientists read post-market safety reports for signals: early signs of an unknown side effect. Serious reports must be filed within 15 calendar days, and an AI answer that cannot be traced is not usable in a regulatory filing.

**What Raya designed.** A 4+1 agent system: a Planner that orchestrates, a Data Compiler, a Medical Reviewer and a PHI Guard, plus a hidden UI agent. Each agent has its own shape so a scientist can tell them apart. Every hand-off is logged, every AI summary sits next to the raw report it came from, patient identifiers are always removed, and nothing is filed until a named scientist signs.

**Evaluation.** 22 hand-written drug-event cases scored against a 12 August 2026 snapshot of openFDA: 0 missed signals (recall 100%), 6 false alarms (precision 60%), 64% of verdicts right overall. It caught 0 of 6 confounded pairs: it cannot tell a drug that causes an outcome from one given to people who already have it. That limit is why a scientist must sign.

**Honesty notes.** A working prototype, not a production system. The persona and the time savings shown in the case study are illustrative estimates.

---
More about Raya Surya: https://rayasurya.github.io/llms-full.txt · Contact: raya.work.ux@gmail.com
