# Session notes — 2026-11-05

**Theme 0 · Unit A1: DNA structure and copying** (plus recall on membranes)

Tags: **[consensus]** textbook view · **[research]** active, unsettled · **[Ball]** Ball's interpretive position

Everything in this session is **[consensus]**. Ball doesn't dispute any of it.

---

## 1. Recall: why membranes block ions, and why that matters for ATP

**Prompt:** Why does a lipid bilayer block ions, and why does that matter for making ATP?

**My answer (summary):** In water, an ion is surrounded by a shell of water molecules oriented toward its charge, which stabilizes it. Crossing the membrane means entering a nonpolar region where nothing can play that role. In mitochondria:

1. Electrons from food pass down the electron transport chain to oxygen.
2. The chain doesn't make ATP. It pumps protons across the inner membrane, building a gradient.
3. The protons flow back through ATP synthase, a rotary motor, and the spinning makes ATP.

This works only because the bilayer is impermeable to ions; if protons leaked, no gradient would build.

**Verdict:** Correct, with the right mechanism. In the diagnostic I had blamed charge repulsion, which is wrong.

### Refinements

**The barrier is an energy cost: the Born energy.** Moving a charge $q$ (ion radius $a$) from a medium that screens it well into one that screens it badly costs

$$
\Delta G \approx \frac{q^2}{8\pi\varepsilon_0 a}\left(\frac{1}{\varepsilon_{\text{core}}} - \frac{1}{\varepsilon_{\text{water}}}\right)
$$

with $\varepsilon_{\text{water}} \approx 80$ and $\varepsilon_{\text{core}} \approx 2$ for the hydrocarbon interior. The $1/\varepsilon_{\text{core}}$ term dominates, so small ions are effectively shut out. Channels and pumps work by providing a polar path through the membrane.

**The proton-motive force is partly voltage.** It's a concentration difference *plus* an electrical potential across the membrane, and in mitochondria the voltage is the larger part.

**Brown fat** proves the point: it adds a deliberate proton leak, so the energy comes out as heat instead of ATP.

---

## 2. DNA structure

- Two strands wound into a double helix, running in **opposite directions** (antiparallel).
- **Sugar-phosphate backbone** on the outside; **bases** on the inside, paired A–T and G–C.
- The backbone is the same whatever the bases are, so **any sequence is chemically allowed**. That's what lets DNA store arbitrary information.
- Each strand determines its partner, so either strand can rebuild the other.

---

## 3. Directionality: what "5′ → 3′" means

Each nucleotide contains a five-carbon sugar. Its carbons are numbered 1′–5′; the prime (′) separates sugar carbons from atoms in the base. Two of them matter:

- The **5′ carbon** carries the phosphate.
- The **3′ carbon** carries an –OH (hydroxyl) group.

Neighbouring nucleotides link from the **3′-OH of one sugar to the 5′-phosphate of the next**, so every link has the same orientation. A strand therefore has two different ends:

```
5′ end                                       3′ end
(free phosphate)                            (free –OH)
  P–[sugar]–P–[sugar]–P–[sugar]–P–[sugar]–OH
       |          |          |          |
       A          G          C          T      ← bases
```

A strand is an **oriented path**, not an undirected one: reading 5′→3′ differs from reading 3′→5′.

### Antiparallel

The two strands point in opposite directions:

```
5′ ─A─G─C─T─→ 3′
    | | | |
3′ ←─T─C─G─A─ 5′
```

A strand's partner is its **reverse complement**: read it backward, swapping each base.

### Why polymerase builds only 5′ → 3′

DNA polymerase can only add a nucleotide to a free **3′-OH**, so new strands grow only at their 3′ end.

The chemical reason is about where the energy sits:

- Each incoming nucleotide brings its own high-energy triphosphate at its 5′ end, and that powers the new bond.
- The growing chain never carries the energy supply at its tip. So when proofreading cuts out a wrong base, what's left is an ordinary 3′-OH, ready to extend.
- If chains grew the other way, the energy would sit on the chain's tip. Removing a mistake would remove the energy, and copying would stall.

**The one-direction rule is the price of being able to proofread.**

---

## 4. Copying (replication)

