# How Life Works — Progress Log

Last updated: 2026-11-19

**How to use:** Start any session with "where were we?" Claude reads this log, gives one recall question from the last unit, and picks up at **Next up**. Sessions are short, one unit each; stopping mid-unit is fine. **End every session with a session-notes markdown file** (`sessions/YYYY-MM-DD-<unit>-<topic>.md`): content taught, diagrams as ASCII, checks with Fog's answers and feedback, terms introduced, next recall prompt with the answer in a collapsible `<details>` block. Quizzes are also delivered as saveable markdown, answers in `<details>`.

***

## Where we are

* **Current theme:** Theme 0 — The standard picture
* **Order for Blocks B/C (chosen 2026-11-16):** interleave — C1 → C2 → B1 → B2, then alternate through the rest of B and C.
* **Next up:** C2 chunk 2 — diffusion equation and Fick's law; diffusion-limited reaction rates; lac repressor's facilitated search (sliding along DNA) \[research].
* **Recall prompts to use next session:** two, both in `sessions/2026-11-18-C2-chunk1-diffusion-random-walks.md`: (1) C2 chunk 1 — the squaring step (1,000× the distance → \~1,000,000× the time); (2) Block A quiz Q4 — K_d, k_on vs. k_off, occupancy curve shift.
* **Block A quiz:** skipped by Fog's choice 2026-11-16; stays saved. Questions folded into recalls, one per session. **Q1 re-tested ✓ 2026-11-18** (after correction). Remaining key chains: Q4 (next), Q5, Q8, Q9.
* **Glossary:** C2 terms pending — add when C2 is complete (list in the 2026-11-18 session notes).

## Theme 0 units

Status: ☐ not started · ◐ in progress / partly covered · ☑ done · ⊘ skipped

### Block A — Information: DNA → protein

* ☑ A1. DNA structure and copying (base pairing, semiconservative replication, proofreading). Completed 2026-11-06: full causal chain for leading/lagging strands stated correctly.
* ☑ A2. Transcription (RNA polymerase, promoters, transcription factors). Completed 2026-11-07: transcription direction stated precisely; K_d/occupancy chain stated correctly after step-by-step checks.
* ☑ A3. RNA processing (splicing, introns/exons, alternative splicing). Completed 2026-11-08: information-shortfall chain and window-model chain both stated correctly after step-by-step checks.
* ☑ A4. The genetic code and translation (codons, tRNA, ribosome). Chunk 1 (code, reading frames, tRNA + synthetases, editing) 2026-11-09; chunk 2 (ribosome) completed 2026-11-10: nonsense-codon chain stated correctly unaided.
* ☑ A5. Protein folding and shape (side chains, Anfinsen, chaperones, misfolding, disordered proteins). Chunk 1 2026-11-11/12. Chunk 2 completed 2026-11-13: both recall and check answered correctly, including correctly flagging a genuine answer-shape ambiguity in the check question.
* ⊘ **Block A quiz (A1–A5)**, `block-a-quiz-2026-11-13.md`, 11 questions. Skipped 2026-11-16 by choice; questions being folded into recalls instead. **Q1 answer key corrected 2026-11-19** (it wrongly put the away-from-fork 3′ end on the template strand rather than the new strand).

### Block B — Energy

* ☐ B1. Free energy, equilibrium, and why life runs far from equilibrium
* ◐ B2. Enzymes and catalysis (barriers, transition states, Michaelis–Menten)
* ☐ B3. ATP as currency; coupling reactions
* ☐ B4. Glycolysis and respiration: overview
* ◐ B5. Chemiosmosis in depth (proton gradients, ATP synthase)
* ☐ B6. Lane's argument: energy and the origin of complex cells \[research]

### Block C — Cells as physical objects

* ☑ C1. Scale and numbers (sizes, counts, timescales). Completed 2026-11-17: chunk 1 (sizes, counts, 1 molecule ≈ 1 nanomolar, surface-to-volume 3/r) — check answered after the question's hidden count→concentration step was made explicit; chunk 2 (timescales, degradation vs. dilution ODE) — check answered correctly unaided, in requested shape.
* ◐ C2. Diffusion and random walks. Chunk 1 done 2026-11-18/19: random walk, ⟨x²⟩ = 2Dt derivation, Stokes–Einstein, D values, t ≈ L²/(6D), axon vs. bacterium, motor crossover. Check passed with correction (squaring step). Chunk 2 next.
* ☐ C3. Crowding: what the inside of a cell is really like
* ◐ C4. Membranes and transport (bilayers, channels, pumps). Bilayer impermeability now correct (desolvation, Born energy); channels and pumps not yet covered.
* ☐ C5. Compartments and the cytoskeleton (prokaryote vs eukaryote)

