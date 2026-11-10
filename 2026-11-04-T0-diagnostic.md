# Session 2026-11-03/04 — Theme 0 diagnostic

**Theme 0** · Eight-question diagnostic to separate real understanding from familiar vocabulary · Outcome: Theme 0 split into Blocks A (information), B (energy), C (cells as physical objects)

Tags: **[consensus]** textbook view · **[research]** active, unsettled · **[Ball]** Ball's interpretive position

*Rebuilt from the chat on 2026-11-10.*

---

## Q1. Bacterial cell vs one of my cells

**My answer.** Mine has a nucleus; a bacterium does not.

**Feedback.** Correct but incomplete: it skipped *why it matters*.

**The textbook picture** [consensus]
- **Two kinds of cell.** Prokaryotes (bacteria, archaea) have no nucleus. Eukaryotes (animals, plants, fungi, protists) have a nucleus and other membrane-bound compartments (mitochondria, endoplasmic reticulum…).
- **Size.** Eukaryotic cells are ~10–30 µm vs ~1–2 µm for bacteria, about 1,000× the volume.
- **Transport.** Eukaryotes have a cytoskeleton that moves material actively; bacteria mostly rely on diffusion.

**Why the nucleus matters: decoupling.** In a bacterium, ribosomes start translating an RNA while it's still being made. In a eukaryote, the nuclear membrane separates the two steps. RNA is processed in the nucleus before export, which adds a layer of control over what a gene produces.

**Why mitochondria matter: energy.** Mitochondria descend from engulfed bacteria [consensus]. Nick Lane argues they are *why* eukaryotes could become large and complex, by multiplying the energy available per gene [research].

**Check.** Name one thing a eukaryote can do with an RNA that a bacterium mostly can't.
- *My answer:* "more control over what the RNA produces."
- *Feedback:* a restatement, not a named thing. Three examples:
  - **Splicing**, including alternative splicing (one gene → several proteins). This is the one to remember.
  - Holding the RNA in the nucleus, or timing its export.
  - **Editing** individual letters.

---

## Q2. What a membrane is made of, and why it doesn't dissolve

**My answer.** A substance of which one side does not react with water.

**Feedback.** Right instinct, wrong in two specifics:
1. **"React" is the wrong word.** Nothing reacts. The question is whether a molecule *interacts favorably* with water: **hydrophilic** (polar or charged) vs **hydrophobic** (nonpolar).
2. **Not "one side" of the membrane.** Each *molecule* (a **phospholipid**: charged head, two hydrocarbon tails) has a water-loving end and a water-avoiding end. They form a **bilayer**:

```
 water
 O O O O O O O O     ← hydrophilic heads face water
 | | | | | | | |
 | | | | | | | |     ← hydrophobic tails hidden inside
 | | | | | | | |
 O O O O O O O O     ← hydrophilic heads face water
 water (inside the cell)
```

**Why it holds together: the hydrophobic effect.** This is mostly **entropy**, not attraction. Water next to a nonpolar tail forms ordered cages. Clumping the tails frees that water and raises total entropy. In ΔG = ΔH − TΔS, the −TΔS term does most of the work. The bilayer **self-assembles**: it is structure not specified by genes, one of Ball's recurring points.

Also standard [consensus]:
- About half a membrane's mass is **proteins**: channels, pumps, receptors.
- The bilayer is a **2D fluid**; lipids diffuse sideways freely.

**Check.** Why is a pure bilayer nearly impermeable to small ions like Na⁺ and K⁺?
- *My answer:* the charged heads repel charged particles.
- *Feedback:* **wrong mechanism.**
  - Charge repulsion would repel one sign and attract the other, but the bilayer blocks Na⁺ and Cl⁻ about equally. Many heads are also net neutral.
  - **The real barrier is the oily core.** A dissolved ion carries a stabilizing shell of oriented water. Nothing in the core can replace it.
  - The cost is the **Born energy**:

