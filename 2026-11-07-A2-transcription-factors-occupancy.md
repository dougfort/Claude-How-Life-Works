# Session 2026-11-07 — A2 chunk 3: Transcription factors and binding occupancy

**Theme 0, Block A** · Unit A2 (transcription), chunk 3 · Unit status after session: ☑ done

Tags: **[consensus]** textbook view · **[research]** active, unsettled · **[Ball]** Ball's interpretive position

*Rebuilt from the chats on 2026-11-10. Includes the short follow-up recall from later the same day.*

---

## 1. Recall: why no lagging-strand problem in transcription?

**My answer.** Only one strand is being read, in the 3′ direction.

**Feedback.** Right word this time (*read*). With only one strand copied, no second strand has its growing end pointing the wrong way. But "in the 3′ direction" is too vague: two molecules (template and RNA) run in opposite directions, so the phrase could describe either.

**One-step check.** Which end of the growing RNA faces the polymerase's direction of travel?
- *My answer:* 3′. ✓

**Precise version.** The polymerase reads the template 3′→5′ and builds the RNA 5′→3′. The RNA's growing 3′ end faces the direction of travel, so it extends continuously. The promoter's orientation decides which strand is the template.

---

## 2. Regulatory transcription factors [consensus]

- **General** transcription factors (last session) are needed at every promoter to seat polymerase.
- **Regulatory** transcription factors sit on top of those. Each recognizes a short DNA sequence (~6–12 bp) and changes **how often** transcription starts. Three kinds:

| Kind | How it works | Example |
|---|---|---|
| **Repressor** | blocks: sits on a site overlapping the promoter so polymerase can't bind | bacterial lac repressor |
| **Activator** | recruits: binds near the promoter and stabilizes polymerase binding | — |
| **Enhancer** (eukaryotes) | activator sites thousands of bp away; DNA **loops** so the bound activator reaches the promoter | — |

**Basic logic:** a gene's output depends on how often its regulatory sites are **occupied**.

---

## 3. The math: occupancy

A single site is a two-state system, **empty** or **bound** by factor T:

$$T + \text{site} \rightleftharpoons T\cdot\text{site}, \qquad K_d = \frac{[T][\text{site}]}{[T\cdot\text{site}]}$$

Fraction of time occupied:

$$\theta = \frac{[T]}{[T] + K_d} = \frac{1}{1 + K_d/[T]}$$

**Stat-mech view.** Empty has weight 1, bound has weight [T]/K_d. θ = bound weight ÷ partition function.

Three things to notice:
1. **Same curve as Michaelis–Menten.** Both rise and then saturate, for the same reason: a single saturable site.
2. **K_d is the concentration at half occupancy.** Put [T] = K_d: θ = K_d/2K_d = ½. Small K_d = tight binding.
3. **A single site is a soft dimmer, not a switch.** Going from 10% to 90% occupancy needs an **81-fold** rise in [T].

**Cooperativity sharpens it.** When several factors bind cooperatively (each bound one makes the next more likely), the curve becomes a **Hill function**:

$$\theta = \frac{[T]^n}{K^n + [T]^n}$$

- n = 1 is the ordinary single-site curve.
- Larger n gives a steeper, more switch-like curve.
- This is the seed of the bistable switches and cell-fate attractors in Theme 3.

```
θ  1 ┤                 ___________  n large (switch)
     │              __/        ____ n = 1 (dimmer)
 0.5 ┤ - - - - - - -+- - __----
     │          __-/ /‾‾
     │     __--‾   /
   0 ┼──‾‾‾───────┴─────────────── [T]
                  K
```

**Modeling caveats**
- **[research]** Assuming *transcription rate ∝ occupancy* is the **thermodynamic model**. It is widely used and often works, but it assumes binding at equilibrium. Real initiation has energy-consuming, non-equilibrium steps; where the assumption fails is actively studied.
- **[Ball]** Many transcription factors have intrinsically disordered regions and bind loosely and promiscuously, so "one factor, one site" is too tidy. Taken up in Theme 2.

---

## 4. Check: smaller K_d, lower or higher concentration?

**Question.** Factors A and B bind the same site; A has the **smaller** K_d. Which needs the higher concentration to keep the site half occupied, and why?

**My answer.** Couldn't answer. I knew "small K_d means tight binding" but didn't know where to go from there.

**Feedback.** That's the right fact, but the wrong one to start from. The one you need is that **K_d is itself the half-occupancy concentration**.

**Step 1.** A is at half occupancy. What is [A] equal to?
- *My answer:* K_d (A's own). ✓

**Step 2.** B reaches half occupancy at its own, larger K_d. Which needs the higher concentration?
- *My answer:* B. ✓

**Connecting the remembered fact:** $K_d = k_{\text{off}}/k_{\text{on}}$ (rate of falling off ÷ rate of landing). A tight binder has a small K_d mainly because it **falls off slowly**. Each molecule that lands stays a long time, so fewer molecules in solution keep the site covered. B keeps falling off, so it needs more.

**Fill-in-the-blank (my completed version)**

> Half occupancy happens when [T] equals **K_d**. A has a **smaller** K_d than B, so A reaches half occupancy at a **lower** concentration. That's because each A molecule stays bound **a long time**, so B needs the **higher** concentration.

**Wording fix.** The comparison is relative: each A molecule stays bound **longer** (than a B molecule), not just "a long time."

**A2 complete.**

---

## 5. Later the same day: recall on dimmers and switches

**Question.** Why does a single binding site act more like a dimmer than an on/off switch, and what makes the response sharper? (I asked for smaller steps.)

**Step 1.** As [T] rises, does θ jump at a threshold (a) or rise gradually (b)?
- *My answer:* b ✓

**Step 2.** So going from mostly off to mostly on takes a small (a) or large (b) change in [T]?
- *My answer:* b ✓ (10% → 90% needs an ~81-fold rise)

**Step 3.** With cooperative binding, is the curve steeper (a) or shallower (b)?
- *My answer:* a ✓ (Hill function, larger n)

**Fill-in-the-blank (my completed version)**

> A single site's occupancy rises **gradually** with concentration, so switching from mostly off to mostly on needs a **large** change in [T]. **Cooperative** binding makes the curve steeper (a Hill function with n **larger than** 1), so a much smaller change in [T] flips the gene.

**Feedback:** correct and complete.

---

## 6. Terms introduced (glossary v3)

activator · repressor · enhancer · regulatory transcription factor · dissociation constant (K_d) · occupancy (θ) · cooperative binding · Hill function · thermodynamic model · (from 11-06) template strand, coding strand, transcription bubble, sigma factor, general transcription factors, RNA polymerase II, TATA box

## 7. Recall prompt for next session

> Why does a single transcription-factor binding site act more like a dimmer than an on/off switch, and what makes the response sharper?

<details>
<summary>Target answer</summary>

Occupancy θ = [T]/([T] + K_d) rises gradually, so going from mostly off to mostly on needs a large (~81-fold) change in concentration. Cooperative binding gives a Hill function with n > 1, a steeper curve, so a much smaller change in [T] flips the gene.

</details>

## 8. Pattern notes

- A remembered fact ("small K_d = tight binding") doesn't automatically connect to a formula. Start from the defining property (K_d *is* the half-occupancy concentration).
- Direction words ("in the 3′ direction") are ambiguous when two antiparallel molecules are involved. Say which molecule.
- Saying "smaller steps" when stuck works well.

**Next up:** A3, RNA processing (splicing, introns and exons, alternative splicing).
