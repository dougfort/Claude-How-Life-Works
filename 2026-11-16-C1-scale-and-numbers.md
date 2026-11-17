# Session notes — C1: Scale and numbers

**Dates:** 2026-11-16 to 11-17 · **Theme 0, Block C** · **Unit status after session:** C1 ☑

Block A quiz skipped by Fog's choice (stays saved; Block A questions to be folded into later recalls). Order chosen for Blocks B/C: **interleave**, C1 → C2 → B1 → B2, then alternate.

Main reference for numbers: Milo & Phillips, _Cell Biology by the Numbers_ (free at book.bionumbers.org). All values are order-of-magnitude **\[consensus]** unless tagged otherwise.

***

## Unit key

**Prefixes:** kilo (k) = 10³ · milli (m) = 10⁻³ · micro (µ, Greek mu) = 10⁻⁶ · nano (n) = 10⁻⁹ · pico (p) = 10⁻¹² · femto (f) = 10⁻¹⁵. Trap: "m" alone = meter; "m" before another unit = milli.

| Abbreviation          | Spelled out                                                           | Notes                                  |
| --------------------- | --------------------------------------------------------------------- | -------------------------------------- |
| nm                    | nanometer                                                             | 10⁻⁹ meter                             |
| µm                    | micrometer ("micron")                                                 | 10⁻⁶ meter = 1,000 nanometers          |
| µm³                   | cubic micrometer                                                      | = 1 femtoliter exactly                 |
| L                     | liter                                                                 |                                        |
| fL                    | femtoliter                                                            | 10⁻¹⁵ liter; one E. coli cell          |
| pL                    | picoliter                                                             | 10⁻¹² liter; human cell ≈ 3 picoliters |
| mol                   | mole                                                                  | ≈ 6 × 10²³ of anything                 |
| M                     | molar                                                                 | moles per liter                        |
| mM, µM, nM            | millimolar, micromolar, nanomolar                                     | 10⁻³, 10⁻⁶, 10⁻⁹ moles per liter       |
| N_A                   | Avogadro's number                                                     | ≈ 6 × 10²³ per mole                    |
| s, ms, µs, ns, ps, fs | second, millisecond, microsecond, nanosecond, picosecond, femtosecond |                                        |
| min, h                | minute, hour                                                          |                                        |

***

## Chunk 1 — How big, how many (2026-11-16)

### Sizes (log ruler, each tick ×10)

```
 1 nm        10 nm        100 nm       1 µm         10 µm        100 µm
  |------------|------------|------------|------------|------------|
  ^ glucose, ATP (~1 nm)
     ^ membrane thickness (~5 nm)
     ^ typical protein (~5 nm)
          ^ ribosome (~25 nm)
                       ^ virus (~100 nm)
                                    ^ E. coli (1 × 2 µm)
                                    ^ mitochondrion (~1 µm)
                                              ^ nucleus (~5 µm)
                                                   ^ human cell (10–20 µm)
```

Protein vs. human cell: 5 nanometers vs. 20 micrometers ≈ 4,000× (about 3.5 decades) — the gap the diagnostic underestimated. Tennis-ball picture: protein = tennis ball → cell ≈ 250 meters across, and packed (proteins fill 20–30% of cytoplasm volume; see C3, crowding).

### Counts

|                 | E. coli (\~1 femtoliter)               | Human cell (\~3 picoliters)                                       |
| --------------- | -------------------------------------- | ----------------------------------------------------------------- |
| Proteins, total | \~3 × 10⁶                              | \~10⁹–10¹⁰                                                        |
| Ribosomes       | \~10⁴–7×10⁴ (more when growing fast)   | \~10⁶–10⁷                                                         |
| Genome          | 4.6 million base pairs, \~4,300 genes  | 3.1 billion base pairs (×2 copies), \~20,000 protein-coding genes |
| ATP             | \~2 × 10⁶ molecules (a few millimolar) | \~10⁹                                                             |

Copy numbers per species range hugely: lac repressor \~10 per E. coli cell; EF-Tu \~10⁵.

### Conversion rule: 1 molecule per E. coli ≈ 1 nanomolar

c = N / (N_A · V). For V = 1 femtoliter = 10⁻¹⁵ liter:

N at 1 nanomolar = 10⁻⁹ mol/L × 10⁻¹⁵ L × 6 × 10²³ /mol ≈ 0.6 ≈ 1 molecule.

Consequences: (1) nanomolar K_d values (A2) correspond to single-digit copy numbers in bacteria, where "concentration" is a statistical average and single binding events matter → gene-expression **noise** (Theme 3). (2) In a human cell (\~3,000× the volume), 1 nanomolar ≈ 1,800 molecules — much less noisy.

### Surface-to-volume ratio

