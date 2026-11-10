# Session 2026-11-08 — A3: RNA processing and splicing

**Theme 0, Block A** · Unit A3 (RNA processing), chunks 1–2 · Unit status after session: ☑ done

Tags: **[consensus]** textbook view · **[research]** active, unsettled · **[Ball]** Ball's interpretive position

*Rebuilt from the chat on 2026-11-10. The recall on dimmers vs switches that opened this chat is in the 2026-11-07 notes.*

---

## 1. Processing the pre-mRNA [consensus]

The raw transcript (**pre-mRNA**) is processed **while it is still being made**:
- **5′ cap:** a modified G attached back-to-front to the front end. Protects it and helps the ribosome find it.
- **Poly-A tail:** a couple hundred A's added at the 3′ end. Protects that end and helps export.
- **Splicing:** introns cut out, exons joined.

---

## 2. Splicing: the mechanism [consensus]

Each intron is marked by three short signals: **GU** at its start, **AG** at its end, and a **branch-point A** a few dozen letters before the end.

```
Pre-mRNA      [ exon 1 ]GU ─────── intron ─────── A ── AG[ exon 2 ]
                       5′ splice site     branch point  3′ splice site

After step 1  [ exon 1 ]-OH        ╭──GU──╮
              free 3′-OH end       │      A──────AG[ exon 2 ]
                                   ╰──────╯
                                    lariat

After step 2  [ exon 1 ][ exon 2 ]          lariat → degraded
              spliced mRNA
```

- **Step 1.** The branch-point A bonds to the intron's first letter. The intron closes into a loop with a tail (a **lariat**), and exon 1 is cut free with a 3′-OH end, the same kind of reactive end as in DNA copying.
- **Step 2.** That 3′-OH attacks the boundary at AG. The exons are joined; the lariat is released and broken down.

**Energy.** Each step swaps one backbone bond for another, so the chemistry costs almost nothing. The cell's ATP goes into the machinery, which rearranges itself repeatedly and checks its choices. [consensus that ATP drives the rearrangements; how far this works as Hopfield-style proofreading is research]

**The spliceosome.** Five small RNAs plus over a hundred proteins, assembled fresh on each intron. Its catalytic core is **RNA**, like the ribosome's [consensus]. Some introns in bacteria and organelles splice *themselves* with the same two-step chemistry. The spliceosome probably descends from such a self-splicing RNA [widely favored; inferred, not proven].

---

## 3. The math: splice signals don't carry enough information

Treat a splice-site signal as a **position weight matrix**: position i has base probabilities pᵢ(b). Its information content is

$$I = \sum_i (2 - H_i), \qquad H_i = -\sum_b p_i(b)\log_2 p_i(b)$$

- A position that is always the same base contributes 2 bits; a position with any base contributes 0.
- **Measured on human genes** (Stephens & Schneider 1992): 5′ site ≈ **8 bits**, 3′ site ≈ **9 bits**.
- **Needed:** singling out one site among N positions takes about log₂ N bits. A 30,000-letter gene needs ~15 bits.
- **Shortfall:** ~7 bits, a factor of 2⁷ ≈ 100. So a gene that long contains on the order of a hundred **cryptic sites**: sequences scoring as well as a real site. They are well documented, and mutations can activate them.

**So the cell must use information beyond the splice sites** [consensus that these exist]:
- **Splicing enhancers and silencers:** short sequences in exons and introns that proteins bind to promote or block nearby sites.
- **Exon definition:** exons are short and introns long, so the machinery first recognizes an exon by pairing the sites on either side.
- **Timing:** splicing happens during transcription, so sites are presented in the order Pol II makes them.

*How* these combine to reach the cell's accuracy is **[research]**.

---

## 4. Check 1: why are 8–9 bits a problem in a long gene?

**My unaided answer.** With too few bits in the signal, a long gene can contain cryptic sites, sequences that look as good as a real splice site.

**Feedback.** The conclusion is right, but two things are missing:
1. **"Can contain" understates it.** With 8 bits, a random stretch matches about once every 2⁸ positions. A long gene is *expected* to contain **many**.
2. **The consequence.** Because decoys score as well as real sites, the signal alone **can't tell them apart**. That is why the cell needs other information.

**One-step check.** If the gene were twice as long, would the expected number of cryptic sites stay the same or roughly double?
- *My answer:* double. ✓ The count scales with length, about N/2⁸.

**Fill-in-the-blank (my completed version)**

> A signal with about 8 bits is matched by chance about once every **256** positions, so the number of chance matches grows in proportion to the gene's **length**. A long gene therefore contains **many** cryptic sites that score as well as real ones, so the signal alone **cannot** tell them apart, and the cell must use **external** information such as enhancers, exon definition and timing.

**Wording fix: "external" → "additional" or "context."** Enhancers, silencers and exon lengths are in the gene's own sequence; timing comes from how transcription runs. Nothing comes from outside the gene. This matters later: Ball's argument rests on regulation depending on *context*, and "external" would make it sound like something outside the genome does the choosing.

---

## 5. Alternative splicing [consensus]

```
Pre-mRNA   [ exon 1 ]──intron──[ exon 2 ]──intron──[ exon 3 ]
                                cassette exon

Included   [ exon 1 ][ exon 2 ][ exon 3 ]  →  protein A
Skipped    [ exon 1 ][ exon 3 ]            →  protein B
```

**Patterns**
- **Cassette exon** (above): kept or skipped.
- **Mutually exclusive exons:** exactly one of a set.
- **Alternative 5′ or 3′ sites** near an exon edge.
- **Intron retention.**

**How common.** RNA-sequencing studies around 2008: over 90% of human multi-exon genes make more than one mRNA version (**isoform**).