$$\Delta G \approx \frac{q^2}{8\pi\varepsilon_0 a}\left(\frac{1}{\varepsilon_{\text{core}}} - \frac{1}{\varepsilon_{\text{water}}}\right),\quad \varepsilon_{\text{core}}\approx 2,\ \varepsilon_{\text{water}}\approx 80$$

  - That is tens of kT or more for a small ion, so the Boltzmann factor is negligible.
  - This is why cells need **channel and pump proteins**.
  - *(Recalled correctly on 2026-11-05.)*

---

## Q3. What DNA physically is, and why its structure suggests copying

**My answer.** A polymer in the double-helix shape.

**Feedback.** Correct label; missed the second half (the copying mechanism). This was the first appearance of the pattern **"name the thing, skip the why."**

**The fuller picture** [consensus]
- **Monomers.** Nucleotides: a sugar, a phosphate, one base (A, T, G, C). Sugar–phosphate backbone, bases sticking out.
- **Pairing.** Two **antiparallel** strands, paired **A–T** and **G–C** by hydrogen bonds:

```
5'  A T G C C T A  3'
    | | | | | | |
3'  T A C G G A T  5'
```

- **Copying.** Each strand determines the other. Unzip, build a new partner for each, and you get two helices, each half old and half new: **semiconservative replication** (Meselson–Stahl 1958).
- **Information.** 2 bits per base pair. Human genome ≈ 3.1 × 10⁹ bp ≈ 6 × 10⁹ bits ≈ 750 MB.
- **Accuracy.** Pairing alone isn't accurate enough. Real copying reaches ~1 error per 10⁹ bp only through energy-spending proofreading (**Hopfield's kinetic proofreading**, 1974). A small example of Ball's theme that precision comes from active processes, not the molecule alone.

**Session rule set here:** no numerical computation in checks; math is shown, not assigned. For the record, pairing alone would need ~21 kT to reach 10⁻⁹. The real difference is only a few kT, giving 10⁻² to 10⁻⁴ without proofreading.

---

## Q4. DNA → protein

**My answer.** Couldn't recall it. **This was the diagnostic's main gap.**

**The pathway** [consensus]

```
NUCLEUS                                          CYTOPLASM
DNA ──transcription──► pre-mRNA ──processing──► mRNA ──export──► ribosome ──translation──► chain ──folding──► protein
     (RNA polymerase)        (splicing, cap, tail)                     (tRNAs bring amino acids)       (chaperones help)
```

1. **Transcription** (nucleus). RNA polymerase binds a **promoter**, helped by **transcription factors**, and copies one DNA strand into RNA (U in place of T).
2. **Processing** (nucleus). Pre-mRNA has **exons** (kept) and **introns** (cut out by **splicing**). It gets a cap and a tail, becomes **mRNA**, and is exported.
3. **Translation** (cytoplasm). A **ribosome** reads three letters at a time (**codons**). 4³ = 64 codons cover 20 amino acids plus stop, so the code is redundant. **tRNAs** bring the amino acids. Starts at AUG, ends at a stop codon.
4. **Folding.** The chain folds, sometimes with **chaperones**, and may be modified and sent to its location.

**Consensus vs Ball: the central dogma.**
- **Crick's 1958 claim** was narrow: sequence information never flows back from protein to nucleic acid. It still holds [consensus].
- **What Ball and Noble attack** is the loose reading "DNA is the program, everything else executes" [Ball].
- **The critics' reply:** no working biologist holds that loose reading.

**Math note.** The genetic code is arranged so that one-letter errors often swap in a similar amino acid. It can be treated as an error-minimizing code (Theme 5).

**Check.** A mutation changes one letter inside an intron. Does the protein change?
- *My answer:* no, since the intron is cut out; it could change the protein if it garbles transcription.
- *Feedback:* the first half is right. The second points at the wrong step. Polymerase copies introns faithfully. **Splicing** is the vulnerable step: a mutation in a splice signal can leave the intron in or skip an exon (a known cause of disease). Some introns also hold regulatory sequences that change the *amount* of protein.

---

## Q5. "A gene is a sequence that codes for a protein": accurate?

