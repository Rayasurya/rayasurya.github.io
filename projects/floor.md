# Floor: A tool that shows where goods can legally go in a shared warehouse, given what sits next to them.

- When: September 2026
- Type: Product design take-home, working prototype
- Case study: https://rayasurya.com/projects/floor/
- Live prototype: https://rayasurya.com/floor/
- Slides (PDF): https://rayasurya.com/decks/floor.pdf

**The problem.** In GodownX, a shared warehouse run by two or three ops staff, a spreadsheet can say a zone is empty but not who it is empty for. Food next to chemicals breaks the law; two tenants can want the same zone.

**The idea.** A zone is never just free. It is free for someone, given what sits next to it.

**What Raya designed.** A floor map whose colours come from a rules engine: distance between zones (12 m per grid step, diagonals included) checked against a minimum distance per pair of goods classes (food and chemicals 24 m, no barrier allowed). A blocked request returns a ladder of fixes instead of a no, and a refusal comes with a date and a way out. When two requests want one zone, the one that removes fewer future legal placements wins (Vertex in C4 would remove 4 of 11 zones from food use, Raheja none).

**AI boundary.** Legality and floor cost are plain code, so the answer is the same every time. AI only helps on request and never gives a verdict.

**Process.** Desk research only (no warehouse staff interviewed). 14 assumptions and 30 decisions written down. The rules engine passes 10 of 10 checks. Seven screens, desktop plus a phone floor check.

**Honesty notes.** Rules are simplified from FSSAI and NFPA 400 guidance; illustrative, not a compliance ruleset. All data is simulated.

---
More about Raya Surya: https://rayasurya.github.io/llms-full.txt · Contact: raya.work.ux@gmail.com