1. **Helicase** unzips the helix, opening a Y-shaped **replication fork**.
2. **DNA polymerase** reads each old strand and builds a complementary new strand.
3. Each new helix has **one old strand and one new strand**: *semiconservative replication* (Meselson and Stahl, 1958).
4. Polymerase can't start from nothing. Each new piece begins on a short **RNA primer**, later replaced by DNA.

---

## 5. Leading and lagging strands

### What happens

```
                         fork moves this way →

3′ ════════════════════════╗   (old strand)
   ───────────────────────→║   new: LEADING — grows toward fork, one continuous piece
                           ╠════════════════  still-paired DNA
   ←─── ←─── ←─── ←───     ║   new: LAGGING — pieces, each growing away from fork
5′ ════════════════════════╝   (old strand)

   (→ / ← mark each new strand's growing 3′ end)
```

- **Leading strand:** its growing end points toward the fork, so polymerase follows the fork continuously.
- **Lagging strand:** its growing end points away from the fork. Polymerase waits until a stretch is exposed, starts near the fork, and copies backward until it meets the previous piece. Then it repeats.
- The pieces are **Okazaki fragments**; **DNA ligase** joins them afterward.

(The session used an interactive diagram with a slider that opens the fork. The sketch above is a static stand-in.)

### Why: the causal chain

This was the hard part of the session. It's three facts in a row:

1. **Polymerase only adds at the 3′ end.** Every new strand grows in one direction only.
2. **A new strand runs opposite to the old strand it copies** (the antiparallel rule).
3. **The two old strands run opposite to each other.** So their copies also run opposite to each other: the two new strands point in opposite directions.

**Therefore:** the fork moves one way. One new strand points with it and can follow. The other *must* point against it, so it has to be made in backward pieces. The direction rule plus the antiparallel arrangement forces this.

**Common mistake (mine):** saying the lag comes from "waiting for template to be exposed." Both strands wait for exposure, so that can't be what distinguishes them. The cause is **direction**; the waiting is a consequence.

**Analogy:** two one-way lanes on a road, running in opposite directions, uncovered gradually from one end. The painter whose lane runs with the uncovering just walks forward behind it. The other painter may only walk the opposite way. He has to hop up to the newly uncovered patch, paint back toward where he's been, and hop again.

**Thought experiment:** if both DNA strands ran the *same* direction, both new strands would point toward the fork and both could be made continuously. There would be no lagging strand.

---

## 6. Accuracy and kinetic proofreading

Base-pairing energies alone would give about **1 error in 10⁴–10⁵ bases**. The real rate is about **1 in 10⁹**, through three layers:

1. **Geometric selection:** polymerase checks the shape of each incoming base pair.
2. **Proofreading:** polymerase backs up and cuts out a mismatched base.
3. **Mismatch repair:** separate enzymes re-check after copying.

### Formalization (Hopfield, 1974)

At equilibrium, the error fraction is set by the binding-energy difference $\Delta\Delta G$ between right and wrong bases:

$$
f_0 \approx e^{-\Delta\Delta G / k_B T}
$$

Each extra discrimination step that **spends free energy** to break detailed balance multiplies the error by roughly another factor of $f_0$:

$$
f \approx f_0^{\,n} \quad (n \text{ independent discrimination steps})
$$

So two steps give about $f_0^2$. **Accuracy beyond the equilibrium limit must be paid for in energy.** This idea comes back in Theme 3, where cells sense signals and make decisions.

---

## 7. Checks this session

| Check | Result |
|---|---|
| Recall: membranes block ions → ATP | ✓ Correct mechanism (loss of water shell) |
| Why must one strand be made in pieces? | ✗ Restated *what* happens, not *why* |
| Same, with hints (polymerase rule + strand arrangement) | ✗ Couldn't assemble the chain |
| If strands ran the same way, would there be a lagging strand? | ✓ "No," but reason given was wrong (exposure, not direction) |

**Status:** A1 stays in progress. The facts are in place; the causal chain behind the lagging strand needs another pass.

## 8. Next time

**Recall prompt:** *Why does one new strand have to be made in pieces?*
Target: polymerase only extends 3′ ends, and the strands are antiparallel, so one new strand necessarily points away from the fork.

Then on to **A2: Transcription**.
