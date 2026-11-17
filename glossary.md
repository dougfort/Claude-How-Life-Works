# How Life Works — Glossary

Last updated: 2026-11-17 · v8 · Covers: Theme 0 diagnostic, recall on membranes, A1 (DNA structure and copying), A2 (transcription), A3 (RNA processing), A4 (genetic code and translation), A5 (protein folding, chaperones, misfolding, disordered proteins), C1 (sizes, counts, timescales), units and prefixes

Tags: **\[consensus]** textbook view · **\[research]** active, unsettled · **\[Ball]** Ball's interpretive position · _(Tn)_ theme where the term matters most

***

## Units and prefixes

**Prefixes.** Each one multiplies the unit it's attached to.

| Prefix | Symbol | Factor | In words      |
| ------ | ------ | ------ | ------------- |
| kilo   | k      | 10³    | thousand      |
| milli  | m      | 10⁻³   | thousandth    |
| micro  | µ      | 10⁻⁶   | millionth     |
| nano   | n      | 10⁻⁹   | billionth     |
| pico   | p      | 10⁻¹²  | trillionth    |
| femto  | f      | 10⁻¹⁵  | quadrillionth |

Note: "m" alone is the meter; "m" in front of another unit is milli (mM = millimolar, mV = millivolt, ms = millisecond). "µ" is the Greek letter mu standing for micro — not to be confused with μ used as a symbol in equations.

**Length**

* **m — meter.**
* **nm — nanometer** = 10⁻⁹ m. Small molecules (glucose, ATP) \~1 nm; typical protein \~5 nm; membrane thickness \~5 nm; ribosome \~25 nm.
* **µm — micrometer** (also "micron") = 10⁻⁶ m = 1,000 nm. E. coli \~1 × 2 µm; human cell \~10–20 µm.

**Volume**

* **L — liter** = 10⁻³ m³ (a cube 10 cm on a side).
* **µm³ — cubic micrometer.** A cube 1 µm on a side. 1 µm³ = 1 fL exactly.
* **fL — femtoliter** = 10⁻¹⁵ L. E. coli's volume is \~1 fL.
* **pL — picoliter** = 10⁻¹² L = 1,000 fL. A human cell is \~3 pL.

**Amount and concentration**