Sphere: S/V = 4πr² / (4/3 πr³) = 3/r. Ten times the radius → one-tenth the membrane per unit interior. Bacteria make ATP at their plasma membrane (B5); Lane argues this caps bacterial size and that mitochondria broke the cap by internalizing energy membranes **\[research / Lane's position, contested — tested in B6]**. The geometry is just 3/r.

### Check 1 (lac repressor occupancy)

_Question (as restated):_ About 10 lac repressor molecules in an E. coli cell; K_d for its site = 1 nanomolar (the concentration of half occupancy). Mostly occupied or mostly empty? Reason in one clause comparing two concentrations.

* Fog asked first for units to be spelled out (done; added to glossary).
* Fog then: "I don't understand the question. I don't know where two concentrations are coming from." **Question flaw, not a gap:** one concentration was hidden as a count; the question silently required converting it.
* One-step: 10 molecules ≈ ? nanomolar → **"10"** ✓
* One-step: 10 nanomolar vs. K_d 1 nanomolar → occupied more or less than half the time? → **"more"** ✓
* Math shown: θ = \[T]/(\[T] + K_d) = 10/11 ≈ 0.91.
* Fill-in: "The repressor's concentration (about ten nanomolar) is more than the K_d (1 nanomolar), so the site is mostly occupied." ✓

Footnote: the real lac repressor binds far more tightly than 1 nanomolar **\[consensus]**; with \~10 copies, single unbinding events let through bursts of expression (Choi et al. 2008) **\[research]** — low-copy noise, back in Theme 3.

***

## Chunk 2 — How fast (2026-11-17)

### Timescales (log ruler, each tick ×1,000)

```
 1 fs      1 ps      1 ns      1 µs      1 ms      1 s       ~17 min   ~12 days
 10⁻¹⁵ s   10⁻¹² s   10⁻⁹ s    10⁻⁶ s    10⁻³ s    1 s       10³ s     10⁶ s
  |---------|---------|---------|---------|---------|---------|---------|
     ^ bond vibration (~10 fs)
                         ^ side chain flips (~ns)
                                   ^—————————————————^ protein folding (µs to s)
                                                  ^ median enzyme turnover (~0.1 s per reaction)
                                                  ^ protein crosses E. coli by diffusion (~0.05 s)
                                                        ^ ribosome adds one amino acid (~0.05–0.2 s)
                                                          ^ one 300-amino-acid protein (~20 s E. coli, ~1 min human)
                                                            ^ E. coli mRNA half-life (few min)
                                                              ^ E. coli divides (~20 min at best)
                                                                     ^ human mRNA, median (~hours)
                                                                        ^ human cell divides (~24 h)
                                                                        ^ human protein, median (~2 days)
```

* **Enzyme turnover:** median \~10 reactions per second per enzyme; fastest \~10⁶–10⁷ per second (e.g. carbonic anhydrase) (Bar-Even et al. 2011) **\[consensus]**.
* **Transcription:** E. coli RNA polymerase \~40–80 nucleotides per second; human RNA polymerase II \~1–4 kilobases (thousands of bases) per minute. Dystrophin, the longest human gene (\~2.2 million base pairs), takes \~16 hours per transcript **\[consensus]**.
* **Translation:** \~10–20 amino acids per second (bacteria), \~5 per second (human) (from A4) **\[consensus]**.
* **Lifetimes:** E. coli mRNAs mostly a few minutes **\[consensus]**. Mouse cells: median \~9 h for mRNA, \~46 h for protein (Schwanhäusser et al. 2011) **\[research; values method-dependent, later studies often shorter for mRNA]**.
* **Takeaway:** bacteria live in minutes; human cells in hours to days.

### Formalization: removal by degradation vs. dilution

p = protein concentration; k = production rate; α_deg = degradation rate (active destruction); α_dil = dilution rate from growth = ln 2 / T_div (T_div = doubling time; ln 2 ≈ 0.69). α is Greek alpha.

dp/dt = k − (α_deg + α_dil) · p

* Steady state: p\* = k / (α_deg + α_dil)
* Response time (halfway to new steady state): t½ = ln 2 / (α_deg + α_dil)

**\[consensus]** In fast-growing bacteria most proteins are stable (α_deg ≈ 0), so dilution does the removing and **a stable protein's response time ≈ one cell cycle**, however fast production switches. (Uri Alon, _An Introduction to Systems Biology_, ch. 2.) Fast responses need actively degraded proteins. Human dividing cells: degradation and dilution comparable; non-dividing cells (e.g. neurons): α_dil = 0, degradation only.

**C2 preview:** diffusion time ∝ distance². Protein across E. coli (\~1 micrometer): \~0.05 s. Across a 20-micrometer human cell: 20× the distance → \~400× the time ≈ 20 s.

### Check 2 (stable protein, production stopped)

_Question:_ Bacterium stops making X (k → 0); X is never degraded. (a) What removes X? (b) How long until X's concentration halves, in a unit of the cell's life cycle?

* Fog: "Dilution removes X from the cell. It takes one cell cycle for the concentration to fall to half." **✓ both parts, unaided, in requested shape.**
* Refinement (wording, not mechanism): dilution doesn't destroy molecules — at division existing copies are shared between daughters, so each cell has half as many.

***

## Terms introduced

Units and prefixes (full set, see glossary section) · Avogadro's number · copy number · 1 molecule ≈ 1 nanomolar rule · surface-to-volume ratio · lac repressor · turnover number · half-life · dilution (growth dilution) · degradation rate · response time

***

## Next recall prompts

**Recall 1 (C1).** A bacterium switches on production of a stable protein (never degraded). Why does its concentration take about one cell cycle to approach its new level, no matter how fast production switches on? _Answer shape:_ a chain of three links: "no degradation → only \_\_\_ removes it → so \_\_\_ sets the response time."

\<details> \<summary>Answer\</summary>

No degradation → only dilution by growth removes it → so the growth (doubling) rate sets the response time: t½ = ln 2 / α_dil = T_div. Removal rate determines response time because the system relaxes exponentially at rate (α_deg + α_dil) toward p\* = k/(α_deg + α_dil).

\</details>

**Recall 2 (Block A quiz, Q1 — re-testing the diagnostic's main gap).** Walk the causal chain from "DNA's two strands are antiparallel" to "one new strand is made in Okazaki fragments." _Answer shape:_ four short links, A → B → C → D.

\<details> \<summary>Answer\</summary>

Antiparallel strands → DNA polymerase can only build 5′→3′ (adds only to a 3′ end) → on one template, the new strand's growing 3′ end points away from the fork → it can't follow the fork, so it's made in short backward pieces (Okazaki fragments), later joined by ligase.

\</details>

**Next unit:** C2 — Diffusion and random walks.
