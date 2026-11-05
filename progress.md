# How Life Works — Progress Log

Last updated: 2026-11-05

**How to use:** Start any session with "where were we?" Claude reads this log, gives one recall question from the last unit, and picks up at **Next up**. Sessions are short, one unit each; stopping mid-unit is fine.

---

## Where we are

- **Current theme:** Theme 0 — The standard picture
- **Next up:** Finish A1. Firm up *why* the lagging strand exists, then move to A2 (Transcription).
- **Last recall prompt to use:** "Why does one new strand have to be made in pieces?" (Target answer: polymerase only extends 3′ ends + the strands are antiparallel → one new strand necessarily points away from the fork.)

## Theme 0 units

Status: ☐ not started · ◐ in progress / partly covered · ☑ done

### Block A — Information: DNA → protein
- ◐ A1. DNA structure and copying (base pairing, semiconservative replication, proofreading). Facts covered 2026-11-05; causal "why" of leading/lagging strands not yet solid.
- ☐ A2. Transcription (RNA polymerase, promoters, transcription factors)
- ☐ A3. RNA processing (splicing, introns/exons, alternative splicing)
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
- Answers name the thing but skip the "why." (Recurred 2026-11-05: described what the lagging strand does, but not why.)
- Standard biology sometimes attributed to Ball.
- Mechanistic, physical reasoning is a strength.
- Spatial questions posed only in words don't land. Draw first, then ask. Fog can say "draw it" at any time.
- When stuck on a "why," smaller checks (yes/no, one-step) work better than open "explain in a sentence" prompts.

## Open questions

(Questions Fog raises that we haven't resolved yet.)

- *(none yet)*

## Session log

- **2026-11-03 to 11-04** — Theme 0 diagnostic, 8 questions plus checks. Set session format: short, irregular sessions, no numerical computation in checks. Started glossary (v1, 61 terms) and this log.
- **2026-11-05** — Recall (membranes): correct, right mechanism this time (loss of water shell). Added Born-energy formalization and the voltage part of the proton-motive force. Started A1: DNA structure, replication, accuracy and Hopfield proofreading; 5′/3′ directionality; leading vs lagging strands with an interactive fork diagram. Checks: "no lagging strand if strands were parallel" ✓; causal reason ✗ (attributed lag to waiting for exposed template, not to direction). A1 stays ◐. Session notes: `sessions/2026-11-05-A1-dna-copying.md`.

## Files

- `glossary.md` — running glossary (v1, 2026-11-04)
- `progress.md` — this file
- `sessions/2026-11-05-A1-dna-copying.md` — notes from the 2026-11-05 session
