# Session 2026-11-09 — A4 chunk 1: The genetic code, tRNA and synthetases

**Theme 0, Block A** · Unit A4 (genetic code and translation), chunk 1 · Unit status after session: ◐ (chunk 2, the ribosome, done 2026-11-10)

Tags: **[consensus]** textbook view · **[research]** active, unsettled · **[Ball]** Ball's interpretive position

*Rebuilt from the chat on 2026-11-10.*

---

## 1. Planning: Block A quiz

Agreed to a quiz across A1–A5, held until **after A5**, so that it covers the whole DNA → protein → shape chain, the main gap in the diagnostic.

---

## 2. Recall: why can't splice sites alone pick out the real sites?

**My answer (unaided).** The splice-site sequence contains too few bits. There are multiple matches in a long gene.

**Feedback.** First two links right, unaided. "Many" is better than "multiple": the number grows with gene length.

**Completion (mine).**

> Since those chance matches score as well as the real sites, the signal alone **is not sufficient**, so the cell must **use other means**.

**Feedback.** Correct, with two precision points:
- The exact point is that the signal **can't tell real sites from decoys**.
- "Other means" is too vague. Name them: **additional context**, meaning splicing enhancers and silencers, exon definition, and timing during transcription.

---

## 3. The counting problem [consensus]

mRNA has 4 letters; proteins use 20 amino acids. How long must a codon be?
- 2 letters: 4² = 16 words, too few.
- **3 letters: 4³ = 64 words**, enough with room to spare.

**In information terms:** picking one of 20 amino acids needs log₂ 20 ≈ **4.3 bits**; a codon carries **6 bits**. The extra capacity is **redundancy**:
- 61 codons code for amino acids; 3 mean **stop**.
- Most amino acids have several codons.
- **AUG** means methionine and is also the usual **start** signal.

---

## 4. Reading frames and frameshifts

There's no punctuation between codons. The start codon fixes where the triplets begin; the ribosome then reads three letters at a time.

```
...A U G G C U U U C A A A...
   AUG GCU UUC AAA        frame set by AUG: Met Ala Phe Lys
```

Insert or delete one letter and every codon downstream shifts: a **frameshift**.

**Crick & Brenner (1961)** used such mutations to show the code is read in non-overlapping triplets. One insertion destroyed function; three nearby insertions often restored it.

---

## 5. The code is a lookup table, implemented by adapters

Nothing chemical makes GCU mean alanine. **The codon never touches the amino acid.**

```
   [Synthetase] ──attaches──► (Ala)
                                 │
                            ┌────┴────┐
                            │  tRNA   │
                            │3′-CGA-5′│  ← anticodon
                            └─┬─┬─┬───┘
                              ┆ ┆ ┆      base-pairing (antiparallel)
   5′ [ AUG ][ G C U ][ UUC ][ AAA ] 3′   mRNA codons
```

- **tRNA** is the adapter. One end carries an amino acid. The other end has a three-letter **anticodon** that pairs with a codon, antiparallel as in DNA.
- **Aminoacyl-tRNA synthetases** are ~20 enzymes, roughly one per amino acid. Each recognizes its amino acid *and* its tRNAs (by the tRNA's whole shape, not just the anticodon) and joins the two.

**The key point.** Codon–anticodon pairing only checks that the tRNA matches the codon. **What a codon means is set when the synthetase loads the tRNA.** If a synthetase loads the wrong amino acid, the ribosome inserts it anyway.

---

## 6. Synthetase accuracy: another case of proofreading [consensus]

- **The puzzle.** Isoleucine and valine differ by a single CH₂ group. From binding energy alone, f₀ ≈ e^(−ΔΔG/k_BT), the isoleucine synthetase would load valine roughly once every hundred or two attempts. Pauling flagged this in the 1950s.
- **Observed error:** around one in tens of thousands.

**The answer: a "double sieve."**
1. The loading site rejects anything **bigger** than isoleucine.
2. A separate **editing site** is too small for isoleucine but fits valine, so it hydrolyses valine off any tRNA it was wrongly loaded onto.

Each sieve gives a factor of discrimination, and they **multiply**, the same f₀ⁿ structure as Hopfield's kinetic proofreading (A1). ATP spent loading a wrong amino acid is wasted; that is the energy cost of accuracy.

---

## 7. How the code is arranged

- **Wobble** [consensus]. Synonymous codons mostly differ in the **third** letter (GCU, GCC, GCA, GCG all mean alanine). Pairing at that position is looser, so one tRNA can read several synonymous codons.
- **Error-minimizing.** Single-letter errors often give the same or a chemically similar amino acid. Freeland & Hurst (1998): the standard code beats about a million random codes on this measure [widely cited].
- **Why it's arranged this way** is disputed [research]:
  - selection optimized it;
  - it reflects how the code expanded historically;
  - Crick's "frozen accident": fixed early by chance.
- **Universality.** The code is nearly universal, with small variants in mitochondria and a few microbes.

---

## 8. Check: which molecule decides that GCU means alanine?

**Question.** Which molecule actually determines that GCU means alanine: the mRNA, the tRNA's anticodon, or the synthetase? And why?

**My answer.** The synthetase joins the amino acid with the tRNA.

**Feedback.** Correct choice. But it says what the synthetase *does*, not why that makes it the deciding step.

**One-step check.** When the anticodon pairs with GCU, does that pairing check which amino acid the tRNA carries?
- *My answer:* no. ✓

**On parsing questions.** I said I often can't parse what a question wants, with people too. Claude agreed the question was ambiguous: "which molecule, and why?" can mean *what does it do* (which I answered correctly) or *what makes it the decider* (what was wanted). Some logged "skips the why" was likely this ambiguity.

**New rule:** every check question states the **shape** of the answer wanted, for example:
- "name the cause in one clause"
- "rule out the other options"
- "give the chain A → B → C"

**Fill-in-the-blank (my completed version)**

> Because the anticodon pairing doesn't check the amino acid, the ribosome adds whatever amino acid **is loaded with the tRNA**. So which amino acid a codon means is fixed at the step where **the synthetase loads the tRNA**.

**Feedback:** correct.

---

## 9. Terms introduced (glossary v5, added 2026-11-10)

codon (updated: 61 sense + 3 stop) · start codon · stop codon · reading frame · frameshift · anticodon · aminoacyl-tRNA synthetase · synthetase editing ("double sieve") · wobble · genetic code (updated: error-minimizing arrangement)

## 10. Recall prompt for next session

> Which step fixes which amino acid a codon means? *Shape:* name the step, then say in one clause why codon–anticodon pairing can't be it.

<details>
<summary>Target answer</summary>

The synthetase loading the tRNA. Pairing matches tRNA to codon but never checks the amino acid, so the ribosome inserts whatever is attached.

</details>

## 11. Pattern notes

- Recall: the first two links came unaided. The consequence was stated vaguely ("not sufficient," "other means"); name the specifics.
- **Answer-shape rule adopted** for all check questions from here on.

**Next up:** A4 chunk 2, the ribosome.
