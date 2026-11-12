# How Life Works — Progress Log

Last updated: 2026-11-12

**How to use:** Start any session with "where were we?" Claude reads this log, gives one recall question from the last unit, and picks up at **Next up**. Sessions are short, one unit each; stopping mid-unit is fine. **End every session with a session-notes markdown file** (`sessions/YYYY-MM-DD-<unit>-<topic>.md`): content taught, diagrams as ASCII, checks with Fog's answers and feedback, terms introduced, next recall prompt with the answer in a collapsible `<details>` block. Quizzes are also delivered as saveable markdown, answers in `<details>`.

---

## Where we are

- **Current theme:** Theme 0 — The standard picture
- **Next up:** A5 chunk 2: chaperones, misfolding and aggregation, intrinsically disordered proteins and Ball's reading of them. Then the Block A quiz.
- **Last recall prompt to use:** "What mainly drives a protein to fold, and where does most of the free-energy gain come from? Answer shape: name the effect, then say in one clause whose entropy rises and why." (Target answer: the hydrophobic effect; mostly water's entropy rises, because oily side chains force water into ordered cages and burying them releases that water.)

## Theme 0 units

Status: ☐ not started · ◐ in progress / partly covered · ☑ done

### Block A — Information: DNA → protein
- ☑ A1. DNA structure and copying (base pairing, semiconservative replication, proofreading). Completed 2026-11-06: full causal chain for leading/lagging strands stated correctly.
- ☑ A2. Transcription (RNA polymerase, promoters, transcription factors). Completed 2026-11-07: transcription direction stated precisely; K_d/occupancy chain stated correctly after step-by-step checks.
- ☑ A3. RNA processing (splicing, introns/exons, alternative splicing). Completed 2026-11-08: information-shortfall chain and window-model chain both stated correctly after step-by-step checks.
- ☑ A4. The genetic code and translation (codons, tRNA, ribosome). Chunk 1 (code, reading frames, tRNA + synthetases, editing) 2026-11-09; chunk 2 (ribosome) completed 2026-11-10: nonsense-codon chain stated correctly unaided.
- ◐ A5. Protein folding and shape (side chains, Anfinsen, chaperones). Chunk 1 (chain and side chains, hydrophobic effect, two-state stability, Anfinsen, Levinthal and the funnel) 2026-11-11/12. Chunk 2 (chaperones, misfolding, disordered proteins + Ball) next.
- ☐ Block A quiz (A1–A5) after A5 — agreed 2026-11-09. Focus on the full DNA → protein chain (diagnostic main gap).

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
- When stuck on a "why," smaller checks (yes/no, one-step) work better than open "explain in a sentence" prompts. Confirmed 2026-11-06, 11-07, 11-08, 11-12. Current approach: ask for the first clause unaided, then fall back to one-step checks and a fill-in-the-blank.
- Direction words ("in the 3′ direction") get used loosely when two antiparallel molecules are involved. Ask which molecule.
- A remembered fact ("small K_d = tight binding") doesn't automatically connect to a formula. Point to the defining property (K_d *is* the half-occupancy concentration) before asking.
- New (2026-11-08): abbreviations and symbols introduced once (Pol II, ψ) don't carry over. Re-define at the point of use, especially inside a check question. **Recurred 2026-11-12:** RT used without definition; Fog asked. Define every symbol where it first appears, even ones standard in physics.
- **Important (2026-11-09):** Fog often can't parse what an open check question wants (true with people too). Some logged "skips the why" was question ambiguity, not a gap. Every check question now states the *shape* of answer wanted ("name the cause in one clause," "rule out the other options," "give the chain A → B → C"). **Working (2026-11-10):** recall and the nonsense-codon check both answered in the requested shape, unaided. **Caution (2026-11-12):** a stated shape isn't enough if a key phrase is loose. "A thing in the cell" admitted water; should have said "something a cell has that the test tube lacked."
- New (2026-11-08): word precision — "replaced," "visible," "external" used where the mechanism needs "competitor appears," "unchallenged," "additional context." Mechanism right, wording loose.
- New (2026-11-10): when asked why X *can't* be the cause, tends to say what X does do rather than what it fails to do. Minor; the logic is there.
- New (2026-11-11): a mechanism step gets stated without the property that makes it work ("forces a second check" without "independent"). Same family as "skips the why"; the fill-in fixed it at once.
- New (2026-11-12): "where is the information" answered one level too far upstream (nucleotide rather than amino acid sequence). Ask what is physically present at the step in question.

## Open questions

(Questions Fog raises that we haven't resolved yet.)

- *(none yet)*

**Deferred threads (raised by Claude):**
- Ball's broad claim that alternative splicing shows the gene is a "resource," not a "program." Assessment so far: the narrow claim ("one gene, one protein" is false) is consensus; the broad claim doesn't follow from splicing alone, since the alternatives and the splicing factors are themselves encoded. Revisit in Theme 3 (cell states as network attractors).
- Ball on intrinsically disordered proteins as a challenge to "sequence → structure → function." Flagged 2026-11-11; cover in A5 chunk 2, fuller treatment in Theme 2.

## Session log

- **2026-11-03 to 11-04** — Theme 0 diagnostic, 8 questions plus checks. Set session format: short, irregular sessions, no numerical computation in checks. Started glossary (v1, 61 terms) and this log.
- **2026-11-05** — Recall (membranes): correct, right mechanism this time (loss of water shell). Added Born-energy formalization and the voltage part of the proton-motive force. Started A1: DNA structure, replication, accuracy and Hopfield proofreading; 5′/3′ directionality; leading vs lagging strands with an interactive fork diagram. Checks: "no lagging strand if strands were parallel" ✓; causal reason ✗ (attributed lag to waiting for exposed template, not to direction). A1 stays ◐. Session notes: `sessions/2026-11-05-A1-dna-copying.md`.
- **2026-11-06** — Recall (lagging strand): first answer named "growing away from the fork" but still gave waiting as the cause. Static fork diagram, then one-step checks: 3′ end of new bottom piece is away from the fork ✓; it can only grow away from the fork ✓. Fill-in-the-blank: 3′ end only + antiparallel → growing end points away → can't extend into new template → segmented ✓. A1 ☑.
- **2026-11-06 (later)** — Started A2. Covered: RNA polymerase reads one strand 5′→3′, template vs coding strand, small bubble not a fork, no primer, higher error rate and why that's tolerable; promoters set start and direction (sigma factor in bacteria; general transcription factors + Pol II in eukaryotes). Bubble diagram. Checks: "no lagging problem because it only opens one strand" — idea right, word wrong (opens both, reads one); one-step: RNA templated on the wrong strand would have 3′ end facing away ✓.
- **2026-11-07** — Recall (transcription direction): "only one strand is read" ✓ (word fixed); "in the 3′ direction" too vague — one-step check: RNA's growing 3′ end faces travel ✓. A2 chunk 3: regulatory transcription factors (activators, repressors, enhancers); occupancy θ = [T]/([T] + K_d) as a two-state partition function; same form as Michaelis–Menten; single site = soft dimmer; cooperativity → Hill function; thermodynamic-model caveat [research]; Ball on disordered, promiscuous factors (deferred to T2). Check (smaller K_d → lower half-occupancy concentration): stuck on open version; after pointing to K_d as the half-occupancy concentration, one-step checks ✓ ✓; added K_d = k_off/k_on; fill-in-the-blank ✓. A2 ☑. Glossary v3 (+16 terms, several entries updated).
- **2026-11-07 (later)** — Recall (single site = dimmer, cooperativity sharpens): asked for smaller steps; three one-step checks ✓ ✓ ✓; fill-in-the-blank ✓.
- **2026-11-08** — A3 chunk 1: cap, poly-A tail, splicing during transcription; splice signals (GU, AG, branch-point A); two-step lariat mechanism (diagram); spliceosome with RNA catalytic core; self-splicing introns as likely ancestor; information content of splice sites (~8–9 bits vs ~15 needed) → cryptic sites → enhancers/silencers, exon definition, timing. Check: unaided answer gave the conclusion ("can contain cryptic sites"), missed "many" and "can't tell apart"; one-step (doubling length doubles decoys) ✓; fill-in ✓, but "external" → corrected to "additional/context." A3 chunk 2: alternative splicing (cassette-exon diagram; patterns; Bcl-x, Dscam 38,016); functional-isoform dispute [research]; SR vs hnRNP competition; ψ = k_inc/(k_inc + k_skip); window-of-opportunity model P = 1 − e^(−kd/v) [research on generality]; Ball's "resource not program" reading and Claude's assessment (deferred to T3). Fog asked what "Pol II" meant (re-defined). Check: unaided answer got the window mechanism; corrected "replaced"/"visible"; ψ needed re-defining; then one-step completion ✓. A3 ☑. Glossary v4 (+20 terms, several entries updated).
- **2026-11-09** — Recall (cryptic sites): "too few bits" and "multiple matches" unaided ✓; completion gave "not sufficient / other means" — corrected to "can't tell them apart" and named context (enhancers/silencers, exon definition, timing). A4 chunk 1: why triplets (4³ = 64; log₂20 ≈ 4.3 bits vs 6 bits → redundancy); 61 sense + 3 stop codons, AUG start; reading frames and frameshifts (Crick–Brenner 1961); tRNA adapter + synthetases (diagram); synthetase editing ("double sieve," Ile/Val) as kinetic proofreading; wobble; error-minimizing code arrangement (Freeland & Hurst 1998) and dispute over why [research]. Check (what fixes codon meaning): synthetase ✓, but answered what it does rather than why it decides. Fog flagged difficulty parsing what questions want → new rule: state the answer shape. One-step (pairing doesn't check the amino acid) ✓; fill-in ✓. Block A quiz scheduled after A5.
- **2026-11-10** — Recall (what fixes codon meaning): synthetase ✓; second clause said what pairing checks rather than what it never checks — supplied the missing link with Chapeville 1962 (Cys→Ala on tRNA^Cys, alanine inserted). A4 chunk 2: ribosome subunits and A/P/E sites (diagram); initiation (cap scanning to first AUG in eukaryotes, Shine–Dalgarno in bacteria; sets the frame); elongation cycle (delivery, peptide bond by rRNA, translocation); N→C synthesis; energy accounting (ATP paid by the synthetase, GTP for movement and accuracy; contrast with DNA copying, where the tip carries no energy); two-stage selection separated by irreversible GTP hydrolysis, f ≈ f₀² [consensus], speed–accuracy tuning [research]; termination by release factors. Check (UGG→UGA mid-gene): release factor in A site → truncated protein released ✓ unaided; added nonsense-mediated decay. A4 ☑. Glossary v5 (+25 terms, several entries updated).
- **2026-11-11 to 11-12** — Recall (f₀²): GTP hydrolysis ✓; "forces a second check" missed independence → explained (reversible step would re-equilibrate and add nothing); fill-in (return / independent / multiply) ✓. A5 chunk 1: backbone, side chains (four groups), planar peptide bond, φ/ψ; hydrophobic effect driven mostly by water's entropy (link to C4); marginal stability (20–60 kJ/mol); two-state folding K = e^(−ΔG/RT), same form as A2 occupancy; Anfinsen 1961 ribonuclease and the scrambled-disulfide control; metastable exceptions (serpins, prions); AlphaFold/2024 Nobel rests on Anfinsen; Levinthal's paradox; folding funnel (diagram), minimal frustration, Zwanzig 1992 biased search; Ball on disordered proteins flagged for chunk 2. Fog asked what RT meant (defined: R·T, molar thermal energy, ≈ 2.6 kJ/mol at 310 K). Check (what Anfinsen rules out / where the information is): first answer "water cages / nucleotide sequence" ✗ (question wording let "water" in; nucleotide one step upstream); one-step checks ✓ ✓; fill-in (machinery / amino acid) ✓. A5 ◐. Session notes: `sessions/2026-11-11-A5-protein-folding-chunk1.md`.

## Files

- `glossary.md` — running glossary (v5, 2026-11-10; A5 terms to be added when A5 is complete)
- `progress.md` — this file
- `sessions/2026-11-04-T0-diagnostic.md` — Theme 0 diagnostic, 2026-11-03/04 (rebuilt 11-10)
- `sessions/2026-11-05-A1-dna-copying.md` — A1 start, 2026-11-05
- `sessions/2026-11-06-A1-A2-lagging-strand-transcription.md` — A1 finish, A2 chunks 1–2 (rebuilt 11-10)
- `sessions/2026-11-07-A2-transcription-factors-occupancy.md` — A2 chunk 3, plus the later recall (rebuilt 11-10)
- `sessions/2026-11-08-A3-rna-processing-splicing.md` — A3 (rebuilt 11-10)
- `sessions/2026-11-09-A4-genetic-code-trna.md` — A4 chunk 1 (rebuilt 11-10)
- `sessions/2026-11-10-A4-translation-ribosome.md` — A4 chunk 2
- `sessions/2026-11-11-A5-protein-folding-chunk1.md` — A5 chunk 1, 2026-11-11/12
