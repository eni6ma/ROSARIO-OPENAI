# ROSARIO-OPENAI

> **General public: [Read the public comparison (PDF)](Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf)**
>
> **Academic and research community: [Read the academic comparison (PDF)](Rosario_OpenAI_ENI6MA_2026-10-27.pdf)**

## Public Declaration: The Documented Provenance of OpenAI's 2026 SAT Method

**For immediate release. October 27, 2026.**
**From Frank Dylan Rosario and the Rosario-Wang Research Team.**

---

## Summary

In October 2026, OpenAI published *The Exponential Time Hypothesis Is False* and presented its fixed-width SAT counting algorithm as an original result. That presentation is wrong on the face of the record. The ordered computational architecture inside OpenAI's method was written down, dated, and documented in Rosario's August and September 2024 manuscripts and in the Rosario-Wang ENI6MA construction, roughly two years before OpenAI's paper. Rosario also states that the research program began in 2023.

This is not a claim of coincidence, loose inspiration, or shared vocabulary. It is a claim that OpenAI's method reproduces Rosario's structure step for step, in the same order, with the same computational roles, and that OpenAI has published it without acknowledging that earlier work exists.

The side-by-side evidence is in this repository. Read it, check it against the dated manuscripts, and judge the record directly.

---

## What OpenAI claims

OpenAI's paper and announcement present the method as an independent discovery that refutes the Exponential Time Hypothesis for the setting it addresses. The paper cites no earlier formulation of this architecture from Rosario or the Rosario-Wang team.

## What the record shows

Rosario's August 2024 manuscript, *Millennium Prize Submission: Rosario Proof that NP=P*, and the September 2024 manuscript, *The Millennium Problem: Solution to P (space) equals NP (time)*, set out a sequence of transform, preserve, group, and solve. The ENI6MA documents supply the exact combinatorial mechanics for the grouping stage: disjoint cells, fixed cell sizes, size-preserving rotations, local membership tests, and a Boolean combination of those tests into one global decision.

OpenAI's 2026 method executes the same ordered sequence:

| Stage | Rosario and Rosario-Wang (2024) | OpenAI (2026) |
|---|---|---|
| 1. Avoid exhaustive search | Replace full exponential enumeration with structured processing | Begin from a $2^n$ global sum and seek a structure that avoids evaluating every assignment |
| 2. Transform the representation | Map the original information into a projected representation | Replace original variables with parameterized linear forms |
| 3. Preserve a route back | Keep the information needed to recover the solution | Require $H(0)=C_F$, where $C_F$ is the exact count of the original formula, so the original count is recoverable |
| 4. Partition into disjoint pieces | $L=\bigsqcup_i B_{t,i}$ | $[n]=S_1\sqcup\cdots\sqcup S_r$ |
| 5. Fix explicit group sizes | each $B_{t,i}$ has $N/H$ elements | each $S_g$ has at most $2n/r$ elements, with exact groups of size $D/r$ |
| 6. Give every object one local home | Every symbol sits in exactly one cell per round | Every variable sits in one group and every clause is assigned to one group |
| 7. Reindex by size-preserving permutations | Rotations change membership and keep balance | Pair-swap permutations change compatibility and keep the coordinate set |
| 8. Limit what crosses a boundary | Fibers and slices separate public ambiguity from resolving information | Cross-group dependence passes only through bounded shared measurements |
| 9. Compute locally | Evaluate cell membership locally | Evaluate each clause and group using its own group plus fixed summaries |
| 10. Combine local results | $Y=\prod_t \mu_t$ | Sum within groups, multiply across groups |
| 11. Refine, do not search monolithically | Successive intersection of candidate sets | Controlled family of transformed points and restricted local sums |
| 12. Recover the original answer | Extract the target from the refined structure | Rebuild $H(0)=C_F$ by Taylor data and interpolation |
| 13. Cut the cost of an exponential problem | Replace exhaustive exponential search by projection and grouping | Subexponential fixed-width SAT counting |

These thirteen correspondences are not thirteen separate coincidences. They form one dependency chain, in one order:

