# Session notes — A5 chunk 1: protein folding (chain, driving force, Anfinsen, funnel)

**Dates:** 2026-11-11 to 11-12
**Theme:** 0 — The standard picture · Block A — Information: DNA → protein
**Unit status after session:** A5 ◐ (chunk 1 of 2 done)

---

## Recall (from A4)

**Prompt:** Why does the ribosome's error rate come out near f₀² rather than f₀? Answer shape: name the energy-spending step, then say in one clause what its being irreversible forces.

**Fog's answer:** "The GTP hydrolysis step spends energy. The step being irreversible forces a second error check."

**Feedback:** Step correct. Second clause was incomplete. A second check alone doesn't give f₀². If the step between the two checks could run backward, the second check would settle into the same equilibrium as the first and add nothing. Irreversibility makes the checks **independent**, and independent chances multiply.

**Fill-in (Fog, correct):** "Because GTP hydrolysis can't run backward, a wrong tRNA can't **return** to the first check. So it has to pass two **independent** checks, and the two error fractions **multiply**." ✓

---

## 1. The chain

- A protein is a chain of amino acids joined by **peptide bonds**, built by the ribosome (A4).
- Repeating **backbone**: N–Cα–C. Each amino acid's identity comes from its **side chain** (R group) on the central carbon, Cα.
- The peptide bond is partly a double bond, so it's flat and doesn't rotate. The flexibility comes from two rotation angles per amino acid, **φ and ψ**, on either side of Cα. (This ψ is unrelated to the splicing ψ from A3.)

| Group | Examples | Role in folding |
|---|---|---|
| Hydrophobic (oily) | Leu, Ile, Val, Phe | Buried in the core |
| Polar, uncharged | Ser, Thr, Asn, Gln | Surface; hydrogen bonds |
| Charged | Asp, Glu (−); Lys, Arg (+) | Surface; salt bridges |
| Special | Gly (tiny, flexible), Pro (kinks), Cys (S–S cross-links) | Local geometry |

## 2. Why it folds: mostly the hydrophobic effect [consensus]

- Water can't hydrogen-bond to oily side chains, so it forms ordered "cages" around them. Burying them in a core releases that water.
- At body temperature the gain is **mostly water's entropy**, not attraction between oily groups. This is the same physics as bilayer impermeability (C4), seen from the other side.
- Hydrogen bonds inside the protein (helices, sheets) replace the bonds the buried backbone lost with water.
- **Marginal stability:** ΔG(unfold) is typically about 20–60 kJ/mol, roughly a few hydrogen bonds. It's a small difference between two large opposing terms: the chain's lost entropy against the gains from burial and bonding.

**Formalization: two-state folding.** U (unfolded) ⇌ N (native):

    K = [U]/[N] = e^(−ΔG/RT)        fraction folded = 1 / (1 + K)

- **RT** = gas constant × absolute temperature = thermal energy per mole (R = N_A·k_B). At 310 K, RT ≈ 2.6 kJ/mol. It's the Boltzmann factor written per mole.
- This is the same two-state partition-function form as binding occupancy (A2).
- At ΔG = 40 kJ/mol (≈ 16 RT), about 1 molecule in 10⁷ is unfolded at any moment. A mutation costing 10–20 kJ/mol can tip the balance.

## 3. Anfinsen: the sequence contains the shape [consensus, with caveats]

