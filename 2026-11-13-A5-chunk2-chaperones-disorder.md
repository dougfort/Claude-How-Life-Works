# Session notes — A5 chunk 2: chaperones, misfolding/aggregation, intrinsically disordered proteins

**Date:** 2026-11-13
**Theme:** 0 — The standard picture · Block A — Information: DNA → protein
**Unit status after session:** A5 ☑ (complete) — Block A (A1–A5) now ☑ complete

---

## Recall (from chunk 1)

**Prompt:** What mainly drives a protein to fold, and where does most of the free-energy gain come from? Answer shape: name the effect, then say in one clause whose entropy rises and why.

**Fog's answer:** "The hydrophobic effect mainly drives a protein to fold. Burying side chains in a core releases the caged water, the free-energy gain comes mostly from water's entropy."

**Feedback:** Correct — effect named, entropy correctly attributed to water, mechanism (caging → release on burial) stated. No corrections needed.

---

## 1. Why folding needs help in vivo

Anfinsen's result (chunk 1) says the sequence *determines* the native shape, but the cell is a harder environment than Anfinsen's dilute test tube:

- **Macromolecular crowding** (link to C4/T0): ~20–30% of cytoplasm volume occupied by other macromolecules → raises effective concentration of partly-folded chains, making wrong-molecule contacts more likely.
- **Co-translational folding**: folding starts N-terminus first while the chain is still emerging from the ribosome, so the back part of the chain isn't available yet — can bias folding down a wrong local path before the full sequence exists.
- Hydrophobic patches exposed mid-folding are sticky by the *same physics* that drives correct folding — an oily surface "wants" to bury itself, and with another exposed patch nearby (crowding again) it can bury into a different molecule instead of its own core.

Misfolding is the same chemistry as folding, finding the wrong partner — not a separate exotic failure mode.

## 2. Chaperones [consensus]

A chaperone does not specify the fold — adds no shape information. It changes the **kinetics** of the search (success rate and speed), via mechanism: shielding exposed hydrophobic surface from the crowded cytoplasm until the chain folds.

- **Chaperonins** (e.g. GroEL/GroES in bacteria): barrel-shaped complex, encloses one unfolded chain in an isolated chamber; ATP-driven binding/release cycle.
- **Hsp70-family chaperones**: bind exposed hydrophobic stretches on nascent/stressed chains to prevent aggregation; ATP-dependent release gives the chain another attempt.

## 3. Misfolding and aggregation [consensus mechanism; disease link well established]

- An incompletely/incorrectly folded chain exposes hydrophobic surface a correctly folded one would have buried.
- Two such exposed chains can stick via that surface; if the resulting aggregate's shape *converts* correctly-folded copies into the same sticky form, the misfold propagates.
- **Amyloid**: a specific, highly stable, repeating cross-β sheet structure many different proteins can misfold into. Implicated in Alzheimer's (amyloid-β, tau), Parkinson's (α-synuclein), type 2 diabetes (amylin), prion disease.
- **Prions**: the sharpest case — a misfolded conformation that directly converts correctly-folded copies on contact, propagating shape with no nucleic acid involved. Direct counterexample to a *strict* reading of "one sequence, one native shape": Anfinsen's principle holds for the free-energy minimum, but prions show the cell doesn't always end up there.

## 4. Intrinsically disordered proteins/regions (IDPs/IDRs) [active research; core phenomenon settled]

- Textbook picture (chunk 1): sequence → one specific 3D structure → function.
- IDPs/IDRs: no single stable fold under physiological conditions — sample a broad conformational ensemble as their *native* state (not denatured/unfolded in the Anfinsen sense).
- Common, not rare: a large fraction of eukaryotic proteomes have substantial disordered regions, especially transcription factors (connects to the T1 glossary note on TFs having disordered regions and binding loosely).
- Functional logic: disorder enables **promiscuity** — binding multiple partners with modest, reversible affinity, sometimes folding only transiently upon binding a specific partner (**coupled folding and binding**). A rigid lock-and-key structure can't do this.

## Ball flag [Ball's interpretive claim, built on consensus biology]

Ball: IDPs show "sequence → structure → function" isn't the full story, since a large fraction of the proteome has no single structure to determine; function arises from a dynamic, context-dependent ensemble. He reads this (with splicing and promiscuous TF binding) as evidence the cell, not the gene, settles outcomes the "program" picture claims are fixed in advance.

**Where this is genuinely contested** (not just Ball's gloss): IDPs' reality and importance aren't disputed. What's debated is generalizing "no fixed structure" to "no structural specificity at all." Many IDRs still have strong sequence-level constraints (short binding motifs, charge patterning) making their behavior non-random and still "encoded" — just not as a single 3D shape. Consensus position: structure is *necessary but not sufficient* to specify function — weaker than Ball's "resource not program" framing.

---

## Check

**Question:** A chaperone and chaperone-free refolding (Anfinsen's ribonuclease) both end at the same native state. Answer shape: one clause on what the chaperone changes about getting there, one clause on what it does *not* change.

**Fog's answer:** "It changes the environment by shielding hydrophobic surfaces, or changes the success rate and speed. The chaperone does not add any shape information."

**Feedback:** Both framings correct and non-conflicting — different levels of description (mechanism: shielding; outcome: success rate/speed). Negative clause (no shape information added) correct. No correction needed — genuine answer-shape ambiguity on my end, flagged by Fog and resolved by giving both valid readings.

---

## Terms introduced this session

chaperone · chaperonin (GroEL/GroES) · Hsp70 · co-translational folding · misfolding · aggregation · amyloid · cross-β sheet · coupled folding and binding · intrinsically disordered protein / region (IDP/IDR, promoted from chunk-1 preview)

*(Also folding in chunk-1 terms not yet in the glossary: backbone, side chain/R group, Cα, φ/ψ, native state, denaturation, disulfide bond, marginal stability, two-state folding, RT, thermodynamic hypothesis, metastable state, serpin, prion, Levinthal's paradox, folding funnel/energy landscape, minimal frustration, kinetic trap — all added in glossary v6.)*

---

## Next session

**Block A quiz (A1–A5)** — the full DNA → protein chain, directly testing the diagnostic's main gap (question 4, "not recalled," 2026-11-03/04).

No new recall prompt this session — the quiz is the recall.
