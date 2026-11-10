# Session 2026-11-10 — A4 chunk 2: Translation and the ribosome

**Theme 0, Block A** · Unit A4 (genetic code and translation), chunk 2 · Unit status after session: ☑ done

Tags: **[consensus]** textbook view · **[research]** active, unsettled · **[Ball]** Ball's interpretive position

---

## 1. Recall: what fixes what a codon means?

**Question.** Which step fixes which amino acid a codon means? *Shape:* name the step, then one clause on why codon–anticodon pairing can't be it.

**My answer.** Set when the synthetase loads the tRNA; codon–anticodon pairing only checks that the tRNA matches the codon.

**Feedback.** Right step. The second clause said what pairing *does* check. The argument needs what it *never* checks: **the ribosome never inspects the amino acid**, so it inserts whatever the tRNA carries.

**Evidence: Chapeville et al. (1962).** tRNA^Cys was loaded with cysteine, and the cysteine was then chemically converted to alanine while still attached. The ribosome inserted alanine wherever the mRNA said cysteine. The adapter is trusted blindly. [consensus]

---

## 2. The ribosome's layout

Two subunits:
- **Small subunit:** holds the mRNA and monitors codon–anticodon pairing.
- **Large subunit:** forms peptide bonds and holds three tRNA slots.

| Site | Name | What sits there |
|---|---|---|
| **A** | aminoacyl | incoming loaded tRNA, over the current codon |
| **P** | peptidyl | tRNA holding the growing chain |
| **E** | exit | emptied tRNA on its way out |

```
              growing chain (exits through the large subunit)
                   o
                  o
           +------o-------------------+
           |  E      P       A        |   large subunit
           | [  ]  [tRNA]  [tRNA]o    |   (o on A-site tRNA = next amino acid)
  5' ======|========================  |======== 3'   mRNA
           |                          |   small subunit
           +--------------------------+
                ribosome moves one codon at a time  -->  toward 3'
```

---

## 3. The three phases of translation [consensus]

### Initiation: getting onto the right AUG
- **Eukaryotes.** The small subunit carries the **initiator tRNA**, which is loaded with methionine. It binds at the 5′ cap and **scans** along the mRNA to the first AUG.
- **Bacteria.** A **Shine–Dalgarno sequence** just upstream of the AUG pairs with the ribosome's own RNA. This positions the ribosome directly, with no scanning.
- The large subunit then joins, with the initiator tRNA already in the **P** site.
- **This step sets the reading frame.** Every later codon is counted in threes from this AUG.

### Elongation: one cycle per codon
1. **Delivery.** A loaded tRNA is escorted to the A site by a GTP-carrying factor (EF-Tu in bacteria, eEF1A in eukaryotes).
2. **Peptide bond.** The whole growing chain moves off the P-site tRNA and onto the amino acid on the A-site tRNA. The chain is now one longer and hangs from A. The catalyst is the large subunit's **RNA**, so the ribosome is a ribozyme.
3. **Translocation.** A second GTP factor (EF-G / eEF2) moves the ribosome exactly one codon along. The tRNAs shift A → P → E, the empty one leaves, and A opens over the next codon.

**Direction and speed.**
- Protein is built **N-terminus → C-terminus** while the mRNA is read **5′ → 3′**.
- Speed is ~10–20 amino acids/s in bacteria and ~5/s in human cells.
- Many ribosomes translate one mRNA at once; this is called a **polysome**.

### Termination
- Stop codons (UAA, UAG, UGA) have **no matching tRNA**.
- A **release factor** (a protein shaped somewhat like a tRNA) binds the A site instead.
- It makes water cut the chain off the P-site tRNA. The protein is released and the subunits separate.

---

## 4. Energy accounting

| Cost | Paid by | Used for |
|---|---|---|
| ATP | the synthetase, when loading the tRNA | stored in the tRNA–amino acid bond; drives the peptide bond later |
| GTP | the elongation factors | movement (translocation) and accuracy |

The ribosome spends **no new ATP on the peptide bond**.

**Contrast with DNA copying (A1).**
- In DNA copying, the energy arrives with each *incoming* nucleotide, so the chain's tip carries none. A wrong base can be cut out afterward, leaving an ordinary 3′ end that can still extend.
- In translation, the energy sits on the **growing chain's tip**, the bond to the P-site tRNA.
- So the ribosome's main checking has to happen **before** the bond forms.

---

## 5. Accuracy as kinetic proofreading [consensus]

Third appearance of Hopfield's scheme (after DNA polymerase and synthetase editing).

- **Pairing energy alone.** A right versus near-right anticodon gives an equilibrium error f₀ ≈ e^(−ΔΔG/k_BT) ~ 10⁻².
- **Two checks.** The ribosome checks once when the tRNA arrives. Then **GTP hydrolysis**, which is **irreversible**, separates that from a second, independent rejection step.
- **The checks multiply.** Because the GTP step can't run backward, a wrong tRNA must pass both:

  f ≈ f₀ · f₀ = f₀² ≈ 10⁻⁴

- **Measured missense error.** About 1 in 10³–10⁴ per codon.
- **Induced fit.** The decoding site also physically senses the geometry of the first two codon–anticodon base pairs.
- **Open question.** How evolution tuned the speed–accuracy trade-off is **[research]**.

---

## 6. Check: a premature stop codon

**Question.** A mutation turns a mid-gene codon UGG (tryptophan) into UGA (stop). What happens during translation? *Shape:* two-link chain. First, what occupies the A site; second, what that does to the protein.

**My answer.** A release factor occupies the A site. The truncated protein is released.

**Feedback.** Correct on both links, unaided.

**Addition: nonsense-mediated decay.** In eukaryotes, quality control often destroys an mRNA whose ribosomes stop too early, typically before the last exon–exon junction. So little truncated protein accumulates. [consensus]

---

## 7. Terms introduced or updated (glossary v5)

A, P and E sites · elongation · elongation factors · GTP · initiation · initiator tRNA · missense error · N-terminus / C-terminus · nonsense mutation · nonsense-mediated decay · peptide bond · polysome · release factor · Shine–Dalgarno sequence · start codon · stop codon · termination · translocation · (updated) ribosome, kinetic proofreading, proofreading (polymerase), aminoacyl-tRNA synthetase

## 8. Recall prompt for next session

> Why does the ribosome's error rate come out near f₀² rather than f₀? *Shape:* name the energy-spending step, then say in one clause what its being irreversible forces.

<details>
<summary>Target answer</summary>

GTP hydrolysis between initial selection and proofreading. Because it can't run backward, a wrong tRNA has to pass two independent checks, so the error fractions multiply.

</details>

## 9. Pattern notes

- The answer-shape rule worked: both the recall and the check were answered in the requested shape.
- Recurring minor slip: asked why X *can't* do something, the answer describes what X *does*. The logic is there; the phrasing misses the negative.

**Next up:** A5, protein folding and shape. Then the Block A quiz (A1–A5).