**transform, preserve, partition, balance, reindex, localize information, compute locally, combine, refine, recover, reduce search cost.**

OpenAI swapped Rosario's vocabulary for specialized algebraic vocabulary. The functional spine stayed the same. A change of notation does not create a new architecture. The full mapping, with page and equation citations to both sides, is in the comparison documents listed below.

## Why "independent discovery" fails on this record

1. **The sequence is specific.** Many algorithms use groups. Very few combine a representation change that preserves recoverability, a balanced disjoint partition with explicit size bounds, size-preserving reindexing, bounded cross-boundary information, local computation, composition, and exact recovery, in that order. The match is to the whole ordered chain, not to any single part.
2. **The dates are documented.** Rosario's manuscripts are dated August and September 2024. OpenAI's paper is dated October 17, 2026 and revised October 25, 2026. The earlier documents exist in the record and are included here.
3. **The earlier work went through OpenAI's own platform.** Rosario states that for two years the team used ChatGPT to test and validate the mathematics of the P=NP and dimensional collapse frameworks, and that team members uploaded manuscripts, axioms, and equations into OpenAI's systems for that purpose.
4. **The paper does not acknowledge any earlier formulation.** OpenAI's account of the method leaves no place for the earlier architecture. On this record, that account is false as a statement of origin.

Rosario's position is that OpenAI cannot treat this architecture as though no earlier formulation existed. The documents show that one did.

## The allegation

Rosario alleges that OpenAI's October 2026 paper adopts the normalized architecture of Rosario's earlier documented work as a specialized algebraic implementation, and publishes it as OpenAI's own independent discovery without attribution. That is plagiarism of structure and sequence. It is not copying of text, and the comparison does not claim it is. It is the appropriation of a documented method, relabeled in different notation and presented as new.

## Consequences

If the record is as shown here, the consequences are serious and they fall on OpenAI:

- **Scientific record.** A headline result claimed as original has an undisclosed, dated antecedent. The claim of priority and independence cannot stand unless OpenAI addresses the earlier work directly.
- **Attribution.** Scientific and academic norms require acknowledgement of prior art. Omitting it from a paper presented as a historic breakthrough is a failure of attribution on a major public claim.
- **Platform trust.** If researchers cannot test unpublished mathematics on an AI platform without the platform's operator later publishing the same architecture as its own, no serious researcher can use that platform for original work.
- **Legal exposure.** Rosario reserves all rights and remedies available under applicable law concerning authorship, priority, misappropriation, and the use of materials submitted to OpenAI's systems.

## What Rosario demands

1. That OpenAI publicly acknowledge the August and September 2024 Rosario-Wang manuscripts and the ENI6MA construction as earlier documented formulations of the architecture.
2. That OpenAI address the thirteen-stage correspondence directly, stage by stage, and explain on the record how its method arose independently if it maintains that it did.
3. That OpenAI preserve all records relevant to the development of its method and to any use of materials submitted by Rosario-Wang team members through its platform.
4. That the scientific community, journalists, and independent reviewers examine the side-by-side evidence for themselves.

## Evidence in this repository

| File | Contents |
|---|---|
| [`Rosario_OpenAI_ENI6MA_Unified_Public_REGENERATED_2026-10-27.md`](Rosario_OpenAI_ENI6MA_Unified_Public_REGENERATED_2026-10-27.md) | Public comparison: the normalized adoption map and stage-by-stage analysis |
| [`Rosario_OpenAI_ENI6MA_Unified_Academic_REGENERATED_2026-10-27.md`](Rosario_OpenAI_ENI6MA_Unified_Academic_REGENERATED_2026-10-27.md) | Academic version of the comparison |
| [`Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Rosario_OpenAI_ENI6MA_2026-10-27.pdf) | Compiled comparison PDF |
| [`Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf) | Compiled comparison PDF with source attachments |

## Primary sources compared