### Theme 0 wrap-up

* ☐ Review quiz / flashcards

## Diagnostic results (2026-11-03 to 11-04)

| # | Topic                   | Result                                                                                                              |
| - | ----------------------- | ------------------------------------------------------------------------------------------------------------------- |
| 1 | Prokaryote vs eukaryote | Core fact right; missed why it matters                                                                              |
| 2 | Membranes               | Right instinct; "react" vs "interact" confused; check answer used wrong mechanism (charge repulsion)                |
| 3 | DNA structure           | Label right; missed copying mechanism                                                                               |
| 4 | DNA → protein           | Not recalled — **main gap**                                                                                         |
| 5 | Definition of a gene    | Right direction; conflated consensus facts with Ball's interpretation                                               |
| 6 | Proteins and catalysis  | Strongest answer; refined to transition-state binding                                                               |
| 7 | ATP and energy          | Currency ✓, storage ✗; energy source not known                                                                      |
| 8 | Scale and speed         | Size off by >10× (protein vs cell ≈ 4,000×); speed matched median enzyme only. **Revisited in C1 (2026-11-16/17).** |

**Patterns to watch:**

* Answers name the thing but skip the "why." (Recurred 2026-11-05, 11-07, 11-08 on cryptic sites. Improving: 2026-11-08 window-model answer gave the mechanism unaided, missing only the last link. **Recurred 2026-11-18:** Q1 recall omitted the polymerase 3′-only rule.)
* Standard biology sometimes attributed to Ball.
* Mechanistic, physical reasoning is a strength.
* Spatial questions posed only in words don't land. Draw first, then ask. Fog can say "draw it" at any time.
* When stuck on a "why," smaller checks (yes/no, one-step) work better than open "explain in a sentence" prompts. Confirmed 2026-11-06, 11-07, 11-08, 11-12, 11-17, 11-18. Current approach: ask for the first clause unaided, then fall back to one-step checks and a fill-in-the-blank.
* Direction words ("in the 3′ direction") get used loosely when two antiparallel molecules are involved. Ask which molecule. **Recurred 2026-11-18** (template vs. new strand) — though the quiz key itself had the same error, which may have reinforced it.
* A remembered fact ("small K_d = tight binding") doesn't automatically connect to a formula. Point to the defining property (K_d _is_ the half-occupancy concentration) before asking.
* New (2026-11-08): abbreviations and symbols introduced once (Pol II, ψ) don't carry over. Re-define at the point of use, especially inside a check question. **Recurred 2026-11-12:** RT used without definition. **Recurred 2026-11-17:** units (nm, µm, fL, pL, nM, mM) used unexpanded; Fog asked for all to be spelled out and glossaried. **Rule now: spell out every unit and symbol at its first appearance in each session**, including standard SI units; give a unit key at the top of a chunk when several appear.
* **Important (2026-11-09):** Fog often can't parse what an open check question wants (true with people too). Every check question now states the _shape_ of answer wanted. **Working (2026-11-10).** **Caution (2026-11-12):** a stated shape isn't enough if a key phrase is loose. **Recurred constructively (2026-11-13):** Fog flagged a genuinely ambiguous check question himself. **New failure mode (2026-11-17):** a check question that silently required an unstated conversion (10 molecules → 10 nanomolar) left Fog unable to see where the second quantity came from. **Rule: every quantity the answer uses must be stated in the question in the form it's compared in, or the conversion step must be named explicitly** ("first convert the count using the 1-molecule ≈ 1-nanomolar rule").
* New (2026-11-08): word precision — "replaced," "visible," "external" used where the mechanism needs "competitor appears," "unchallenged," "additional context." Mechanism right, wording loose. (Minor recurrences 2026-11-17: "dilution removes X from the cell"; 2026-11-18: "cell division sets the response time" where growth rate is the precise driver for concentration.)
* New (2026-11-10): when asked why X _can't_ be the cause, tends to say what X does do rather than what it fails to do. Minor; the logic is there.
* New (2026-11-11): a mechanism step gets stated without the property that makes it work ("forces a second check" without "independent"). Same family as "skips the why"; the fill-in fixed it at once.
* New (2026-11-12): "where is the information" answered one level too far upstream (nucleotide rather than amino acid sequence). Ask what is physically present at the step in question.
* **New (2026-11-18/19): states a scaling rule correctly but doesn't apply it.** "Time grows as the square of distance" stated ✓; next link gave only the distance ratio; then, after correctly choosing "much more than a million," the fill-in (written the next morning) reverted to "million-times-longer time" (linear). The rule and its application aren't yet joined. Re-test the application step (squaring the factor) directly, not just the rule's name.

