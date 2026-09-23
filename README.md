# Scott Cole

I build multi-agent systems where local LLMs are the actual decision-makers — not a chat
wrapper around one model, real autonomous agents, under real hardware constraints (8GB-class
consumer GPUs, zero cloud API cost), with honest documentation of what works and what still
doesn't.

Five projects, one specialty:

| Project | What it actually is |
|---|---|
| **[Evo](https://github.com/ScottColeSW/Evo)** | LLM-driven tribes grow from a handful of survivors into a founded, warring, or allying civilization — entirely on their own. Seven-era progression, a five-tier Maslow read on each tribe's condition, diplomacy that can genuinely backfire into war, and a headless benchmark harness for reproducible model-vs-model comparison. |
| **[Void-Marauders](https://github.com/ScottColeSW/Void-Marauders)** | A sci-fi colony sim where a crew of autonomous agents explores, builds, and can mutiny — loyalty is outcome-sensitive, not a flat scoreboard: a risky order that gets someone hurt costs a captain real trust, and it's directly measurable. |
| **[Palimpsest](https://github.com/ScottColeSW/Palimpsest)** | The memory substrate the other projects actually run on. Curated, not total recall; weight that stays legible instead of vanishing. Tested against one falsifiable bar — does having this memory change a judgment, not just "does storage work." |
| **[life-rolls](https://github.com/ScottColeSW/life-rolls)** | Five or more distinct local models bluff and call each other out in a live Liar's Dice tournament. Zero external dependencies — arithmetic always happens in real code, never asked of a model. |
| **[Dominion](https://github.com/ScottColeSW/Dominion)** | Thirteen contestants, each backed by a local model, draft trivia domains and duel for a game-show grand prize — with a scripted fallback so the show never stalls if a model call fails. |

## What actually differentiates this work

- **The model only ever proposes; the system stays authoritative.** Every project deterministically
  validates and applies what an agent decides — an LLM never directly mutates world state.
- **Small, local, resource-constrained on purpose.** Everything here runs on consumer-grade
  hardware, not a hosted API — part of what gets measured is exactly how (and whether) a small
  quantized model reasons under real constraints.
- **Honest about limits, not just capabilities.** Every README here says what's unverified, what's
  still scripted rather than learned, and what's a deliberate boundary rather than a gap — Palimpsest's
  own docs draw a line at cross-model memory sharing on purpose, not because it's unsolved by accident.
- **Real tests that prove something, not just that code runs.** Palimpsest's suite specifically checks
  "does memory present change the outcome vs. memory absent" — not just that storage works.

---

📍 Connect: [linkedin.com/in/scottcole](https://linkedin.com/in/scottcole)