**Examples**
- **Bcl-x** (human): two different 5′ splice sites give a long protein that *prevents* cell suicide and a short one that *promotes* it. One gene, opposite functions.
- **Dscam** (fruit fly): four clusters of mutually exclusive exons give 12 × 48 × 33 × 2 = **38,016** possible proteins. Each neuron expresses its own subset as an identity tag, so its own branches recognize each other and spread apart.

**What it doesn't settle** [research, disputed]
- Isoform counts come from **RNA**. Proteomics finds far fewer distinct **proteins** than the RNA data predict.
- One camp (Tress and colleagues, among others) argues most genes have one dominant protein isoform, and much alternative splicing is low-level noise from the leaky signals of §3. Others argue detection methods miss rare isoforms.
- "Most genes splice alternatively" is solid. "Most genes make several functional proteins" is not established.

---

## 6. How the choice is made: the math

**Competition.** **SR proteins** bind enhancers and promote inclusion; **hnRNPs** bind silencers and promote skipping. Their levels differ by cell type, giving tissue-specific splicing. This is the A2 occupancy picture, now on RNA instead of DNA.

**ψ ("percent spliced in")** is the fraction of transcripts that include the exon (70 of 100 → ψ = 0.7). With inclusion and skipping as competing first-order processes:

$$\psi = \frac{k_{\text{inc}}}{k_{\text{inc}} + k_{\text{skip}}}$$

This has the same form as occupancy and Michaelis–Menten.

**The window-of-opportunity (kinetic coupling) model.** Splicing happens during transcription. Suppose the cassette exon has a weak 3′ site, and the competing site that allows skipping (at exon 3) exists only once Pol II (RNA polymerase II, the enzyme transcribing the gene) has made it.
- The exon gets a **window** τ = d/v to be recognized unchallenged (d = distance to the competitor, v = Pol II speed).
- If recognition is a Poisson process with rate k:

$$P(\text{recognized within window}) = 1 - e^{-kd/v}$$

- **Evidence:** mutant Pol II that runs slower changes splicing as predicted.
- **Status:** supported for many exons; how general it is remains debated [research].

---

## 7. Ball's use of this, and an assessment

**[Ball]** Alternative splicing shows a gene doesn't specify a protein. The cell's state decides which protein a gene yields, so the gene is a resource the cell draws on, not a program it executes.

**Assessment (Claude)**
- **The narrow claim** ("one gene, one protein" is false) is right and textbook consensus.
- **The broad claim doesn't follow from splicing alone.** The alternatives are encoded in sequence (exons, enhancers), and the SR proteins and hnRNPs that choose are gene products. A gene-centric biologist can coherently reply that the program is just *conditional*.
- **The circularity is real and interesting:** the genome's output depends on a cell state that the genome's output helps create. But Ball's case needs more than splicing.
- It gets stronger in **Theme 3**, where cell states are attractors of the whole network. Kept open until then.

---

## 8. Check 2: why does slowing Pol II raise inclusion of a weak exon?

**Question asked about an abbreviation first.** I asked what "Pol II" meant. Eukaryotes have three main RNA polymerases, numbered by discovery:
- **Pol I** makes ribosomal RNA.
- **Pol II** makes the pre-mRNA of protein-coding genes, plus many non-coding RNAs.
- **Pol III** makes tRNAs and other small RNAs.

In the window model, v is Pol II's speed.

**My unaided answer.** The window length is the time during which the exon with a weak splice site can be recognized before it gets replaced by a stronger competitor farther down the chain. Slowing the RNA polymerase increases the time that the alternate exon is visible.

**Feedback.** My best unaided answer so far: it gave the mechanism, not just the outcome. Two corrections and one missing link:
1. **"Gets replaced"** isn't it. The competing site doesn't exist yet because it hasn't been transcribed. Once Pol II makes it, the two compete and the stronger usually wins.
2. **"Visible"** is off. The exon stays visible after the window closes; the window gives it time **with no competition**.
3. **Missing link:** why a longer window raises inclusion.

I didn't understand what to say about ψ. Re-defined as the fraction of transcripts including the exon, then two one-step checks (more likely recognized? fraction up or down?).

**Completed sentence (mine)**

> A longer window means the weak site is **more** likely to be recognized before the competitor appears, so ψ **goes up**.

**Full chain:** slower polymerase → longer window → weak site more likely recognized in time → more transcripts include the exon → ψ up.

**A3 complete.**

---

## 9. Terms introduced (glossary v4)

5′ cap · poly-A tail · pre-mRNA · branch point · lariat · spliceosome · self-splicing intron · splice site · cryptic splice site · position weight matrix · information content · splicing enhancer / silencer · exon definition · alternative splicing · cassette exon · mutually exclusive exons · isoform · SR proteins · hnRNP proteins · percent spliced in (ψ) · kinetic coupling (window model) · (updated) RNA polymerase II

## 10. Recall prompt for next session

> Why can't the splice-site sequences alone pick out the real splice sites in a long gene?

<details>
<summary>Target answer</summary>

Each signal carries only ~8–9 bits, so chance matches occur about once every 2⁸ positions. Their number grows with gene length, so a long gene has many cryptic sites that score as well as real ones. The signal can't tell them apart, so the cell uses additional context: splicing enhancers and silencers, exon definition, and timing during transcription.

</details>

## 11. Pattern notes

- "Names the thing, skips the why" recurred on check 1. It is improving: check 2 gave the mechanism unaided.
- Abbreviations and symbols introduced once (Pol II, ψ) don't carry over. Re-define them inside check questions.
- Word precision: "replaced," "visible," "external" where the mechanism needs "competitor appears," "unchallenged," "additional context."

**Next up:** A4, the genetic code and translation.
