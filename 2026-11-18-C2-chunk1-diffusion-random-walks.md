# Session notes — Recalls + C2 chunk 1: Diffusion and random walks

**Dates:** 2026-11-18 to 11-19 · **Theme 0, Block C** · **Unit status after session:** C2 ◐ (chunk 1 done)

***

## Recall 1 (C1): why a stable protein responds in about one cell cycle

_Prompt:_ A bacterium switches on production of a stable protein (never degraded). Why does its concentration take about one cell cycle to approach its new level, however fast production switches on? Shape: "no degradation → only \_\_\_ removes it → so \_\_\_ sets the response time."

* Fog: "no degradation → only dilution removes it → so cell division sets the response time." **✓**

* Refinement: the precise last link is the **growth rate** (doubling time), not division as an event. For concentration, dilution comes from volume growth. At division both copy number and volume halve, so concentration doesn't jump.

  * Copies per cell: drop in steps at each division.
  * Concentration: falls smoothly as the cell grows, α_dil = ln 2 / T_div (α_dil = dilution rate, T_div = doubling time, ln 2 ≈ 0.69).

***

## Recall 2 (Block A quiz, Q1): antiparallel strands → Okazaki fragments

_Prompt:_ Walk the chain from "the two strands are antiparallel" to "one new strand is made in Okazaki fragments." Shape: four links, A → B → C → D.

* Fog's first answer: "at the replication fork, one template strand's 3′ end faces _away_ from the fork → polymerase on that strand can't follow the fork continuously, so it builds short pieces backward."

* Two problems:

  1. **Wrong molecule.** What points away from the fork is the 3′ end of the _new_ strand. On the lagging side, the template's 3′ end points _toward_ the fork. (Same antiparallel-direction trap as A1.)
  2. **Missing link:** the polymerase rule, i.e. why the 3′ direction matters.

* **Note (found while writing these notes):** the Block A quiz's own answer key for Q1 had the same wrong-molecule wording. Fog's first answer may have echoed it. The key is now corrected.

Diagram used (fork moves right; the parent helix is still intact on the right; arrowheads show growth direction):

```
                                              fork moves →
                                                   │
 top template     5′ ───────────────────────────── ╲  ═════════
 new pieces          3′ ◄─────── 5′   3′ ◄──── 5′   ╲  parent
                                                     >  helix
 new strand          5′ ──────────────────────► 3′  ╱  (not yet
 bottom template  3′ ───────────────────────────── ╱   unwound)
                                                   │
```

* One-step checks: (a) the polymerase adds only to the new strand's \_\_\_ end → **"3′"** ✓. (b) On the top template, the new strand's growing 3′ end points toward or away from the fork? → **"away"** ✓
* Fill-in: "The strands are antiparallel → polymerase can only add to the new strand's 3′ end → so on one template, the new strand's growing end points away from the fork → so it can't follow the fork and is made in short pieces, later joined together." **✓ complete.** The joining enzyme is DNA ligase.
* Progress: links C and D came unprompted; B (the rule) and the choice of molecule needed prompting.

***

## C2 chunk 1: Why diffusion works over short distances and fails over long ones

### Unit key

nm = nanometer (10⁻⁹ meter) · µm = micrometer (10⁻⁶ meter) · µm²/s = square micrometers per second (unit of D) · s = second · ps = picosecond (10⁻¹² second) · m/s = meters per second

### 1. Why molecules random-walk \[consensus]

A protein in cytoplasm is hit by water molecules \~10¹³ times per second. Between hits it moves at \~10 meters per second (thermal speed), but it loses its direction after \~1 picosecond, having moved only \~0.01 nanometers. On any longer timescale its path is a sequence of short, uncorrelated steps: a **random walk** (the motion itself is called **Brownian motion**).

### 2. The math: why distance grows as √t \[consensus]

One-dimensional walk, step +a or −a with equal probability, one step every time τ (tau):

x_N = s₁ + s₂ + … + s_N, with ⟨sᵢ⟩ = 0

⟨x_N²⟩ = Σᵢ Σⱼ ⟨sᵢ sⱼ⟩ = N a²

Cross terms (i ≠ j) average to zero because the steps are independent: they partly cancel. Only the N diagonal terms survive. With N = t/τ:

**⟨x²⟩ = 2Dt**, where **D = a²/(2τ)** is the **diffusion coefficient**.

* 3D: axes independent → ⟨r²⟩ = 6Dt.
* Typical distance √⟨r²⟩ grows as **√t**, not t.
* Inverted: **time to cover distance L ≈ L²/(6D)**. Twice the distance → four times the time.
* The spread of positions becomes Gaussian with variance 2Dt (central limit theorem). This is the diffusion equation's solution, in chunk 2.

_Interactive shown in the session:_ 500 one-dimensional walkers; measured root-mean-square distance tracks √N (100 steps → \~10 units; 400 steps → \~20).