* **mol — mole.** A count: N_A ≈ 6 × 10²³ of anything (see Avogadro's number). The chemist's "dozen."
* **M — molar** = moles per liter (mol/L). A concentration.
* **mM — millimolar** = 10⁻³ M. ATP in cells: a few mM.
* **µM — micromolar** = 10⁻⁶ M.
* **nM — nanomolar** = 10⁻⁹ M. Typical transcription-factor K_d values. In an E. coli cell, 1 nM ≈ 1 molecule.

**Energy, temperature, voltage**

* **J — joule;** **kJ — kilojoule** = 1,000 J. **kJ/mol — kilojoules per mole:** energy per mole of molecules (divide by N_A for energy per molecule).
* **K — kelvin.** Absolute temperature; 0 K is absolute zero. 310 K = 37 °C, body temperature.
* **k\_BT** — Boltzmann's constant × absolute temperature: thermal energy per molecule. (RT is the same thing per mole; see RT.)
* **mV — millivolt** = 10⁻³ volt. Membrane voltages are \~100–200 mV.

**Sequence length**

* **bp — base pair.** One rung of the DNA ladder; the unit of DNA length. **Mbp** = million base pairs (E. coli genome 4.6 Mbp); **Gbp** = billion base pairs (human genome 3.1 Gbp per copy).
* **nt — nucleotide.** Unit of length for single-stranded RNA or DNA. **kb — kilobase** = 1,000 bases (or base pairs).

**Time and rate**

* **s — second.** **min — minute.** **h — hour.**
* **ms — millisecond** = 10⁻³ s. **µs — microsecond** = 10⁻⁶ s. **ns — nanosecond** = 10⁻⁹ s. **ps — picosecond** = 10⁻¹² s. **fs — femtosecond** = 10⁻¹⁵ s.
* Rough cell timescales: bond vibration \~10 fs; side-chain flips \~ns; protein folding µs to s; enzyme turnover \~0.1 s (median); E. coli division \~20 min; human cell division \~24 h.
* **/s or s⁻¹ — per second** (a rate, e.g. amino acids added per second).

***

**3′ end / 5′ end** — The two chemically different ends of a DNA or RNA strand, named after carbons in the sugar. The 5′ end has a free phosphate; the 3′ end has a free –OH. Every link in the backbone runs 3′-OH → 5′-phosphate, so a strand has a direction, like an arrow. New strands can grow only at the 3′ end ("synthesis runs 5′ → 3′"). \[consensus] _(T0)_

**5′ cap** — A modified G attached back-to-front to the 5′ end of pre-mRNA early in transcription. Protects the RNA's front end and helps the ribosome find it. \[consensus] _(T0)_

**A, P and E sites** — The three tRNA slots in the ribosome. **A** (aminoacyl): where the incoming loaded tRNA binds over the current codon. **P** (peptidyl): holds the tRNA carrying the growing chain. **E** (exit): where the emptied tRNA leaves. Each cycle the tRNAs shift A → P → E. \[consensus] _(T0)_

**Activation barrier (activation energy, ΔG‡)** — The energy hump a reaction must get over between starting molecules and products. Rate depends on it exponentially: k ∝ e^(−ΔG‡/k_BT). Enzymes lower it. _(T0)_

**Activator** — A regulatory transcription factor that increases how often transcription starts, mainly by helping RNA polymerase land and stay on the promoter. \[consensus] _(T0, T1)_

**Active site** — The pocket in a folded enzyme whose shape and chemistry fit a particular substrate; where catalysis happens. _(T0, T2)_

**Aggregation (protein)** — Misfolded or partly-folded proteins sticking together via hydrophobic surface that correct folding would have buried. If the resulting assembly's shape can convert correctly-folded copies into the same sticky form, the misfold propagates (see amyloid, prion). The same hydrophobic chemistry that drives correct folding, finding the wrong partner — not a separate failure mode. \[consensus mechanism] _(T2)_

**Alternative splicing** — Joining a gene's exons in different combinations, so one gene yields several mRNA isoforms. Patterns: cassette exons, mutually exclusive exons, alternative 5′/3′ splice sites, intron retention. Over 90% of human multi-exon genes make more than one isoform \[consensus]; how many of those isoforms make _functional_ proteins is disputed — proteomics finds far fewer than RNA data predict \[research]. Ball reads it as the cell, not the gene, deciding the product \[Ball]. Examples: Bcl-x (opposite functions from one gene), fly Dscam (38,016 possible isoforms). _(T1)_

**Amino acid** — The building block of proteins. There are 20 standard ones, differing in their side chains (oily, charged, polar). _(T0)_

**Aminoacyl-tRNA synthetase** — Enzyme that attaches the correct amino acid to its tRNA, spending ATP; roughly one per amino acid. **This is the step that fixes what each codon means**: codon–anticodon pairing matches tRNA to codon but never checks the amino acid, so the ribosome inserts whatever is attached (Chapeville et al. 1962: cysteine on tRNA^Cys chemically converted to alanine → alanine inserted at cysteine codons). The ATP spent here also stores the energy later used to make the peptide bond. \[consensus] _(T0)_

**Amyloid** — A specific, highly stable, repeating cross-β sheet structure that many different, otherwise unrelated proteins can misfold into. Implicated in Alzheimer's (amyloid-β, tau), Parkinson's (α-synuclein), type 2 diabetes (amylin). \[consensus disease link] _(T2)_

**Anfinsen's principle** — A protein's amino-acid sequence determines its folded shape. \[consensus] for many proteins, with caveats: some need chaperones, some never fold (see intrinsically disordered protein), some end up metastable rather than at the global minimum (see prion). _(T0, T2)_

**Anticodon** — The three letters on a tRNA that pair (antiparallel) with a codon on the mRNA. _(T0)_

**Antiparallel** — The two strands of DNA run in opposite chemical directions (labeled 5′→3′ and 3′→5′). Combined with polymerase's one-direction rule, this is what forces a lagging strand. _(T0)_

**Archaea** — One of the two groups of prokaryotes (the other is bacteria). Look like bacteria but are a distinct lineage; eukaryotes likely arose from an archaeal host. _(T0)_

**ATP (adenosine triphosphate)** — The cell's energy _currency_, not storage. Splitting off a phosphate (ATP → ADP + Pi) releases \~20 k_BT under cellular conditions. Useful because the cell keeps the ATP/ADP ratio far from equilibrium. A human recycles roughly their body weight in ATP daily. Concentration a few mM (\~2 million molecules in an E. coli cell). _(T0)_

**ATP synthase** — A rotary motor in the mitochondrial inner membrane. Protons flowing through it spin it, and the rotation makes ATP. _(T0)_

**Avogadro's number (N_A)** — ≈ 6 × 10²³: the number of molecules in one mole. Converts between counts and concentrations: N = c · V · N_A (c in mol/L, V in liters). \[consensus] _(T0)_

**Backbone (protein)** — The repeating N–Cα–C chain running through a protein, the same in every amino acid; side chains hang off Cα and give each position its chemical identity. The peptide bond within it is planar (partial double-bond character); flexibility comes from the rotation angles φ and ψ on either side of each Cα. _(T2)_

**Bacteria** — Prokaryotes; single cells with no nucleus, typically 1–2 µm (micrometers). _(T0)_

**Base pairing (complementary)** — A pairs with T (U in RNA), G pairs with C. Each DNA strand therefore determines the other, which is the basis of copying. _(T0)_

**Born energy** — The energy cost of moving a charged ion from water into a low-dielectric medium such as a membrane's oily core: ΔG ≈ (q²/8πε₀a)(1/ε_core − 1/ε_water), with ε_water ≈ 80 and ε_core ≈ 2. Large enough to keep small ions out of the bilayer. \[consensus] _(T0)_

**Branch point** — A single A inside an intron, a few dozen letters before its 3′ end. In splicing step 1 it bonds to the intron's first letter, forming the lariat. \[consensus] _(T0)_

**Brown fat** — Tissue that deliberately leaks protons across mitochondrial membranes (via the protein thermogenin) to turn food energy into heat. _(T0)_

**Cassette exon** — An exon that is either included or skipped, giving two isoforms. The simplest pattern of alternative splicing. \[consensus] _(T1)_

**Catalyst** — Something that speeds a reaction without being used up. Speeds forward and reverse equally, so it changes rate, not the final equilibrium. _(T0)_

**Chaperone** — A protein that helps other proteins fold correctly or prevents misfolding/aggregation. Adds no shape information (Anfinsen's principle still holds) — changes the _kinetics_ of the search: raises success rate and speed, mainly by shielding exposed hydrophobic surface from the crowded cytoplasm until the chain folds. \[consensus] _(T0, T2)_

**Chaperonin** — A barrel-shaped chaperone (e.g. bacterial GroEL/GroES) that encloses a single unfolded chain in an isolated internal chamber, shielding it from the rest of the crowded cytoplasm; cycles via ATP-driven binding and release. \[consensus] _(T2)_

**Chemiosmosis** — Making ATP using a proton gradient across a membrane. Mitchell, 1961; ridiculed, then Nobel 1978. \[consensus] Used by essentially all life. _(T0)_

**Coding strand** — The DNA strand _not_ read during transcription. Its sequence matches the RNA's (with T in place of U), which is why gene sequences are conventionally written as the coding strand. \[consensus] _(T0)_

**Codon** — Three consecutive letters of mRNA, read by the ribosome as one unit. 4³ = 64 codons: 61 specify amino acids, 3 are stop signals. _(T0)_

**Co-translational folding** — Folding that begins while the chain is still emerging from the ribosome, N-terminus first, so later parts of the sequence aren't yet available. Can bias folding down a wrong local path before the full chain exists — one reason folding in vivo needs more help than Anfinsen's test tube. _(T0, T2)_

**Cooperative binding** — Binding of one molecule makes binding of the next more likely (e.g. transcription factors that touch each other on adjacent sites). Turns the soft occupancy curve into a steep switch (see Hill function). \[consensus] _(T0, T3)_

**Copy number** — How many molecules of a given species a cell contains. Ranges enormously: \~10 lac repressors vs. \~10⁵ EF-Tu in one E. coli cell. Rule of thumb: in an E. coli cell (\~1 fL), **1 molecule ≈ 1 nM** (exactly 0.6 molecules at 1 nM); in a human cell (\~3 pL), 1 nM ≈ 1,800 molecules. At single-digit copy numbers, "concentration" is a statistical average and binding events cause large relative fluctuations — the root of gene-expression noise (T3). \[consensus] _(T0, T3)_

**Coupled folding and binding** — An intrinsically disordered region folding into a specific, transient shape only upon binding a particular partner, rather than holding one fold beforehand. Lets a single disordered region bind different partners in different ways. _(T2)_

**Cross-β sheet** — The repeating structural motif of amyloid: stacked β-sheets running perpendicular to the fibril axis. Unusually stable, which is why amyloid aggregates resist clearance. \[consensus] _(T2)_

**Cryptic splice site** — A sequence that scores as well as a real splice site but normally isn't used. Expected in large numbers because splice-site signals carry too little information (see information content); mutations can activate them. \[consensus] _(T0, T1)_

**Cytoplasm** — The cell's interior outside the nucleus; crowded, not a dilute soup. _(T0)_

**Cytoskeleton** — The internal protein scaffolding of eukaryotic cells; gives shape and carries out active transport. _(T0)_

**Cα (alpha carbon)** — The central carbon of each amino acid in a protein backbone; the side chain and the backbone's two flexible rotation angles (φ, ψ) are both anchored here. _(T2)_

**Degradation rate (α_deg)** — The rate constant at which a cell actively destroys a molecule (proteins by proteases, mRNAs by nucleases); units of 1/time. One of two removal routes in dp/dt = k − (α_deg + α_dil)p; see dilution, response time. Most bacterial proteins have α_deg ≈ 0 (stable); actively degraded ones are used where fast responses are needed. \[consensus] _(T0, T3)_

**Denaturation** — Loss of a protein's native fold, by heat, chemical disruption (e.g. urea) or breaking stabilizing bonds (e.g. reducing disulfides). Anfinsen's ribonuclease experiment denatured, then spontaneously re-folded, the protein. _(T2)_

**Desolvation** — Stripping an ion's shell of oriented water molecules. The main reason ions can't cross a lipid bilayer: nothing in the oily core can replace the shell's stabilization (see Born energy, hydration shell). _(T0)_

**Dielectric constant (ε)** — How strongly a medium screens electric charge. Water ≈ 80 (screens strongly); hydrocarbon ≈ 2 (barely screens). _(T0)_

**Diffusion** — Random thermal motion of molecules. Time to cover distance L scales as t \~ L²/(2dD) (d = dimensions, D = diffusion coefficient): fast over nanometers, hopeless over centimeters. A protein crosses E. coli (\~1 µm) in \~0.05 s; a 20 µm human cell takes \~400× longer (\~20 s). _(T0, T3)_

**Dilution (growth dilution, α_dil)** — Loss of concentration because a growing cell spreads the same molecules through more volume; at division, existing copies are shared between the two daughters, so nothing is destroyed. Rate α_dil = ln 2 / T_div (T_div = doubling time; ln 2 ≈ 0.69). In fast-growing bacteria it is the main way stable proteins are "removed," so their response time ≈ one cell cycle (Alon, ch. 2). Zero in cells that never divide (e.g. neurons). \[consensus] _(T0, T3)_

**Dissociation constant (K_d)** — For T + site ⇌ T·site: K_d = \[T]\[site]/\[T·site] = k_off/k_on. It is a concentration: the one at which the site is half occupied. Small K_d = tight binding, mainly because the bound molecule falls off slowly, so fewer molecules are needed to keep the site covered. \[consensus] _(T0, T3)_

**Disulfide bond (S–S)** — A covalent cross-link between two cysteine side chains, stabilizing a folded shape from outside the backbone. Anfinsen's ribonuclease has four; breaking and re-forming them (with a reducing agent) was key to his refolding experiment and its scrambled control. _(T2)_

**DNA** — Deoxyribonucleic acid. A double-stranded helical polymer of nucleotides; stores hereditary sequence. 2 bits per base pair; human genome ≈ 3.1 × 10⁹ bp (base pairs). _(T0)_

**DNA ligase** — Enzyme that seals the gaps between Okazaki fragments, joining them into one continuous strand. _(T0)_

**DNA polymerase** — Enzyme that builds a new DNA strand complementary to a template. Can only add to an existing 3′ end, so it needs a primer to start and builds only 5′ → 3′. Most also proofread. _(T0)_

**Electron transport chain** — Membrane proteins in mitochondria that pass electrons from food molecules to oxygen, using the energy to pump protons across the membrane. _(T0)_

**Elongation (translation)** — The repeated cycle that adds one amino acid per codon: (1) a loaded tRNA is delivered to the A site; (2) the peptide bond forms, moving the whole chain onto the A-site tRNA; (3) translocation moves the ribosome one codon along. \~10–20 amino acids/s in bacteria, \~5/s in human cells. \[consensus] _(T0)_

**Elongation factors** — GTP-carrying proteins that run the elongation cycle: one escorts loaded tRNAs to the A site (EF-Tu in bacteria, eEF1A in eukaryotes); another drives translocation (EF-G / eEF2). EF-Tu is among the most abundant bacterial proteins (\~10⁵ copies per cell). \[consensus] _(T0)_

**Endosymbiosis** — One cell living inside another. Mitochondria descend from engulfed bacteria. \[consensus] _(T0)_

**Enhancer** — In eukaryotes, a DNA region bound by activators that can lie thousands of base pairs from the gene it controls; the DNA loops so the bound activators reach the promoter. \[consensus] Not the same as a _splicing_ enhancer (see splicing enhancer / silencer). _(T0, T1)_

**Enzyme** — A biological catalyst, usually a protein (sometimes RNA — see ribozyme). Rate enhancements \~10⁶ to \~10¹⁷. _(T0)_

**Eukaryote** — Cell with a nucleus and internal membrane compartments (animals, plants, fungi, protists). Typically 10–30 µm (micrometers). _(T0)_

**Exon** — Part of a gene's RNA that is kept after splicing. Usually short (\~150 letters on average in humans). _(T0, T1)_

**Exon definition** — Because exons are short and introns long, the splicing machinery first recognizes an exon by pairing the splice sites on either side of it. One source of information beyond the splice sites themselves. \[consensus] _(T0)_

**Folding funnel / energy landscape** — The resolution \[consensus on the picture, active research on details] to Levinthal's paradox: the space of conformations isn't searched blindly but is shaped like a funnel, with most native-like contacts lowering free energy, biasing the search downhill. Sequences selected for **minimal frustration** (favorable interactions mostly agree) have the steepest, cleanest funnels. _(T2)_

**Frameshift** — An insertion or deletion of a number of letters that isn't a multiple of 3, shifting the reading frame so every codon downstream is misread (usually hitting a stop soon). Crick–Brenner (1961) used frameshifts to show the code is read in triplets. \[consensus] _(T0)_

**Gene** — No single agreed definition. Molecular sense: a stretch of DNA that is transcribed into a functional product. Evolutionary sense: a unit inherited and selected over generations (Dawkins' usage). "A sequence that codes for a protein" is inaccurate: misses non-coding genes, alternative splicing, and regulatory DNA. \[consensus that the simple definition fails] _(T1)_

**General transcription factors** — In eukaryotes, the set of proteins needed at essentially every RNA polymerase II promoter to position the polymerase and open the DNA (TFIID, TFIIB and others). Contrast regulatory transcription factors, which vary gene to gene. \[consensus] _(T0)_

**Genetic code** — The many-to-one map from 64 codons to 20 amino acids plus stop. Redundant (log₂20 ≈ 4.3 bits needed, 6 bits available), and arranged so single-letter errors often swap in a chemically similar amino acid (Freeland & Hurst 1998) \[consensus that it is error-minimizing; why it ended up so is debated — research]. _(T0, T5)_

**Glycolysis** — First stage of breaking down glucose, in the cytoplasm; yields a little ATP without oxygen. _(T0)_

**GTP (guanosine triphosphate)** — ATP's close chemical relative. Used by translation factors; on the ribosome its hydrolysis is the irreversible step that separates the two accuracy checks (see kinetic proofreading). _(T0)_

**Half-life (t½)** — Time for a quantity decaying exponentially at rate α to fall to half: t½ = ln 2 / α (ln 2 ≈ 0.69). E. coli mRNAs: mostly a few minutes \[consensus]. Mouse cells: median \~9 h for mRNA, \~46 h for protein (Schwanhäusser et al. 2011) \[research; method-dependent, later studies often find shorter mRNA lifetimes]. _(T0, T3)_

**Helicase** — Enzyme that unzips the DNA double helix ahead of copying, opening the replication fork. _(T0)_

**Hill function** — θ = \[T]ⁿ/(Kⁿ + \[T]ⁿ). Occupancy curve for cooperative binding; n (Hill coefficient) sets steepness. n = 1 is the ordinary single-site curve; larger n approaches an on/off switch. Seed of bistable switches in Theme 3. _(T0, T3)_

**hnRNP proteins** — RNA-binding proteins that typically bind splicing silencers and promote exon skipping. Compete with SR proteins; their balance differs by cell type. \[consensus] _(T1)_

**Hsp70** — A family of chaperones that bind exposed hydrophobic stretches on nascent or stressed chains to prevent aggregation; ATP-dependent release gives the chain another folding attempt. \[consensus] _(T2)_

**Hydration shell** — The layer of water molecules that surrounds a dissolved ion, oriented toward its charge. Strongly stabilizes the ion. _(T0)_

**Hydrophilic / hydrophobic** — "Water-loving" (polar or charged; interacts favorably with water) / "water-fearing" (nonpolar). About interaction, not chemical reaction. _(T0)_

**Hydrophobic effect** — Nonpolar molecules cluster in water mainly because it frees water molecules from ordered cages — an entropy gain. Drives membrane formation and protein folding (where it is the main driving force — see two-state folding). _(T0, T2)_

**Induced fit** — An enzyme changes shape as it binds its substrate (Koshland). Refines lock-and-key. The ribosome's decoding site uses it too, sensing the geometry of codon–anticodon pairing. _(T0, T2)_

**Information content (of a sequence motif)** — For a position weight matrix: I = Σᵢ (2 − Hᵢ) bits, Hᵢ = −Σ_b pᵢ(b) log₂ pᵢ(b). A fully fixed position gives 2 bits; a random one gives 0. Picking one site out of N positions needs \~log₂ N bits; with I bits, chance matches occur about N/2^I times. Human splice sites: \~8 bits (5′) and \~9 bits (3′) (Stephens & Schneider 1992) — well short of what a long gene needs. _(T0, T3)_

**Initiation (translation)** — Getting the ribosome onto the right start codon. Eukaryotes: the small subunit with the initiator tRNA binds at the 5′ cap and scans to the first AUG. Bacteria: a Shine–Dalgarno sequence positions the ribosome directly. The large subunit then joins. Sets the reading frame. \[consensus] _(T0)_

**Initiator tRNA** — Special tRNA carrying methionine that begins every protein; it starts in the P site rather than entering at A. \[consensus] _(T0)_

**Intrinsically disordered protein / region (IDP / IDR)** — A protein, or a region of one, with no single fixed fold under physiological conditions — it samples a broad conformational ensemble as its _native_ state (not "unfolded" in the denaturation sense). Common in eukaryotic proteomes, especially in transcription factors. Functionally useful for promiscuous, reversible binding to multiple partners, sometimes folding transiently only on binding a specific partner (see coupled folding and binding). \[consensus that the phenomenon is real and widespread; active research on how far "no fixed structure" generalizes — many IDRs retain strong sequence-level constraints (motifs, charge patterning)] Ball reads IDPs as evidence that "sequence → structure → function" isn't the whole story, since there is often no single structure to determine \[Ball]. _(T2)_

**Intron** — Part of a gene's RNA that is cut out during splicing. Often thousands of letters; makes up most of a typical human gene's length. Starts with GU, ends with AG. _(T0, T1)_

**Isoform** — One of the alternative mRNA (or protein) versions made from the same gene. _(T1)_

**Kinetic coupling ("window of opportunity" model)** — Because splicing happens during transcription, an exon with a weak site gets a window τ = d/v (distance to the competing site ÷ Pol II speed) to be recognized unchallenged. With recognition rate k: P(recognized) = 1 − e^(−kd/v). Slower Pol II → longer window → higher ψ. Supported for many exons; generality debated \[research]. _(T1, T3)_

**Kinetic proofreading** — Hopfield (1974). Copying machinery spends energy to recheck and reject errors, reaching accuracy beyond what binding energies allow. Equilibrium error f₀ ≈ e^(−ΔΔG/k_BT); n energy-consuming discrimination steps give roughly f₀ⁿ. Accuracy beyond the equilibrium limit costs energy. Examples: DNA copying (\~1 error per 10⁹ bp with all layers), synthetase editing, and the ribosome's two-stage tRNA selection separated by irreversible GTP hydrolysis (f ≈ f₀², f₀ \~ 10⁻² → \~10⁻⁴). _(T0, T3)_

**Kinetic trap** — A local, non-global free-energy minimum where a folding (or search) process can get stuck; shown as a side pocket on a folding-funnel diagram. _(T2)_

**Lac repressor** — The bacterial transcription factor that shuts off the lactose-digesting genes when no lactose is present. Classic repressor; only \~10 copies per E. coli cell (≈ 10 nM). Binds its site far more tightly than 1 nM, so the gene is off almost all the time \[consensus]; rare single unbinding events let through bursts of expression (Choi et al. 2008) \[research]. _(T0, T1, T3)_

**Lagging strand** — The new DNA strand whose growing 3′ end points away from the replication fork. It can't follow the fork, so it is made in backward pieces (Okazaki fragments). Cause: polymerase's 5′ → 3′ rule plus antiparallel strands — not "waiting for exposed template," which both strands do. \[consensus] _(T0)_

**Lariat** — The loop-with-a-tail shape an intron takes during splicing, after the branch-point A bonds to the intron's first letter. Released and degraded after the exons are joined. \[consensus] _(T0)_

**Leading strand** — The new DNA strand whose growing 3′ end points toward the replication fork, so it is made continuously as the fork opens. \[consensus] _(T0)_

**Levinthal's paradox** — Levinthal (1969): with \~3 conformations per amino acid, a 100-residue chain has 3¹⁰⁰ ≈ 10⁴⁷ possible shapes; sampling 10¹³/s would take \~10²⁷ years, yet real folding takes microseconds to seconds. Resolved by the folding funnel. _(T2)_

**Lipid bilayer** — Two sheets of phospholipids, tails inward, heads facing water on both sides. Self-assembles. Nearly impermeable to ions because they'd have to lose their hydration shell to enter the nonpolar core (see Born energy). _(T0)_

**Lock and key** — Fischer's picture of enzyme specificity: rigid complementary shapes. Superseded in part by induced fit; Ball argues recognition is looser still \[Ball]. _(T0, T2)_

**Macromolecular crowding** — Large molecules occupy \~20–30% of cytoplasm volume. Raises the effective concentration of partly-folded chains, making wrong-molecule contacts (misfolding, aggregation) more likely than in a dilute test tube. _(T0, T2)_

**Marginal stability** — ΔG(unfold) for most proteins is typically only \~20–60 kJ/mol, roughly a few hydrogen bonds — a small difference between two large opposing terms (the chain's lost entropy vs. the gains from burial and bonding). A mutation costing 10–20 kJ/mol can tip the balance toward unfolding. _(T2)_

**Membrane protein** — Protein embedded in a membrane: channels (let ions through), pumps (push ions against gradients), receptors (detect signals). About half a membrane's mass. _(T0, T3)_

**Messenger RNA (mRNA)** — The processed RNA copy of a gene (capped, spliced, poly-A tailed) that leaves the nucleus and is translated by ribosomes. _(T0)_

**Metastable state** — A folded (or other) state that is stable and kinetically trapped but is not the global free-energy minimum. Exceptions to "sequence determines the one native shape," either by design (serpins) or by accident (prions). _(T2)_

**Michaelis–Menten kinetics** — Standard model of enzyme rate: v = V_max\[S] / (K_M + \[S]). Rises with substrate, then saturates. Same functional form as single-site occupancy. _(T0, T3)_

**Minimal frustration** — The evolutionary principle that a protein's favorable interactions mostly agree with each other, so folding doesn't have to fight itself; gives the folding funnel its clean downhill bias. Formalized (Zwanzig 1992): a bias of a few RT per residue against incorrect local conformations cuts search time from astronomical to milliseconds — the same mathematics as a biased vs. unbiased random walk. _(T2)_

**Mismatch repair** — Enzymes that scan newly copied DNA and fix mispaired bases the polymerase missed. The third layer of copying accuracy. _(T0)_

**Missense error** — A wrong amino acid inserted during translation. Ribosome rate roughly 1 in 10³–10⁴ per codon. \[consensus] _(T0)_

**Mitochondrion** — Eukaryotic organelle, descended from a bacterium, where most ATP is made via chemiosmosis. \~1 µm long. Lane argues mitochondria made complex cells possible by vastly raising energy per gene \[research]. _(T0)_

**Mutually exclusive exons** — A set of exons of which exactly one is included in each transcript. Fly Dscam has four such clusters: 12 × 48 × 33 × 2 = 38,016 combinations. \[consensus] _(T1)_

**Native state** — The folded, functional conformation a protein normally settles into; usually (but not always — see metastable state) the global free-energy minimum. _(T2)_

**N-terminus / C-terminus** — The two ends of a protein chain: the free amino group (N) and the free carboxyl group (C). Proteins are built N → C while the mRNA is read 5′ → 3′. \[consensus] _(T0)_

**Non-coding RNA** — RNA that functions as RNA and is never translated: tRNA, ribosomal RNA, microRNAs, long non-coding RNAs. _(T1)_

**Nonsense mutation** — A change that turns an amino-acid codon into a stop codon inside a gene. A release factor binds there and the truncated protein is released. \[consensus] _(T0)_

**Nonsense-mediated decay** — Eukaryotic quality control that destroys mRNAs whose ribosomes stop too early (typically before the last exon–exon junction), so little truncated protein accumulates. \[consensus] _(T0)_

**Nucleotide** — Building block of DNA/RNA: a sugar, a phosphate, and one base (A, T/U, G, C). _(T0)_

**Nucleus** — Membrane-bound compartment holding a eukaryote's DNA. \~5 µm across. Separates transcription from translation, enabling RNA processing. _(T0)_

**Occupancy (θ)** — Fraction of time a binding site is bound. Single site: θ = \[T]/(\[T] + K_d) = 1/(1 + K_d/\[T]); in stat-mech terms, empty has weight 1, bound has weight \[T]/K_d. θ = ½ exactly when \[T] = K_d. A single site is a soft dimmer: 10% → 90% occupancy needs an 81-fold rise in \[T]. Example: 10 nM factor, K_d = 1 nM → θ = 10/11 ≈ 0.91. \[consensus] _(T0, T3)_

**Okazaki fragment** — One of the short pieces in which the lagging strand is made; later joined by DNA ligase. _(T0)_

**Peptide bond** — The bond joining amino acids in a protein. On the ribosome, the chain on the P-site tRNA is transferred onto the amino acid of the A-site tRNA; catalyzed by ribosomal RNA. Its energy comes from the synthetase's earlier ATP spend, not from new ATP. Partial double-bond character makes it planar and non-rotating (see backbone). \[consensus] _(T0, T2)_

**Percent spliced in (ψ, PSI)** — The fraction of a gene's transcripts that include a given exon (70 of 100 → ψ = 0.7). Simple competition model: ψ = k_inc/(k_inc + k_skip), same form as occupancy. _(T1, T3)_

**Phospholipid** — Membrane molecule with a charged/polar head and two hydrocarbon tails. _(T0)_

**Poly-A tail** — A run of a couple hundred A's added to the 3′ end of pre-mRNA. Protects that end and helps export from the nucleus. \[consensus] _(T0)_

**Polysome** — One mRNA being translated by many ribosomes at once, spaced along it. _(T0)_

**Position weight matrix** — A table of base probabilities pᵢ(b) at each position of a sequence signal; used to score candidate sites and compute information content. _(T0, T3)_

**Pre-mRNA** — The raw RNA transcript before splicing and capping. Processed while still being transcribed. _(T0)_

**Primer** — Short RNA stretch that gives DNA polymerase a 3′ end to start from (polymerase can't start a strand from nothing). Later replaced by DNA. _(T0)_

**Prion** — A misfolded protein conformation that directly converts correctly-folded copies of the same protein into the same misfolded shape on contact, propagating without any nucleic acid involved. A metastable state, not the global free-energy minimum — the sharpest exception to a strict reading of Anfinsen's principle. \[consensus] _(T2)_

**Prokaryote** — Cell with no nucleus: bacteria and archaea. _(T0)_

**Promoter** — DNA region where RNA polymerase binds to start transcription. Its orientation sets the direction of transcription and so which strand is the template. _(T0, T1)_

**Proofreading (polymerase)** — DNA polymerase backs up and cuts out a wrongly added base before continuing. Works because the chain's tip carries no energy supply, so removing a base leaves an ordinary 3′ end that can still extend. (Contrast the ribosome, where the energy sits on the chain's tip, so checking happens mainly _before_ the bond forms.) _(T0)_

**Protein** — A chain of amino acids that folds into a functional shape. Typical size \~5 nm (nanometers) across. An E. coli cell holds \~3 million; a human cell \~1–10 billion. _(T0)_

**Proton gradient (proton-motive force)** — Difference in proton concentration and voltage across a membrane (\~150–200 mV across \~5 nm in mitochondria); in mitochondria the voltage is the larger part. Powers ATP synthase. _(T0)_

**Reading frame** — Which of the three possible ways of grouping letters into triplets is used. Set by the start codon; everything downstream is counted in threes from it. _(T0)_

**Release factor** — Protein that recognizes a stop codon in the A site (no tRNA matches stop codons) and makes water cut the finished chain off the P-site tRNA. \[consensus] _(T0)_

**Replication fork** — The Y-shaped region where the double helix is being unzipped and both strands copied. _(T0)_

**Repressor** — A regulatory transcription factor that decreases transcription, classically by sitting on a site that overlaps the promoter so polymerase can't bind (e.g. the bacterial lac repressor). \[consensus] _(T0, T1)_

**Response time** — Time for a molecule's concentration to get halfway to a new steady state after its production rate k changes. From dp/dt = k − (α_deg + α_dil)p: steady state p\* = k/(α_deg + α_dil), response time t½ = ln 2/(α_deg + α_dil). Set by the _removal_ rates, not by k. For a stable bacterial protein (α_deg ≈ 0), t½ ≈ one cell cycle (Alon, _An Introduction to Systems Biology_, ch. 2). \[consensus] _(T0, T3)_

**Reverse complement** — A DNA strand's partner sequence: read the strand backward and swap each base (A↔T, G↔C). Follows from antiparallel pairing. _(T0)_

**Ribosome** — Large RNA–protein machine that translates mRNA into protein. \~25 nm across; \~10⁴–7×10⁴ per E. coli cell depending on growth rate. Small subunit holds the mRNA and monitors codon–anticodon pairing; large subunit forms peptide bonds and has the A, P and E sites. Its catalytic core is RNA (a ribozyme). _(T0)_

**Ribozyme** — An RNA molecule that acts as an enzyme. Examples: the ribosome's core, the spliceosome's core, self-splicing introns. _(T0)_

**RNA** — Ribonucleic acid. Usually single-stranded; uses U instead of T. Carries messages, does catalysis, regulates genes. _(T0, T1)_

**RNA polymerase** — Enzyme that builds an RNA copy of a DNA strand. Reads the template 3′→5′ and builds RNA 5′→3′, so the RNA's growing 3′ end faces the direction of travel. Needs no primer; error rate much higher than DNA polymerase (\~1 in 10⁴–10⁵), tolerable because RNA copies are many and short-lived. Speed: \~40–80 nt/s in E. coli. _(T0)_

**RNA polymerase II (Pol II)** — The eukaryotic RNA polymerase that transcribes protein-coding genes into pre-mRNA (and many non-coding RNAs). Needs the general transcription factors to start; its long tail carries the RNA-processing machinery. Speed \~1–4 kb per minute; the longest human gene (dystrophin, \~2.2 Mbp) takes \~16 h per transcript. Eukaryotes have three main RNA polymerases, numbered by discovery: Pol I (ribosomal RNA), Pol II (pre-mRNA), Pol III (tRNAs, small RNAs). _(T0)_

**RNA world hypothesis** — Early life used RNA for both information and catalysis before DNA and proteins. \[research] — widely favored, unproven. _(T0)_

**RT** — Gas constant × absolute temperature (R·T); thermal energy per mole, the Boltzmann factor k_BT written per mole (R = N_A·k_B). At 310 K (kelvin), RT ≈ 2.6 kJ/mol (kilojoules per mole). Appears in two-state folding (K = e^(−ΔG/RT)) and elsewhere any Boltzmann-type ratio is written per mole instead of per molecule. _(T2)_

**Self-splicing intron** — An intron (in some bacteria and organelles) that cuts itself out using the same two-step chemistry as the spliceosome. Probably the spliceosome's ancestor \[widely favored; inferred]. _(T0)_

**Semiconservative replication** — Each new DNA double helix has one old strand and one new strand. Meselson–Stahl, 1958. \[consensus] _(T0)_

**Serpin** — A class of protein deliberately folded into a metastable, "spring-loaded" state rather than the global free-energy minimum, so it can snap to a lower-energy shape when triggered (e.g. to trap a target protease). A designed exception to "native state = global minimum." _(T2)_

**Shine–Dalgarno sequence** — Short bacterial mRNA sequence just upstream of the start codon that pairs with the ribosome's own RNA, positioning the ribosome without scanning. \[consensus] _(T0)_

**Side chain (R group)** — The chemical group hanging off each amino acid's Cα that gives it its identity (oily, polar, or charged). Which side chains end up buried vs. exposed, and how they interact, is what makes a sequence fold into a particular shape. _(T0, T2)_

**Sigma factor** — Bacterial protein that joins RNA polymerase and recognizes promoter sequences, positioning the polymerase; released once transcription is under way. \[consensus] _(T0)_

**Splice site** — Short signal sequences marking intron boundaries: GU at the intron's 5′ end (5′ splice site), AG at its 3′ end (3′ splice site). Carry only \~8–9 bits, so cryptic look-alikes are common. Mutations here can cause intron retention or exon skipping. _(T0, T1)_

**Spliceosome** — The machine that splices pre-mRNA: five small RNAs plus over a hundred proteins, assembled fresh on each intron. Its catalytic core is RNA. Spends ATP on rearrangements, not on the bond chemistry. \[consensus] _(T0)_

**Splicing** — Cutting introns out of pre-mRNA and joining exons, in two steps: (1) branch-point A attacks the 5′ splice site, forming a lariat and freeing exon 1's 3′-OH; (2) that 3′-OH attacks the 3′ splice site, joining the exons. Each step swaps one backbone bond for another. Happens during transcription. \[consensus] _(T0, T1)_

**Splicing enhancer / silencer** — Short sequences in exons or introns that, when bound by proteins (SR proteins, hnRNPs), promote or block use of nearby splice sites. Supply information the splice sites lack. \[consensus] _(T0, T1)_

**SR proteins** — RNA-binding proteins that typically bind splicing enhancers and promote exon inclusion. Compete with hnRNPs. \[consensus] _(T1)_

**Start codon** — AUG (methionine); marks where translation begins and sets the reading frame. \[consensus] _(T0)_

**Stop codon** — UAA, UAG, UGA. No tRNA matches them; a release factor binds instead and ends translation. \[consensus] _(T0)_

**Substrate** — The molecule an enzyme acts on. _(T0)_

**Surface-to-volume ratio (S/V)** — Membrane area per unit of interior volume. For a sphere of radius r, S/V = 4πr² / (4/3 πr³) = 3/r: a cell 10× wider has 10× less membrane per unit volume. Matters because bacteria make ATP at their outer membrane (B5). Lane argues this caps bacterial size and that mitochondria broke the cap by internalizing energy-making membranes \[research / Lane's position, contested — B6]. The geometry itself is \[consensus]. _(T0)_

**Synthetase editing ("double sieve")** — Second check by aminoacyl-tRNA synthetases: a separate editing site cuts off wrong amino acids small enough to slip into the loading site (e.g. valine wrongly loaded onto tRNA^Ile). A form of kinetic proofreading. \[consensus] _(T0)_

**TATA box** — Short A/T-rich sequence about 25–30 bp upstream of the start site in some eukaryotic promoters (a minority in humans); bound by TATA-binding protein, part of the general transcription machinery. \[consensus] _(T0)_

**Template strand** — The DNA strand read by RNA polymerase; the RNA is complementary to it. Which strand serves as template is set by the promoter's orientation and can differ from gene to gene. \[consensus] _(T0)_

**Termination (translation)** — A stop codon reaches the A site, a release factor binds, the chain is cut free, and the subunits separate. \[consensus] _(T0)_

**Thermodynamic hypothesis (Anfinsen)** — The claim that a protein's native structure is its global free-energy minimum, and the amino acid sequence alone determines where that minimum is. Supported by Anfinsen's 1961 ribonuclease refolding (and its scrambled-disulfide control); the 2024 Chemistry Nobel (AlphaFold, protein design) rests on this premise. \[consensus, with caveats — see metastable state] _(T2)_

**Thermodynamic model (of gene regulation)** — Assumption that transcription rate is proportional to promoter/site occupancy computed at binding equilibrium. Widely used and often works, but real initiation has energy-consuming, non-equilibrium steps; where the model fails is studied actively. \[research] _(T0, T3)_

**Transcription** — Making an RNA copy of a DNA sequence, by RNA polymerase, in the nucleus (in eukaryotes). Opens both strands, reads one — so there is no lagging-strand problem. _(T0)_

**Transcription bubble** — The short region (\~10–15 bp) of unwound DNA that travels with RNA polymerase; the DNA rewinds behind it. A bubble, not a fork: only one strand is being copied. _(T0)_

**Transcription factor** — Protein that binds DNA and helps control whether a gene is transcribed. Two kinds: _general_ (needed at every promoter to seat polymerase) and _regulatory_ (recognize specific short sequences, \~6–12 bp; activators or repressors). A gene's output depends on how often its regulatory sites are occupied (see occupancy). \[consensus] Many have disordered regions and bind loosely, so "one factor, one site" is too tidy \[Ball; developed further via intrinsically disordered protein, T2]. _(T0, T1)_

**Transfer RNA (tRNA)** — Adapter RNA carrying one amino acid and recognizing the matching codon via its anticodon. Which amino acid it carries is set by its synthetase, not by the ribosome. _(T0)_

**Transition state** — The unstable halfway configuration at the top of the activation barrier. Enzymes work by binding it more tightly than the substrate (Pauling). _(T0)_

**Translation** — Building a protein from mRNA, by ribosomes, codon by codon, in three phases: initiation, elongation, termination. A 300-amino-acid protein takes \~20 s in E. coli, \~1 min in human cells. _(T0)_

**Translocation** — The GTP-driven step that moves the ribosome exactly one codon along the mRNA, shifting tRNAs A → P → E and opening the A site for the next codon. \[consensus] _(T0)_

**Turnover number (k_cat)** — The maximum number of reactions one enzyme molecule catalyzes per second when saturated with substrate; V_max = k_cat × \[enzyme] in Michaelis–Menten. Median across known enzymes \~10 per second; fastest \~10⁶–10⁷ per second (e.g. carbonic anhydrase) (Bar-Even et al. 2011). \[consensus] _(T0)_

**Two-state folding** — Model of folding as an equilibrium between unfolded (U) and native (N) states: K = \[U]/\[N] = e^(−ΔG/RT), fraction folded = 1/(1 + K). Same mathematical form as single-site binding occupancy (A2). _(T2)_

**Uncoupling** — Letting protons leak back across the membrane without passing through ATP synthase; food energy becomes heat instead of ATP. _(T0)_

**Wobble** — Loose pairing at the codon's third position (Crick 1966), so one tRNA can read several codons that differ only there. Fewer tRNAs than the 61 sense codons are needed. \[consensus] _(T0)_
