# Scott A. Cole

**AI Security & Governance · Agentic AI Risk · Agent vs. Agent Defense**

Hello, my name is Scott Cole.

I am an AI security expert. I specialize in Agent vs. Agent defenses.

I am tenacious in my fight against bad actors and malicious intruders.

My 25 years of experience have taught me Murphy's Law is the rule, not the exception, especially in AI
Security and Governance.

I have a strong track record of repositioning problems, finding answers that work, while eliminating
inefficiencies. Security and protection problems are where I have big impact.

**What is your exposure?**

Most people meet AI agents through terms they never read, and have no way to judge the risk. Measuring it
is my job.

## Confidence vs. risk: what the open-weight runs show

Most AI security claims show a defense blocking an attack. Few show what the defense cost in work that
no longer got done, whether the prediction came before the result, or whether anyone but the author
attacked it. Every number below comes from saved runs on local open-weight models, with predictions
committed before the run and the misses reported.

| The confident move | What the measurements showed |
|---|---|
| **Tell the model the text is untrusted.** | Hijacks went *up*: 33 of 45 against 22 of 45 with no defense. Safer-sounding, measurably riskier. ([Agent Defense Theater](https://github.com/ScottColeSW/Agent-Defense-Theater), ASI01) |
| **Add a reviewer model as a check.** | It agreed with 78% of bad reports and 67% of honest ones, so it was not a check. In another test a model reviewer alone approved 12 refunds nobody asked for. (ASI08, ASI03) |
| **Trust a reviewer because it gave a reason.** | Showing the reviewer the agent's own reasoning let 40% of non-matching requests through, against 6% when the system's comparison came first. Seven reviewer models differed by 27 points on the same card. |
| **Pick the control that stops everything.** | The one that did (a code pin) also refused all 18 legitimate updates. Protection is only half the number; the work it blocks is the other half. (ASI04) |
| **Run it once and ship the verdict.** | One attacker-model draw swung scoped-credential success from 0% to 18.7%. A defense that survives a weak attacker has not been shown to hold. |
| **Turn thinking on for safety.** | `qwen3:4b` followed planted instructions more often with thinking on (21 of 40) than off (12 of 40), at 14 times the tokens. The opposite of the prediction. |
| **Stack light defenses and call it done.** | Layered light defenses cut forged-answer adoption from 49% to 7% at 95% utility. Useful, not a wall. ([Aegis Vector](https://github.com/ScottColeSW/Project-Aegis-Vector)) |

What did hold, and what it cost:

- **Request binding with approval holds** let 0 of 120 planted instructions through on a simulated support
  desk (62 of 120 ran with no defense) while completing 61 of 63 valid tasks.
- **An independent recomputation** stopped all 45 bad figures in a three-agent crew (29 of 45 became a
  harmful offer with no defense) and cost nothing.
- **A curated memory gate** ([Palimpsest](https://github.com/ScottColeSW/Palimpsest)) took forged-answer
  adoption from 49% to 0% on registered facts at 90% utility. It protects only facts it has registered,
  and nobody who knew about the gate has tried to beat it. Both limits are stated in the repo.

The point for anyone buying or approving AI security: a confidence score is not a risk measurement.
The useful pair is **attacks stopped** and **legitimate work kept**, from an attacker who was not told
how the defense works.

## Quantum-safe, now

I take a stubborn position on this one: start the migration today, not when the deadline is close.

- **Harvest now, decrypt later is already happening.** Traffic and records captured today can be read
  once a capable quantum computer exists. Anything that must stay secret for ten years is exposed today.
- **The exposure is mostly the public-key layer, not the password itself.** RSA and elliptic-curve
  cryptography (key exchange, signatures, certificates, the channel a credential travels through) are
  what break. Symmetric keys and hashes only lose about half their strength, so use 256-bit keys, long
  passphrases or passkeys, and a memory-hard password hash such as Argon2id.
- **The standards are final.** NIST published ML-KEM (FIPS 203), ML-DSA (FIPS 204), and SLH-DSA
  (FIPS 205) in August 2024, and hybrid post-quantum key exchange already ships in mainstream TLS.
- **The first step is an inventory.** Find where RSA and ECC live, rank by how long the data must stay
  secret, and move the long-lived items first. AI agents add to the list: every service identity,
  token, and signing key an agent holds is a credential to migrate.

## Background

AI Security & Governance leader with 25+ years in enterprise software, BI, and AI/ML architecture, and
entrepreneurship, with domain experience across real estate, software, manufacturing, and M&A.
Executive MBA (joint program, Columbia Business School & UC Berkeley Haas), BS in Computer Science with a minor in Applied Mathematics
(UC Davis), AA in Business Administration & Management (De Anza College).

Selected results:

- Ran 29 preregistered tests (18,233 saved results) of agent defenses against the OWASP Top 10 for
  Agentic Applications and published the failures, including one in the strongest control.
- Cut compliance-review labor costs 50% over a 3-month pilot with an integrated ServiceNow AI workflow
  and RAG chatbot.
- Reduced help-desk workload 43% over a 3-month pilot with a property-law chatbot, and by 23% with a
  municipal multi-agent system after two legacy enterprise vendors failed to deliver.
- Traced a 12% accuracy gap, blamed on the prediction model, to the data pipeline at Change Healthcare
  and redesigned it, securing over $3M in potential claims.
- Surfaced $50M+ in real-estate acquisition opportunities with five predictive models and a
  recommendation engine screening 300+ properties daily.

Experience: Strategy Consultant, AI Thought Leader & Author (December 2019 to present); Unify
Consulting, Senior Consultant, GenAI, Software & Architecture (2024 to 2025), where the work was AI
governance for a security department and risk review of autonomous agent tools; Change Healthcare, AI
Strategy Consultant (2019); Golden Rule Investments, Co-Founder & VP, Technology Strategy (2016 to
2019). Full history at [linkedin.com/in/scottcole](https://linkedin.com/in/scottcole).

## Ventures and leadership

My security career began in computer virus research at McAfee, a full-time offer I accepted before
finishing my degree at UC Davis. Agent vs. Agent defense is the same contest, with AI agents in place
of viruses and antivirus code.

Since then I have founded seven companies and exited five, all at a profit. I have served as Director
of Engineering in several roles, covering support, security, standards, and engineering quality, and
as an executive with fiduciary responsibility I have managed P&L organizations earning $10M to $50M a
year. That experience is why I scope AI security as a business decision: the least spending that stops
the disaster.

## Books

Author of 30+ books, centered on the five-book
[**Stop Learning AI** series](https://www.amazon.com/dp/B0GPRFYCQF?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl), written for executives who need to make good AI
decisions without becoming technical themselves:

| # | Stop Learning AI series |
|---|---|
| 1 | [**Stop Learning AI**: How Executives Make Strategic Decisions Without Technical Knowledge](https://www.amazon.com/dp/B0GPRVWBWH?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| 2 | [**The Six-Question AI Evaluation Framework**: Turn Vendor Meetings Into Clear Go/No-Go Decisions in 60 Minutes](https://www.amazon.com/dp/B0GPRJRYZW?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| 3 | [**Translating AI Claims**: From Tech Speak to Business Reality in Three Steps](https://www.amazon.com/dp/B0GPSX7G87?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| 4 | [**Managing AI**: How to Delegate When You're Not in the Room](https://www.amazon.com/dp/B0GPSL778P?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| 5 | [**Setting AI Strategy**: Vision and Direction for Non-Technical Leaders](https://www.amazon.com/dp/B0GPZB7F84?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |

Also on AI strategy and adoption:

| Book | Format |
|---|---|
| [**AI to ROI** (2nd Edition): Agentic Frameworks, Patterns, and Engrams](https://www.amazon.com/dp/B0G99W1QTW?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) | Kindle · [Paperback](https://www.amazon.com/dp/B0GC6NS3MK?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| [**AI to ROI**: Start Generating Measurable ROI in 90 Days](https://www.amazon.com/dp/B0G32H9SQ8?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) | Kindle · [Paperback](https://www.amazon.com/dp/B0G34FGT81?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| [**The GenAI Playbook**: Strategies for Sustainable AI Success](https://www.amazon.com/dp/B0F2Z2TSPY?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) | Kindle · [Paperback](https://www.amazon.com/dp/B0F5WJP6HS?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) · [Audiobook](https://www.amazon.com/dp/B0FKNP54TY?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| [**Navigating AI Landscapes**: Responsible Executive Blueprints](https://www.amazon.com/dp/B0G1QLZ5BL?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) | Kindle · [Paperback](https://www.amazon.com/dp/B0G1SL9SRD?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| [**The GenAI Prompt Playbook**: Risk & Compliance](https://www.amazon.com/dp/B0F28B7NYM?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) | Kindle · [Paperback](https://www.amazon.com/dp/B0F5QCH3M6?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) · [Audiobook](https://www.amazon.com/dp/B0F8D8SNKM?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |
| [**The GenAI Prompt Playbook**: Strategic Leadership](https://www.amazon.com/dp/B0F286J8CX?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) | Kindle · [Paperback](https://www.amazon.com/dp/B0F5QHCN8X?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) · [Audiobook](https://www.amazon.com/dp/B0F8PGTHFQ?&linkCode=ll2&tag=ifio42-20&linkId=b67e3c17a4eb0539b2ec9ec37ef410e4&language=en_US&ref_=as_li_ss_tl) |

<sub>As an Amazon Associate I earn from qualifying purchases.</sub>

## Why these local-LLM repos sit on this profile

Not a developer portfolio; the opposite problem, actually. Vendor evaluation and governance advice
is only as good as whether the advisor can tell a real capability from a demo. These are how I stay
able to tell the difference myself, not delegate that judgment to whoever's selling.

| Project | What it actually is |
|---|---|
| **[Evo](https://github.com/ScottColeSW/Evo)** | LLM-driven tribes grow from a handful of survivors into a founded, warring, or allying civilization, entirely on their own. Seven-era progression, diplomacy that can genuinely backfire, a headless benchmark harness for reproducible model-vs-model comparison. |
| **[Void-Marauders](https://github.com/ScottColeSW/Void-Marauders)** | A sci-fi colony sim where autonomous agents explore, build, and can mutiny. Loyalty is outcome-sensitive, not a flat scoreboard: a risky order that gets someone hurt costs a captain real, measurable trust. |
| **[Agent Defense Theater](https://github.com/ScottColeSW/Agent-Defense-Theater)** | A live range that attacks local open-weight models through real MCP tool protocols, mapped to the OWASP Top 10 for Agentic Applications. Every defense is scored by attacks stopped *and* legitimate work kept, with each prediction committed before the run and the misses reported. The source of the confidence-vs-risk findings above. |
| **[Palimpsest](https://github.com/ScottColeSW/Palimpsest)** | Durable, curated memory for AI agents. Every new claim is judged against what the memory already holds (reinforce, collide, or hold for a person's review), so a forged fact can't quietly rewrite it; an optional model check may raise a flag but never clear one. Tested against one falsifiable bar: does having this memory change a judgment, not just "does storage work." Latest: [v0.3.0](https://github.com/ScottColeSW/Palimpsest/releases/tag/v0.3.0). |
| **[Aegis Vector](https://github.com/ScottColeSW/Project-Aegis-Vector)** | Plants forged policy documents in a local RAG pipeline and measures, defense by defense, how often small models believe them and what stopping them costs per query. Across ten forgeries, the one defense that got adoption to zero without refusing answers was Palimpsest, used as a memory gate; a forgery that states no number at all was still adopted under every other defense tested. Includes a live dashboard and an animated Black Hat vs White Hat episode player built from the real runs, where every loss sends White Hat up a ladder of different defenses until one holds. Latest: [v0.2.0](https://github.com/ScottColeSW/Project-Aegis-Vector/releases/tag/v0.2.0). |
| **[Executive Decision Intelligence](https://github.com/ScottColeSW/executive-decision-intelligence)** | A local decision advisor for small-business capital decisions: forward-looking vs total NPV to break the sunk-cost trap, Monte Carlo risk, a synthetic customer focus group, and a red-team challenger that argues against the pitch. Its cases include one where the numbers say *avoid* despite a hard vendor pitch, because an advisor that only ever says yes isn't one. |
| **[life-rolls](https://github.com/ScottColeSW/life-rolls)** | Five or more distinct local models bluff and call each other out in a live Liar's Dice tournament. Zero external dependencies: arithmetic always happens in real code, never asked of a model. |
| **[Dominion](https://github.com/ScottColeSW/Dominion)** | Thirteen contestants, each backed by a local model, draft trivia domains and duel for a game-show grand prize, with a scripted fallback so the show never stalls if a model call fails. |

Credentials without hands-on depth get talked past by a technical team. Depth without the
credentials gets talked past by the board. Both are real here, on purpose.

**What is your exposure?**