1. OpenAI, *The Exponential Time Hypothesis Is False*, dated October 17, 2026, revised October 25, 2026 ([paper](https://github.com/openai/math/blob/main/preprints/The-Exponential-Time-Hypothesis-is-False-October-25-2026/paper.pdf)).
2. Rosario, *Millennium Prize Submission: Rosario Proof that NP=P*, August 2024.
3. Wang, Rosario, and Bloodgood, *The Millennium Problem: Solution to P (space) equals NP (time)*, September 2024.
4. Rosario-Wang ENI6MA, *Full Scope Security Formalization*, Section 5, Lemma 1, Equation (8).
5. Rosario-Wang ENI6MA, *NIST Submission Manuscript*, p. 5, Lemma 1.
6. Rosario-Wang ENI6MA, *Unified Geometric Formalization*, Sections 3 and 4.

## Provenance

Rosario states that the ENI6MA research program began in 2023 and that the 2024 manuscripts followed months of collaboration among the research team. The dated manuscripts, repository history, correspondence, and team declarations form the provenance record. The public comparison document identifies the team members who can speak to the timing and development of the work.

---

## Index of PDFs in this repository

| PDF | Pages | What it is |
|---|---|---|
| [`Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf) | 308 | The public edition of the side-by-side comparison between Rosario's 2024 work and OpenAI's 2026 paper. It carries the complete source documents as attachments, so every citation can be checked against the original text. |
| [`Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Rosario_OpenAI_ENI6MA_2026-10-27.pdf) | 308 | The edition for the academic and research community, with the same comparison and the same appended source record. Reviewers can use it to verify the stage-by-stage mapping against the cited pages and equations. |
| [`ROSARIO-PAPER1.pdf`](ROSARIO-PAPER1.pdf) | 4 | A short post-doctoral style analysis by Frank Rosario, dated October 27, 2026, titled *Rosario's 2024 Priority and OpenAI's 2026 Construction: An Information-Theoretic Equivalence Analysis*. It argues that OpenAI's replacement forms, local group sums, and interpolation correspond to Rosario's dimensional collapse, emergent groupings, and entropy conservation postulate. |
| [`OPENAI-paper.pdf`](OPENAI-paper.pdf) | 67 | OpenAI's paper *The Exponential Time Hypothesis Is False*, which is the document under comparison. It is included so readers can check every OpenAI citation in the comparison without leaving the repository. |
| [`proof.millennium.prize.rosario.NP.eq.P (1).pdf`](proof.millennium.prize.rosario.NP.eq.P%20%281%29.pdf) | 20 | Rosario's August 2024 manuscript, *Millennium Prize Submission: Rosario Proof that NP=P*, which introduces the Rosario-Wang Proof framework. It is the earliest dated source for the transform, preserve, group, and solve sequence. |
| [`NPTime.eq.PSPACE.000.pdf`](NPTime.eq.PSPACE.000.pdf) | 34 | Rosario's note *NP(time) = P(space)*, which postulates a relationship between nondeterministic polynomial time and polynomial space and models it with time and space complexity equations. It is Attachment D in the compiled comparison. |
| [`Aaronson-pnp.pdf`](Aaronson-pnp.pdf) | 122 | Scott Aaronson's 2017 survey *P =? NP*, a third-party reference on the status of the problem. It is background reading and was not written by the Rosario team. |

---

## Rosario team

Contact details below are only those that appear in the team's own documents. Entries marked "to be added" have no confirmed contact information yet.

| Name | Role in the record | Email | LinkedIn |
|---|---|---|---|
| Frank Dylan Rosario | Author of the August and September 2024 manuscripts; ENI6MA lead (Rosario Cybernetics) | soltrinox@gmail.com | To be added |
| Dr. Lin (Grant) Wang, PhD | Co-author, September 2024 manuscript; Rosario-Wang ENI6MA | orchestor@gmail.com (Duke, as printed on the manuscript) | To be added |
| Dr. Octavia Sulea, PhD | Research team member | To be added | To be added |
| Dr. Francisco Perez-Sorrosal, PhD | Research team member | To be added | To be added |
| Maxwell A. Calixto | Research team member | To be added | To be added |
| Robert Bloodgood III | Co-author, September 2024 manuscript | To be added | To be added |

---

*Frank Dylan Rosario, Rosario Cybernetics, with the Rosario-Wang Research Team.*