**My answer.** This is where Ball comes in; the phrase sounds like a computer program, and there could be a lot more going on than simple encoding.

**Feedback.** Right direction, but two separate claims were merged.

**(a) Is the definition accurate? No, and you don't need Ball to see it** [consensus]:
- **One gene, many proteins** (alternative splicing).
- **Genes that never make protein** (tRNA, ribosomal RNA, microRNAs, long non-coding RNAs).
- **The coding part is a sliver.** Coding sequence is ~1–2% of the human genome; regulatory DNA decides when genes are used.
- **No agreed definition.** The molecular sense (transcribed unit) and the evolutionary sense (inherited, selected unit; Dawkins' usage) don't line up.

**(b) Ball's interpretive claim** [Ball]: causation runs substantially the other way. The cell, in context, decides what a gene does; genes are a resource, not a program.
- *Standard pushback:* biologists already know everything in (a), so Ball is fighting a metaphor, not a belief. The real dispute is whether the metaphor still distorts reasoning.
- *Habit to build:* ask which kind of claim you're making.

**Check.** Which failure do tRNA and ribosomal RNA illustrate, and why are they especially awkward?
- *My answer:* genes that never make protein; awkward because they help make proteins.
- *Feedback:* **correct.** Sharper version: the machinery that reads the "recipe" is built from non-recipe genes. The ribosome's peptide-bond step is catalyzed by its **RNA**, making it a **ribozyme** [consensus]. That is key evidence for the **RNA world** hypothesis [research].

---

## Q6. How a 1D chain does something specific

**My answer.** It folds into a 3D shape that can catalyze a reaction, probably by binding a reagent and reducing the energy needed.

**Feedback.** The strongest answer of the diagnostic.

**Why it folds the way it does.** Side chains are oily, charged or polar. Oily ones bury themselves in the core (the hydrophobic effect again). **Anfinsen's principle**, that sequence determines fold, holds for many proteins [consensus], with caveats: chaperones, and **intrinsically disordered proteins** (Theme 2).

**Where specificity comes from.** The fold creates an **active site** whose shape and chemistry fit a **substrate** (the standard term; "reagent" is lab vocabulary).
- Lock and key (Fischer) → induced fit (Koshland) [consensus].
- Ball argues recognition is looser and more promiscuous still [Ball, Theme 2].

**Two corrections**
1. An enzyme lowers the **activation barrier**, not the reaction's overall ΔG:

```
energy
  │       ╱‾‾╲         ← uncatalyzed transition state
  │      ╱ ╱‾╲ ╲       ← catalyzed: lower peak
  │ S ──╯ ╱   ╲ ╲
  │      ╱     ╲ ╰── P
  │                    ΔG (S→P) unchanged
  └──────────────────── reaction progress
```

2. **What it binds:** enzymes bind the **transition state** more tightly than the substrate (Pauling). That is what lowers the peak.

**Math** (read, not compute):
- **Eyring:** $k \propto e^{-\Delta G^\ddagger / k_B T}$. Exponential, so modest barrier cuts give speedups of 10⁶ to 10¹⁷.
- **Michaelis–Menten:** $v = V_{\max}[S]/(K_M + [S])$. Rises, then saturates as every enzyme is busy.

**Check.** Does an enzyme for A → B also speed B → A?
- *My answer:* yes, the barrier is lowered.
- *Feedback:* **correct.** It speeds both by the *same factor*, so enzymes change rate, not the final equilibrium. Pushing a reaction uphill needs payment, which is ATP.

---

## Q7. What ATP is for, and where its energy comes from

**My answer.** Energy transfer and storage; didn't know the source.

**Feedback.** "Transfer" ✓, "storage" ✗, and the source is the important part.

**What ATP is**
- **Currency, not savings.** Storage is fat and glycogen. A human recycles about their body weight in ATP daily.
- **Energy per molecule.** ATP → ADP + Pi releases ~20 kT under cellular conditions.
- **How it pays.** Enzymes **couple** unfavorable reactions to ATP splitting.
- **Where the energy really is.** Not in a magic bond: the cell holds the ATP/ADP ratio far from equilibrium, like a charged battery.

**Where the energy comes from**
1. **Glycolysis** (cytoplasm): a little ATP directly.
2. **Electron transport chain** (mitochondria): electrons from food pass to oxygen.
3. That chain doesn't make ATP. It **pumps protons** across the inner membrane.
4. Protons flow back through **ATP synthase**, a rotary motor whose spinning makes ATP.

```
        intermembrane space:  H⁺ H⁺ H⁺ H⁺ H⁺ H⁺   (high H⁺)
  ════════[pump]═══[pump]═══[pump]══════[ATP synthase]════  inner membrane
            ↑ e⁻ from food drive pumping     ↓ H⁺ flows back, rotor spins
        matrix:              (low H⁺)        ADP + Pi → ATP
```

- **Chemiosmosis:** Mitchell 1961, ridiculed, Nobel 1978 [consensus].
- **Callback to Q2:** this works only because the bilayer is impermeable to ions.
- **Scale:** ~150–200 mV across ~5 nm, a field on the order of 3 × 10⁷ V/m.
- **Lane's origin claim:** all life uses proton gradients, which he reads as a clue to an origin at alkaline hydrothermal vents [research, contested].

**Check.** Poke holes so protons leak back, bypassing ATP synthase. What happens?
- *My answer:* the motor doesn't spin, no ATP; the food energy is lost as heat.
- *Feedback:* **correct.** **Brown fat** does this on purpose (thermogenin). The 1930s diet drug DNP did it chemically and killed people by overheating.

---

## Q8. Scale and speed

**My answer.** A protein is ~100× smaller than a cell; molecular events happen at tens per second.

**Feedback.** Size off by more than 10×. The speed matches one process, not a general rate.

| | Typical size |
|---|---|
| Protein | ~5 nm |
| Bacterium | ~1–2 µm (~300× a protein) |
| Human cell | ~20 µm (~4,000× a protein; ~10¹⁰ in volume) |

- A human cell holds billions of proteins.
- Macromolecules fill 20–30% of the cytoplasm, closer to a crowded subway car than a dilute soup.

| Event | Timescale |
|---|---|
| Bond vibration | ~10⁻¹⁴ s |
| Small molecule diffuses across a bacterium | ~1 ms |
| Fast enzyme (catalase) | ~10⁷ reactions/s |
| Median enzyme | ~10 reactions/s |
| Ribosome adds an amino acid | ~10–20 per s |
| Gene expression changes | minutes |
| Cell division | 20 min (E. coli) to ~1 day (human) |

**Diffusion:** $t \sim L^2/(2dD)$. Fast over nanometers, hopeless over centimeters. That is one reason cells are small and large cells need active transport. Constant thermal buffeting is the "noise" of Theme 3 and the physical basis of Ball's claim that cells aren't clockwork.

---

## Diagnostic summary

| # | Topic | Result |
|---|---|---|
| 1 | Prokaryote vs eukaryote | Core fact right; missed why it matters |
| 2 | Membranes | Right instinct; "react" vs "interact"; check used wrong mechanism |
| 3 | DNA structure | Label right; missed copying mechanism |
| 4 | DNA → protein | Not recalled — **main gap** |
| 5 | Definition of a gene | Right direction; mixed consensus with Ball |
| 6 | Proteins and catalysis | Strongest answer |
| 7 | ATP and energy | Currency ✓, storage ✗; source unknown |
| 8 | Scale and speed | Size off by >10×; speed = median enzyme only |

**Strengths.** Physical, mechanistic reasoning.

**Gaps**
- The DNA → protein backbone needs building, not reviewing.
- Vocabulary is at label level.
- Answers name the thing and skip the why.
- Standard biology gets attributed to Ball.

**Decisions made**
- Short sessions at irregular intervals.
- No assigned computation.
- Work mainly from Ball plus explanation (no other texts on hand).
- Start a glossary (v1, 61 terms) and a progress log.
- Theme 0 order: **Block A** information (DNA → protein), **Block B** energy, **Block C** cells as physical objects.