- **1961, ribonuclease.** Fully unfolded with urea (disrupts folding forces) plus a reducing agent (breaks the 4 S–S cross-links). Activity lost. Both removed slowly, in a test tube with no cell present: it **refolded on its own** and recovered nearly full activity. Nobel Prize 1972.
- **Thermodynamic hypothesis:** the native structure is the free-energy minimum, and the amino acid sequence determines where it is.
- **Control:** when cross-links formed *before* the urea was removed, the result was scrambled and nearly inactive. A trace of reducing agent, letting cross-links break and re-form, rescued it. The information is in the sequence, but the chain has to be free to search.
- **Caveats:** some proteins sit in a metastable state rather than the global minimum, either by design (serpins, a spring-loaded fold) or by accident (prions).
- The 2024 Chemistry Nobel (AlphaFold structure prediction; Baker's protein design) rests on Anfinsen's premise.

## 4. Levinthal's paradox and the funnel

- **Levinthal (1969):** with 3 conformations per amino acid, a 100-residue chain has 3¹⁰⁰ ≈ 10⁴⁷ shapes. Sampling 10¹³ per second would take about 10²⁷ years. Real folding takes microseconds to seconds.
- **Resolution** [consensus on the picture, active research on the details]: the landscape is a **funnel**. Most native-like contacts lower the free energy, so the search is biased downhill. Evolution selected sequences with **minimal frustration**, meaning their favorable interactions mostly agree.
- **Formalization (Zwanzig 1992):** a small bias of a few RT per amino acid against incorrect local conformations cuts the search time from astronomical to milliseconds. It's the same mathematics as a biased random walk compared with an unbiased one: exponential search time becomes roughly linear in distance.

```
 Free energy        width = number of conformations (entropy)
     |      \ . . . . . . . . . . . . . . . /    <- unfolded ensemble:
     |       \_                          _ /        many shapes, high G
     |         \_    \       |      /  _/
     |           \_   \      |     /  /_
     |             \   \     |    / [x]     <- kinetic trap (side pocket)
     |              \_  \    |   / _/
     v                \_ \   |  /_/
   lower                 \_\ | //
                            (N)              <- native state
```

## Ball flag

- "Sequence → structure → function" is textbook consensus. Ball stresses that many proteins, especially in eukaryotes, have long stretches that never fold into one shape (intrinsically disordered regions). This is an active research area. **Deferred to chunk 2.**

---

## Check

**Question:** Anfinsen's ribonuclease refolded in a test tube with no cell present. Answer shape: (1) name one thing in the cell that this rules out as the source of the folded shape, then (2) say in one clause where the shape information must be instead.

**Fog's first answer:** "(1) water cages (2) the nucleotide sequence."

**Feedback:**
- The question was ambiguous: "a thing in the cell" includes water. The intended meaning was something the cell has that the test tube lacked.
- (1) Water was in the test tube, so the hydrophobic effect was operating. It's part of the folding mechanism, not something ruled out. What's ruled out is the cell's **machinery**: ribosome, chaperones, any external template.
- (2) One step too far back. There was no DNA or mRNA in the tube, only protein. The information is in the **amino acid sequence**, which the nucleotide sequence encodes.

**One-step checks:** (a) DNA or mRNA in the tube? **No** ✓ (b) Ribosomes or chaperones in it? **No** ✓

**Fill-in (Fog, correct):** "The test tube had none of the cell's **machinery**, so the shape information must be in the protein's own **amino acid** sequence." ✓

---

## Terms introduced

backbone · side chain (R group) · Cα · peptide bond (planar) · φ, ψ (backbone rotation angles) · hydrophobic effect · native state · denaturation · disulfide (S–S) bond · marginal stability · two-state folding · RT · thermodynamic hypothesis (Anfinsen) · metastable state · serpin · prion · Levinthal's paradox · folding funnel / energy landscape · minimal frustration · kinetic trap · intrinsically disordered region (preview)

*(To be added to the glossary when A5 is complete.)*

---

## Next session

A5 chunk 2: chaperones, misfolding and aggregation, intrinsically disordered proteins and Ball's reading of them. Then the Block A quiz.

**Recall prompt:** What mainly drives a protein to fold, and where does most of the free-energy gain come from? Answer shape: name the effect, then say in one clause whose entropy rises and why.

<details>
<summary>Target answer</summary>

The hydrophobic effect. Mostly it's **water's** entropy that rises: oily side chains force water into ordered cages, and burying them in the core releases that water.

</details>
