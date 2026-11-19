# Block A Quiz — DNA → Protein (A1–A5)

Covers A1 (DNA structure & copying), A2 (transcription), A3 (RNA processing), A4 (genetic code & translation), A5 (protein folding). This is the chain the Theme 0 diagnostic flagged as the main gap (question 4, "not recalled," 2026-11-03/04) — this quiz is the direct re-test of it.

**How to use:** Answer each question in your own words first, in writing. Only then open the `<details>` block. No scoring pressure — the point is to see exactly where a chain breaks, if it breaks.

_Corrected 2026-11-19: Q1's answer key originally said the_ template _strand's 3′ end faces away from the fork. That was wrong — it is the_ new _strand's growing 3′ end. Fixed below\._

***

**Q1 (A1).** Walk the full causal chain from "DNA's two strands are antiparallel" to "one new strand is made in Okazaki fragments." State it as A → B → C → D (four short links).

\<details> \<summary>Answer\</summary>

Antiparallel strands → DNA polymerase can only add nucleotides to the new strand's 3′ end (builds 5′→3′) → so on one template, the _new_ strand's growing 3′ end points _away_ from the fork (on that side the template's own 3′ end points toward the fork) → polymerase on that strand can't follow the fork continuously, so it builds short pieces backward (Okazaki fragments), later joined by ligase.

\</details>

***

**Q2 (A1).** Why does DNA polymerase need a primer, but DNA ligase doesn't?

\<details> \<summary>Answer\</summary>

Polymerase can only _add_ a nucleotide to an existing 3′-OH — it cannot start a chain from nothing, so it needs a primer to supply that first 3′ end. Ligase isn't building a new strand; it's sealing an existing nick between two already-synthesized pieces (joining a 3′-OH to a 5′-phosphate that are already there, side by side).

\</details>

***

**Q3 (A2).** A gene's promoter sits on the strand conventionally written left-to-right. Which strand is the template strand, and which direction does RNA polymerase move along the DNA?

\<details> \<summary>Answer\</summary>

The promoter's orientation sets transcription direction. If the promoter reads left-to-right on the "top" (coding) strand, RNA polymerase travels left-to-right along the DNA, which means it is reading the _bottom_ strand (3′→5′, left to right) as template, producing RNA that matches the top/coding strand (with U for T). The template strand is whichever one RNA polymerase actually reads — determined by promoter orientation, not fixed to "top" or "bottom."

\</details>

***

**Q4 (A2).** Transcription factor X has a tenfold lower K_d than factor Y for its own binding site. What does that mean physically in terms of k_on and k_off, and what does it imply about where X's occupancy curve sits compared to Y's?

\<details> \<summary>Answer\</summary>

K_d = k_off/k_on, and K_d is the concentration at which a site is half-occupied. A tenfold lower K_d mainly means X falls off its site (k_off) much more slowly than Y falls off its site — once bound, X stays bound longer. Physically: X's occupancy curve (θ vs. \[T]) is shifted left relative to Y's — X reaches half-occupancy at a tenfold lower concentration, so X will be substantially occupied at concentrations where Y is barely bound at all.

\</details>

***

**Q5 (A3).** Splice sites carry only \~8–9 bits of information. Give the reasoning in two short sentences: (a) why that's a problem on its own, (b) what actually solves it in the cell.

\<details> \<summary>Answer\</summary>

(a) A human gene is large enough that \~8–9 bits isn't enough to pick out the real splice site uniquely — by chance alone, cryptic look-alike sites with the same score should occur often, and the signal alone can't tell real from cryptic. (b) Splicing enhancers/silencers (bound by SR proteins / hnRNPs), exon definition (pairing sites across a short exon rather than a long intron), and timing (the window-of-opportunity kinetic coupling with Pol II speed) all supply additional context that the bare splice-site sequence lacks.

\</details>

***

**Q6 (A3).** Ball reads alternative splicing as evidence the gene is a "resource," not a "program." What's the narrow version of this claim that's uncontroversial, and why doesn't the broad version follow automatically from splicing alone?

\<details> \<summary>Answer\</summary>

Narrow, consensus claim: "one gene → one protein" is false — one gene routinely yields multiple distinct protein products depending on splicing choices made after transcription. Broad claim (Ball's): this shows genes are a flexible resource the cell draws on as needed, rather than a fixed program. This doesn't follow automatically because the alternatives themselves, and the splicing factors (SR/hnRNP balance) that choose among them, are _also_ encoded in the genome — the "choice" is itself a product of other genetically-specified machinery, so it's not obviously a departure from "programmed," just a more indirect, context-dependent program. (Deferred to Theme 3: cell states as network attractors, where this gets a fuller answer.)

\</details>

***

**Q7 (A4).** Why does the genetic code need 3-letter codons rather than 2 or 1? Use the information argument.

\<details> \<summary>Answer\</summary>

20 amino acids need log₂20 ≈ 4.3 bits to distinguish. One letter (4 options: A/U/G/C) gives only 2 bits — far short. Two letters give 4² = 16 combinations ≈ 4 bits — still short of 20. Three letters give 4³ = 64 combinations ≈ 6 bits — enough to cover 20 amino acids with room to spare (hence the redundancy: 61 sense codons for 20 amino acids).

\</details>

***

**Q8 (A4).** At which single step is "what amino acid this codon means" actually fixed? What experiment demonstrated this, and what did it show?

\<details> \<summary>Answer\</summary>

It's fixed at the aminoacyl-tRNA synthetase step — when the synthetase attaches a specific amino acid to a specific tRNA. Codon–anticodon pairing in the ribosome checks only that the tRNA matches the codon; it never checks which amino acid is attached. Chapeville et al. (1962) showed this directly: they chemically converted the cysteine already attached to tRNA^Cys into alanine. The ribosome still inserted alanine wherever a cysteine codon appeared — proving the ribosome reads the tRNA, not the amino acid, and that the synthetase step is what actually fixes codon meaning.

\</details>

***

**Q9 (A4/A2 integration).** DNA polymerase and the ribosome both achieve higher-than-equilibrium accuracy by spending energy, but via different strategies — one checks mainly _before_ the bond forms, one mainly _after_. Name which does which, and explain why the difference traces to where the energy supply sits on the growing chain.

\<details> \<summary>Answer\</summary>

DNA polymerase proofreads _after_ the bond forms: it backs up and excises a wrongly-added base, which works because the chain's 3′ tip carries no stored energy — removing a base just leaves an ordinary 3′-OH that can still extend normally. The ribosome's major accuracy step happens mainly _before_ the peptide bond forms: GTP hydrolysis (an irreversible, energy-spending step) gates a second, independent check on the tRNA before the bond is made — because on the ribosome the energy for the eventual bond is already stored on the chain's tip (from the synthetase's earlier ATP spend), so you can't "back up and redo" the same way; you have to get it right going in.

\</details>

***

**Q10 (A5).** A protein and a prion-converted version of the same protein have identical amino acid sequences but different stable folds. What does this say about Anfinsen's principle, interpreted strictly vs. loosely?

\<details> \<summary>Answer\</summary>

Strict reading ("sequence determines _the_ folded shape, full stop") is falsified by prions — same sequence, two different stable conformations. Looser, correct reading: sequence determines the free-energy _landscape_ (which shapes are possible and how stable each is), and under normal conditions the cell reaches the global minimum — but prions show the landscape can have more than one deep, stable well, and which one a molecule ends up in isn't determined by sequence alone; it can depend on which conformation it was exposed to (template-like propagation from existing misfolded copies).

\</details>

***

**Q11 (A5).** Explain why intrinsically disordered regions are a genuine complication for "sequence → structure → function," distinguishing the settled part of the claim from Ball's stronger reading of it.

\<details> \<summary>Answer\</summary>

Settled part: a large fraction of eukaryotic proteins (especially transcription factors) have regions with no single stable fold — they function as a dynamic ensemble, sometimes folding only transiently when they bind a specific partner. This means "structure" in the rigid, single-shape sense isn't what's doing the functional work for these regions, so "structure" can't be inserted as a universal middle step between sequence and function. Ball's stronger reading: generalizes this to suggest sequence doesn't tightly determine behavior at all for these regions — function is contextual, decided by the cell/environment in the moment. The more cautious consensus view: many disordered regions still carry strong sequence-level constraints (short binding motifs, charge patterning) that make their behavior highly non-random — so it's "necessary but not sufficient," not "unconstrained by sequence."

\</details>