### 3. How big D is

**Stokes–Einstein relation:** D = k_B T / (6π η r). Here k_B = Boltzmann's constant, T = temperature, η (eta) = viscosity, r = radius. Bigger molecule or thicker liquid → smaller D. \[consensus]

| Molecule, where                                                 | D (square micrometers per second) |
| --------------------------------------------------------------- | --------------------------------- |
| Small molecule (glucose), in water                              | \~600                             |
| GFP (green fluorescent protein, typical protein size), in water | \~90                              |
| GFP in human-cell cytoplasm                                     | \~25                              |
| GFP in E. coli cytoplasm                                        | \~7 (Elowitz et al. 1999)         |

Values from Milo & Phillips \[consensus, order of magnitude]. Why cytoplasm slows proteins 4–13× is the subject of C3, crowding \[research].

### 4. Consequences, using t ≈ L²/(6D)

* Protein across E. coli (1 micrometer, D ≈ 7): **\~0.02 seconds**.
* Protein across a human cell (20 micrometers, D ≈ 25): **\~3 seconds**. This corrects the C1 preview (\~20 seconds), which used the bacterial D. The 400× scaling from 20× the distance was right.
* Protein down a 1-meter nerve axon (D ≈ 25): \~10¹⁰ seconds ≈ **200 years**.
* **Motor proteins** walk along cytoskeletal tracks at \~1 micrometer per second: the 1-meter trip takes \~10 days \[consensus]. (Motors and tracks come up in C5.)

**Crossover argument** (a rough argument of my own, not a standard textbook result): diffusion's effective speed over distance L is L/t ≈ 6D/L, which rises as L shrinks; a motor's speed v is fixed. They break even at L\* ≈ 6D/v, about 100 micrometers for a protein. Below L\*, diffusion wins; above it, directed transport wins. This is consistent with bacteria relying almost entirely on diffusion while large eukaryotic cells also use motors.

### Check

_Question:_ Why does diffusion move proteins across a bacterium in a fraction of a second but would take centuries down a 1-meter axon? Shape: "diffusion time grows as the \_\_\_ of the distance → so \_\_\_."

* Fog: "diffusion time grows as the square of the distance → so the bacterium is roughly 1 micrometer compared to the 1 meter axon." First link **✓**; the second link stated the distances but not what the square rule does to them.
* One-step: a million times the distance → time a million times longer, or much more? → **"much more than a million"** ✓
* Shown: (10⁶)² = 10¹², a trillion. 0.02 seconds × 10¹² ≈ 10¹⁰ seconds, centuries. The different D values in the two cytoplasms (7 vs. 25) change this by only a factor of a few.
* Fill-in (next morning): "…so a million-times-longer distance takes a **million**-times-longer time…" **✗ on the key blank.** This is the linear answer, which contradicts the previous step. Correct: **trillion** (10¹²).
* Counted as passed with correction. The squaring step goes into the next recall.

***

## Terms introduced (glossary additions pending, to be added when C2 is complete)

Brownian motion · random walk · mean-square displacement ⟨x²⟩ · diffusion coefficient D · Stokes–Einstein relation · viscosity η · GFP (green fluorescent protein) · diffusion time t ≈ L²/(6D) · axon · motor protein · crossover length L\* ≈ 6D/v

***

## Next recall prompts

**Recall 1 (C2 chunk 1, the squaring step).** A protein takes about 0.02 seconds to diffuse across a 1-micrometer bacterium. A distance 1,000 times longer: does it take about 1,000 times longer, or about 1,000,000 times longer? _Answer shape:_ pick one, then one clause naming the rule that decides it.

\<details> \<summary>Answer\</summary>

About 1,000,000 times longer, because diffusion time grows as the square of the distance: (1,000)² = 1,000,000. (For reference, 1,000 micrometers = 1 millimeter, about 20,000 seconds ≈ 6 hours.)

\</details>

**Recall 2 (Block A quiz, Q4: K_d and rates).** Transcription factor X has a tenfold lower K_d (dissociation constant: the concentration at which its site is half-occupied) than factor Y. _Answer shape:_ two parts. (a) Which rate mostly differs: binding (k_on) or unbinding (k_off)? Which factor's is slower? (b) Is X's occupancy curve shifted left or right of Y's when plotted against concentration?

\<details> \<summary>Answer\</summary>

(a) Usually k_off. K_d = k_off / k_on, and k_on values are often near the limit set by diffusion, so they vary less; tighter binders mostly differ by falling off more slowly. X's k_off is slower. (b) Shifted left: X reaches half-occupancy at one-tenth the concentration. (Chunk 2's diffusion-limited rate makes the k_on point concrete.)

\</details>

**Next unit:** C2 chunk 2. Diffusion equation and Fick's law; diffusion-limited reaction rates; lac repressor's facilitated search (sliding along DNA) \[research].
