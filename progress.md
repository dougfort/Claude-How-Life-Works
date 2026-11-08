# How Life Works — Progress Log

Last updated: 2026-11-08

**How to use:** Start any session with "where were we?" Claude reads this log, gives one recall question from the last unit, and picks up at **Next up**. Sessions are short, one unit each; stopping mid-unit is fine.

---

## Where we are

- **Current theme:** Theme 0 — The standard picture
- **Next up:** A4: The genetic code and translation (codons, tRNA, ribosome).
- **Last recall prompt to use:** "Why can't the splice-site sequences alone pick out the real splice sites in a long gene?" (Target answer: each signal carries only ~8–9 bits, so chance matches occur about once every 2⁸ positions; their number grows with gene length, so a long gene has many cryptic sites that score as well as real ones; the signal can't tell them apart, and the cell uses additional context — splicing enhancers/silencers, exon definition, timing during transcription. Ask for the first clause unaided; watch for "external" instead of "additional/context.")

## Theme 0 units

Status: ☐ not started · ◐ in progress / partly covered · ☑ done

### Block A — Information: DNA → protein
- ☑ A1. DNA structure and copying (base pairing, semiconservative replication, proofreading). Completed 2026-11-06: full causal chain for leading/lagging strands stated correctly.
- ☑ A2. Transcription (RNA polymerase, promoters, transcription factors). Completed 2026-11-07: transcription direction stated precisely; K_d/occupancy chain stated correctly after step-by-step checks.
- ☑ A3. RNA processing (splicing, introns/exons, alternative splicing). Completed 2026-11-08: information-shortfall chain and window-model chain both stated correctly after step-by-step checks.
- ☐ A4. The genetic code and translation (codons, tRNA, ribosome)
- ☐ A5. Protein folding and shape (side chains, Anfinsen, chaperones)

### Block B — Energy
- ☐ B1. Free energy, equilibrium, and why life runs far from equilibrium
- ◐ B2. Enzymes and catalysis (barriers, transition states, Michaelis–Menten)
- ☐ B3. ATP as currency; coupling reactions
- ☐ B4. Glycolysis and respiration: overview
- ◐ B5. Chemiosmosis in depth (proton gradients, ATP synthase)
- ☐ B6. Lane's argument: energy and the origin of complex cells [research]

### Block C — Cells as physical objects
- ◐ C1. Scale and numbers (sizes, counts, timescales)
- ☐ C2. Diffusion and random walks
- ☐ C3. Crowding: what the inside of a cell is really like
- ◐ C4. Membranes and transport (bilayers, channels, pumps). Bilayer impermeability now correct (desolvation, Born energy); channels and pumps not yet covered.
- ☐ C5. Compartments and the cytoskeleton (prokaryote vs eukaryote)

### Theme 0 wrap-up
- ☐ Review quiz / flashcards

## Diagnostic results (2026-11-03 to 11-04)

| # | Topic | Result |
|---|---|---|
| 1 | Prokaryote vs eukaryote | Core fact right; missed why it matters |
| 2 | Membranes | Right instinct; "react" vs "interact" confused; check answer used wrong mechanism (charge repulsion) |
| 3 | DNA structure | Label right; missed copying mechanism |
| 4 | DNA → protein | Not recalled — **main gap** |
| 5 | Definition of a gene | Right direction; conflated consensus facts with Ball's interpretation |
| 6 | Proteins and catalysis | Strongest answer; refined to transition-state binding |
| 7 | ATP and energy | Currency ✓, storage ✗; energy source not known |
| 8 | Scale and speed | Size off by >10× (protein vs cell ≈ 4,000×); speed matched median enzyme only |

**Patterns to watch:**
- Answers name the thing but skip the "why." (Recurred 2026-11-05, 11-07, 11-08 on cryptic sites. Improving: 2026-11-08 window-model answer gave the mechanism unaided, missing only the last link.)
- Standard biology sometimes attributed to Ball.
- Mechanistic, physical reasoning is a strength.
- Spatial questions posed only in words don't land. Draw first, then ask. Fog can say "draw it" at any time.
- When stuck on a "why," smaller checks (yes/no, one-step) work better than open "explain in a sentence" prompts. Confirmed 2026-11-06, 11-07, 11-08. Current approach: ask for the first clause unaided, then fall back to one-step checks and a fill-in-the-blank.
- Direction words ("in the 3′ direction") get used loosely when two antiparallel molecules are involved. Ask which molecule.
- A remembered fact ("small K_d = tight binding") doesn't automatically connect to a formula. Point to the defining property (K_d *is* the half-occupancy concentration) before asking.
- New (2026-11-08): abbreviations and symbols introduced once (Pol II, ψ) don't carry over. Re-define at the point of use, especially inside a check question.
- New (2026-11-08): word precision — "replaced," "visible," "external" used where the mechanism needs "competitor appears," "unchallenged," "additional context." Mechanism right, wording loose.

## Open questions

(Questions Fog raises that we haven't resolved yet.)

- *(none yet)*

**Deferred threads (raised by Claude):**
- Ball's broad claim that alternative splicing shows the gene is a "resource," not a "program." Assessment so far: the narrow claim ("one gene, one protein" is false) is consensus; the broad claim doesn't follow from splicing alone, since the alternatives and the splicing factors are themselves encoded. Revisit in Theme 3 (cell states as network attractors).

## Session log

- **2026-11-03 to 11-04** — Theme 0 diagnostic, 8 questions plus checks. Set session format: short, irregular sessions, no numerical computation in checks. Started glossary (v1, 61 terms) and this log.
- **2026-11-05** — Recall (membranes): correct, right mechanism this time (loss of water shell). Added Born-energy formalization and the voltage part of the proton-motive force. Started A1: DNA structure, replication, accuracy and Hopfield proofreading; 5′/3′ directionality; leading vs lagging strands with an interactive fork diagram. Checks: "no lagging strand if strands were parallel" ✓; causal reason ✗ (attributed lag to waiting for exposed template, not to direction). A1 stays ◐. Session notes: `sessions/2026-11-05-A1-dna-copying.md`.
- **2026-11-06** — Recall (lagging strand): first answer named "growing away from the fork" but still gave waiting as the cause. Static fork diagram, then one-step checks: 3′ end of new bottom piece is away from the fork ✓; it can only grow away from the fork ✓. Fill-in-the-blank: 3′ end only + antiparallel → growing end points away → can't extend into new template → segmented ✓. A1 ☑.
- **2026-11-06 (later)** — Started A2. Covered: RNA polymerase reads one strand 5′→3′, template vs coding strand, small bubble not a fork, no primer, higher error rate and why that's tolerable; promoters set start and direction (sigma factor in bacteria; general transcription factors + Pol II in eukaryotes). Bubble diagram. Checks: "no lagging problem because it only opens one strand" — idea right, word wrong (opens both, reads one); one-step: RNA templated on the wrong strand would have 3′ end facing away ✓.
- **2026-11-07** — Recall (transcription direction): "only one strand is read" ✓ (word fixed); "in the 3′ direction" too vague — one-step check: RNA's growing 3′ end faces travel ✓. A2 chunk 3: regulatory transcription factors (activators, repressors, enhancers); occupancy θ = [T]/([T] + K_d) as a two-state partition function; same form as Michaelis–Menten; single site = soft dimmer; cooperativity → Hill function; thermodynamic-model caveat [research]; Ball on disordered, promiscuous factors (deferred to T2). Check (smaller K_d → lower half-occupancy concentration): stuck on open version; after pointing to K_d as the half-occupancy concentration, one-step checks ✓ ✓; added K_d = k_off/k_on; fill-in-the-blank ✓. A2 ☑. Glossary v3 (+16 terms, several entries updated).
- **2026-11-07 (later)** — Recall (single site = dimmer, cooperativity sharpens): asked for smaller steps; three one-step checks ✓ ✓ ✓; fill-in-the-blank ✓.
- **2026-11-08** — A3 chunk 1: cap, poly-A tail, splicing during transcription; splice signals (GU, AG, branch-point A); two-step lariat mechanism (diagram); spliceosome with RNA catalytic core; self-splicing introns as likely ancestor; information content of splice sites (~8–9 bits vs ~15 needed) → cryptic sites → enhancers/silencers, exon definition, timing. Check: unaided answer gave the conclusion ("can contain cryptic sites"), missed "many" and "can't tell apart"; one-step (doubling length doubles decoys) ✓; fill-in ✓, but "external" → corrected to "additional/context." A3 chunk 2: alternative splicing (cassette-exon diagram; patterns; Bcl-x, Dscam 38,016); functional-isoform dispute [research]; SR vs hnRNP competition; ψ = k_inc/(k_inc + k_skip); window-of-opportunity model P = 1 − e^(−kd/v) [research on generality]; Ball's "resource not program" reading and Claude's assessment (deferred to T3). Fog asked what "Pol II" meant (re-defined). Check: unaided answer got the window mechanism; corrected "replaced"/"visible"; ψ needed re-defining; then one-step completion ✓. A3 ☑. Glossary v4 (+20 terms, several entries updated).

## Files

- `glossary.md` — running glossary (v4, 2026-11-08)
- `progress.md` — this file
- `sessions/2026-11-05-A1-dna-copying.md` — notes from the 2026-11-05 session