## Open questions

(Questions Fog raises that we haven't resolved yet.)

* _(none yet)_

**Deferred threads (raised by Claude):**

* Ball's broad claim that alternative splicing shows the gene is a "resource," not a "program." Assessment so far: the narrow claim ("one gene, one protein" is false) is consensus; the broad claim doesn't follow from splicing alone, since the alternatives and the splicing factors are themselves encoded. Revisit in Theme 3 (cell states as network attractors).
* Ball on intrinsically disordered proteins as a challenge to "sequence → structure → function." Covered at the A5-appropriate level 2026-11-13; fuller treatment still due in Theme 2.
* Low-copy-number noise (lac repressor bursts, Choi et al. 2008) — flagged in C1; develop in Theme 3.
* Lane's surface-to-volume argument for why bacteria stay small — flagged in C1; test in B6.
* Why cytoplasm slows protein diffusion 4–13× relative to water — flagged in C2; C3 (crowding).
* Motor-vs-diffusion crossover L\* ≈ 6D/v (Claude's rough argument, not textbook) — revisit in C5.

## Session log

* **2026-11-03 to 11-04** — Theme 0 diagnostic, 8 questions plus checks. Set session format: short, irregular sessions, no numerical computation in checks. Started glossary (v1, 61 terms) and this log.
* **2026-11-05** — Recall (membranes): correct, right mechanism this time (loss of water shell). Added Born-energy formalization and the voltage part of the proton-motive force. Started A1: DNA structure, replication, accuracy and Hopfield proofreading; 5′/3′ directionality; leading vs lagging strands with an interactive fork diagram. Checks: "no lagging strand if strands were parallel" ✓; causal reason ✗ (attributed lag to waiting for exposed template, not to direction). A1 stays ◐. Session notes: `sessions/2026-11-05-A1-dna-copying.md`.
* **2026-11-06** — Recall (lagging strand): first answer named "growing away from the fork" but still gave waiting as the cause. Static fork diagram, then one-step checks ✓ ✓. Fill-in-the-blank ✓. A1 ☑.
* **2026-11-06 (later)** — Started A2. RNA polymerase, template vs coding strand, bubble not fork, no primer, error rate; promoters (sigma factor; general TFs + Pol II). Checks: idea right, word wrong (opens both, reads one); one-step ✓.
* **2026-11-07** — Recall (transcription direction) ✓ after one-step check. A2 chunk 3: regulatory TFs; occupancy θ = \[T]/(\[T] + K_d); Hill function; thermodynamic-model caveat \[research]; Ball on disordered factors (deferred to T2). Check (smaller K_d → lower half-occupancy concentration): stuck on open version; one-step checks ✓ ✓; fill-in ✓. A2 ☑. Glossary v3.
* **2026-11-07 (later)** — Recall (single site = dimmer, cooperativity sharpens): three one-step checks ✓ ✓ ✓; fill-in ✓.
* **2026-11-08** — A3 chunks 1–2: cap, poly-A, splicing mechanism, spliceosome, splice-site information content → cryptic sites → context; alternative splicing, ψ, window-of-opportunity model; Ball's "resource not program" and Claude's assessment (deferred to T3). Checks completed via one-step + fill-in. A3 ☑. Glossary v4.
* **2026-11-09** — Recall (cryptic sites) ✓ with correction. A4 chunk 1: triplet code, reading frames, tRNA + synthetases, editing, wobble, error-minimizing code \[research]. Fog flagged difficulty parsing questions → rule: state the answer shape. Check ✓ after one-step + fill-in.
* **2026-11-10** — Recall ✓ with missing link supplied (Chapeville 1962). A4 chunk 2: ribosome, initiation, elongation, energy accounting, two-stage selection f ≈ f₀², termination. Check (nonsense codon) ✓ unaided. A4 ☑. Glossary v5.
* **2026-11-11 to 11-12** — Recall (f₀²) ✓ after fill-in on independence. A5 chunk 1: backbone, side chains, hydrophobic effect, marginal stability, two-state folding, Anfinsen, Levinthal, funnel. Fog asked what RT meant. Check ✗ then ✓ via one-step + fill-in. Session notes: `sessions/2026-11-11-A5-protein-folding-chunk1.md`.
* **2026-11-13** — Recall ✓ unaided. A5 chunk 2: chaperones, misfolding, amyloid, prions, IDPs + Ball. Check: Fog flagged question ambiguity, both readings correct. A5 ☑ — **Block A complete.** Glossary v6. Session notes: `sessions/2026-11-13-A5-chunk2-chaperones-disorder.md`. Block A quiz delivered.
* **2026-11-16 to 11-17** — Fog chose to skip the Block A quiz and interleave Blocks B/C (C1 → C2 → B1 → B2 …). **C1 chunk 1:** log ruler of sizes; protein vs. cell ≈ 4,000× (diagnostic Q8 gap); counts table (E. coli vs. human cell); N = c·V·N_A and the 1 molecule ≈ 1 nanomolar rule; noise at low copy number \[→ T3]; S/V = 3/r and Lane's argument flagged \[research, → B6]. Fog asked for all units to be spelled out → unit key given, glossary v7 with a Units and prefixes section. Check (lac repressor occupancy): Fog couldn't see where the second concentration came from — question hid a count→concentration conversion (question flaw); one-step checks "10" ✓, "more" ✓; θ = 10/11 ≈ 0.91 shown; fill-in ✓. Choi et al. 2008 bursts \[research]. **C1 chunk 2:** log ruler of timescales; enzyme turnover, transcription/translation speeds, mRNA/protein lifetimes \[Schwanhäusser 2011, research]; dp/dt = k − (α_deg + α_dil)p, steady state and response time; stable bacterial proteins respond in \~one cell cycle (Alon ch. 2); C2 diffusion preview (t ∝ L²). Check (stable protein, production stopped): "dilution; one cell cycle" ✓ unaided, in requested shape; wording refinement (copies shared between daughters, not removed). **C1 ☑.** Glossary v8 (time units, turnover number, half-life, dilution, degradation rate, response time). Session notes: `sessions/2026-11-16-C1-scale-and-numbers.md`.
* **2026-11-18 to 11-19** — Recall 1 (C1 response time) ✓; refinement: growth rate, not division as an event, dilutes concentration. Recall 2 (Block A Q1): template vs. new strand confused and polymerase rule missing; fork diagram; one-step "3′" ✓, "away" ✓; full four-link fill-in ✓. Quiz Q1 key found to carry the same template-strand error → corrected. **C2 chunk 1:** Brownian motion and random walk; ⟨x²⟩ = 2Dt derivation (cross terms vanish), 3D 6Dt; interactive 500-walker simulation; Stokes–Einstein; D table (Milo & Phillips; Elowitz 1999); t ≈ L²/(6D): E. coli \~0.02 s, human cell \~3 s (corrects C1 preview's \~20 s), 1-meter axon \~200 years vs. motors \~10 days; crossover L\* ≈ 6D/v (Claude's rough argument). Check: "square" ✓; second link incomplete; one-step "much more than a million" ✓; fill-in ✗ ("million" for "trillion") → corrected, passed with correction. C2 ◐. Session notes: `sessions/2026-11-18-C2-chunk1-diffusion-random-walks.md`.

## Files

* `glossary.md` — running glossary (v8, 2026-11-17, \~215 entries plus a Units and prefixes section). C2 terms pending.
* `progress.md` — this file
* `block-a-quiz-2026-11-13.md` — Block A quiz (A1–A5), 11 questions, answers in `<details>`; skipped, questions folded into recalls. Q1 key corrected 2026-11-19.
* `sessions/2026-11-04-T0-diagnostic.md` — Theme 0 diagnostic, 2026-11-03/04 (rebuilt 11-10)
* `sessions/2026-11-05-A1-dna-copying.md` — A1 start, 2026-11-05
* `sessions/2026-11-06-A1-A2-lagging-strand-transcription.md` — A1 finish, A2 chunks 1–2 (rebuilt 11-10)
* `sessions/2026-11-07-A2-transcription-factors-occupancy.md` — A2 chunk 3, plus the later recall (rebuilt 11-10)
* `sessions/2026-11-08-A3-rna-processing-splicing.md` — A3 (rebuilt 11-10)
* `sessions/2026-11-09-A4-genetic-code-trna.md` — A4 chunk 1 (rebuilt 11-10)
* `sessions/2026-11-10-A4-translation-ribosome.md` — A4 chunk 2
* `sessions/2026-11-11-A5-protein-folding-chunk1.md` — A5 chunk 1, 2026-11-11/12
* `sessions/2026-11-13-A5-chunk2-chaperones-disorder.md` — A5 chunk 2, 2026-11-13
* `sessions/2026-11-16-C1-scale-and-numbers.md` — C1 (both chunks), 2026-11-16/17
* `sessions/2026-11-18-C2-chunk1-diffusion-random-walks.md` — recalls + C2 chunk 1, 2026-11-18/19
