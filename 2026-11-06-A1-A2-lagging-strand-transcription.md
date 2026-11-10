# Session 2026-11-06 — A1 finish (lagging strand) and A2 start (transcription, promoters)

**Theme 0, Block A** · A1 (DNA structure and copying) → ☑ done · A2 (transcription), chunks 1–2 → ◐

Tags: **[consensus]** textbook view · **[research]** active, unsettled · **[Ball]** Ball's interpretive position

*Rebuilt from the chat on 2026-11-10.*

---

## 1. Recall: why is one new strand made in pieces?

**My first answer.** The lagging strand, growing away from the fork, must wait for a stretch of the original to be exposed, then copy backwards until it reaches the previous piece.

**Feedback.** "Growing away from the fork" is right. But *waiting for exposed template* is still given as the cause, and it isn't the cause: **both** strands wait for exposed template.

### Worked through with a diagram

```
                                           fork moves →
 top template      3' ──────────────────────╮
 new (leading)     5' ═══════════════► 3'    ╲______________ 5'
                                                             (still paired)
 new piece         ?  ════  ?                ╱‾‾‾‾‾‾‾‾‾‾‾‾‾‾ 3'
 bottom template   5' ──────────────────────╯
```

**Step 1.** The new piece on the bottom template pairs *antiparallel* with it. Which end is its 3′ end?
- *My answer:* the left end, away from the fork. ✓

**Step 2.** Polymerase adds only to a 3′ end. Which way can the piece grow?
- *My answer:* away from the fork. ✓
- *Clarification (my question was badly worded).* New template keeps appearing on the **right**, at the fork, but the piece's growing end is on the **left**. It can never extend into newly opened template. So each time the fork opens a stretch, a **fresh piece** (with a new primer) must start there. It grows leftward until it meets the previous piece, and ligase joins them.

**Fill-in-the-blank (my completed version)**

> Polymerase only adds to the **3′ end**, and the two templates are **antiparallel**, so on one of them the new strand's growing end points **away from** the fork. It can't extend into newly opened template, so it has to be **segmented**.

**Feedback.** The full causal chain, correct and in the right order. **A1 complete.**

**Method note.** Diagram first, then one-step checks, then a fill-in-the-blank: this is what cracked it. Say "draw it" or "smaller steps" any time.

---

## 2. A2 chunk 1: what transcription is [consensus]

RNA polymerase reads **one** strand of a gene's DNA and builds a complementary RNA. Same rule as DNA polymerase: it adds only to a 3′ end, so RNA grows 5′ → 3′.

**How it differs from replication**

| | Replication | Transcription |
|---|---|---|
| Opening | a fork; whole molecule unzipped | small **bubble**, ~12–14 bp, rezips behind |
| Strands read | both | **one** (the *template strand*) |
| Primer | needed | **none** — starts from nothing |
| Error rate | ~1 per 10⁹ | ~1 per 10⁴–10⁵ |

- **Template vs coding strand.** The RNA has the same sequence as the *other* strand (U for T), so that one is called the **coding strand**.
- **Why sloppiness is tolerable.** A transcript is a short-lived working copy, made many times. An error dies with that copy and isn't inherited.

```
                     RNA polymerase moves →
                        ___________
 coding   5' ──────────╯           ╰──────────── 3'
              [promoter]
 template 3' ──────────╮           ╭──────────── 5'
                        ‾‾‾‾‾‾‾‾‾‾‾
                     RNA 3' end ● (at the polymerase)
            5' ═══════════════╯   RNA peels off as a single strand
```

---

## 3. A2 chunk 2: promoters, first pass [consensus]

The polymerase must know **where to start** and **which way to go**.
- A **promoter** is a stretch of DNA just upstream of a gene, recognized and bound to set up the start.
- It is **asymmetric**, so it fixes the direction, and the direction decides which strand is the template.
- Neighboring genes can sit on opposite strands and run in opposite directions.

**Bacteria.** A detachable polymerase subunit, the **sigma factor**, recognizes two short motifs about 10 and 35 bases upstream of the start.

**Eukaryotes.** **RNA polymerase II** can't recognize a promoter alone. **General transcription factors** assemble there first (some promoters have a **TATA box** as a landing pad) and recruit the polymerase.

**Why this matters.** If polymerase depends on other proteins to get onto DNA, then which genes run is decided by which proteins are present and bound. That is where regulation lives (chunk 3), and the first step toward Ball's quarrel with the "genetic program" [Ball].

---

## 4. Check: why does transcription have no lagging-strand problem?

**My answer.** It only opens one strand.

**Feedback.** Right idea, wrong word, and the word matters. Transcription **opens** both strands (that's the bubble) but **reads** only one.

**Full causal version.** In replication, both strands must be copied while the fork moves one way, so one is always pointed wrong. In transcription, the promoter picks the strand oriented so the RNA's growing 3′ end faces the direction of travel. The other strand is ignored, so every transcript is effectively a leading strand.

**One-step check.** If the polymerase kept moving right but used the *top* strand as template, would the RNA's 3′ end face the direction of travel or away from it?
- *My answer:* away. ✓
- *Feedback:* the top strand runs 5′→3′ left to right, so the RNA's 3′ end would be on the left: the lagging-strand problem. That is why the promoter's direction effectively chooses the template.

---

## 5. Terms introduced

template strand · coding strand · transcription bubble · promoter · sigma factor · general transcription factors · RNA polymerase II · TATA box *(added to the glossary in v3)*

## 6. Recall prompt for next session

> Transcription opens both DNA strands. Why is there no lagging-strand problem?

<details>
<summary>Target answer</summary>

Only one strand is read. The promoter sets the direction, so the template is the strand whose RNA grows with its 3′ end facing the polymerase's travel; the other strand is ignored. Watch the word: it *opens* both strands and *reads* one.

</details>

## 7. Pattern notes

- Spatial "why" questions land after a diagram plus one-step checks, not as open prose prompts.
- Word precision: "opens" vs "reads." The mechanism was right; the verb was wrong.

**Next up:** A2 chunk 3, transcription factors and binding occupancy.
