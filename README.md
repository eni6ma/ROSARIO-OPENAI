# ROSARIO-OPENAI

> **General public: [Read the public comparison (PDF)](Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf)**
>
> **Academic and research community: [Read the academic comparison (PDF)](Rosario_OpenAI_ENI6MA_2026-10-27.pdf)**

## Contents

- [Index of PDF files](#index-of-pdf-files) (every PDF in this repository, with page counts and what each one is)
- [Index of Markdown files](#index-of-markdown-files)
- [Equation verification guide](#equation-verification-guide) (each key equation, side by side, with the page where you can check it)
- [Where to find each source inside the 308-page compiled PDFs](#where-to-find-each-source-inside-the-308-page-compiled-pdfs)
- [Primary sources compared](#primary-sources-compared)
- [Provenance](#provenance)
- [Rosario team](#rosario-team)

## Public Declaration: The Documented Provenance of OpenAI's 2026 SAT Method

**For immediate release. October 27, 2026.**
**From Frank Dylan Rosario and the Rosario-Wang Research Team.**

---

## Summary

In October 2026, OpenAI published *The Exponential Time Hypothesis Is False* and presented its fixed-width SAT counting algorithm as an original result. That presentation is wrong on the face of the record. The ordered computational architecture inside OpenAI's method was written down, dated, and documented in Rosario's August and September 2024 manuscripts and in the Rosario-Wang ENI6MA construction, roughly two years before OpenAI's paper. Rosario also states that the research program began in 2023.

This is not a claim of coincidence, loose inspiration, or shared vocabulary. It is a claim that OpenAI's method reproduces Rosario's structure step for step, in the same order, with the same computational roles, and that OpenAI has published it without acknowledging that earlier work exists.

The side-by-side evidence is in this repository. Read it, check it against the dated manuscripts, and judge the record directly.

OpenAI's substitutions within Rosario's sequence

OpenAI's later paper reproduces Rosario's ordered functional blueprint through specialized algebraic machinery. Rosario's dimensional collapse becomes low-degree replacement linear forms. Rosario's cells and emergent groupings become an $(r,\tau,D)$-design. Rosario's information-retention requirement becomes $H(0)=C_F$ together with bounded shared measurements. Rosario's rotations and alphabet transformations map onto pair labels and swap matrices. Rosario's extraction objective maps onto exact interpolation from Taylor data.

These substitutions preserve the same sequence from beginning to end. The later method follows Rosario's route to computational advantage: transform the representation, preserve the original task, partition the transformed state, preserve group-size structure while reindexing, localize external information, compute within local pieces, combine the contributions, and reconstruct the original answer. OpenAI's fixed-width SAT result is therefore a specialized algebraic implementation of the Rosario blueprint.

The computational objective remains the reduction of exhaustive global work. Rosario's 2024 program targets polynomial time and $P=NP$. OpenAI's 2026 implementation reaches a subexponential fixed-width SAT counting bound through the same normalized architecture.

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

# The Rosario Sequence and OpenAI’s 2026 SAT Construction: A Beginning-to-End Structural Map

**Author:** Mr. Frank Dylan Rosario  
**Date:** October 27, 2026

The central comparison between Mr. Frank Dylan Rosario’s earlier computational work and OpenAI’s 2026 SAT construction becomes strongest when the two systems are normalized into their functional operations rather than compared by terminology. Rosario’s August and September 2024 manuscripts describe a computational strategy in which an exponentially difficult global problem is moved into a different representation, the relationships necessary for solving the original problem are preserved, the reorganized state is divided into useful groups, those groups become the operative units of computation, and the result is extracted from the reorganized representation. The later Rosario-Wang ENI6MA construction makes those operations concrete through balanced disjoint partitions, controlled group sizes, rotations that change membership while preserving cardinality, membership signatures, successive intersection of candidate sets, fibers and private slices, Boolean composition of local membership decisions, and final target extraction. OpenAI’s 2026 paper then follows the same normalized sequence through a specialized algebraic implementation: replacement linear forms, disjoint bounded groups, exact balanced auxiliary fibers, designated clause groups, pair-swapping permutations, bounded shared measurements, local group calculations, sum-product composition, and interpolation back to the original SAT count. The comparison therefore runs continuously from the original problem representation to the final recovered answer.

Rosario’s first important move was to treat computational difficulty as a problem of representation. His 2024 construction proposes moving a difficult problem from its original high-dimensional form into another representation in which useful relationships can become available for computation. The August manuscript writes this in terms of higher-dimensional information $I_H$, projected information $I_L$, and a projection $I_L=P(I_H)$. It describes the transformation as a reorganization that retains critical information while reducing redundant complexity. The September manuscript then gives the order explicitly: project the problem while preserving critical relationships, organize the projected information into groups, and use the resulting organization to obtain the solution. OpenAI’s 2026 construction begins in precisely the corresponding place. It starts with a $2^n$-assignment SAT calculation whose direct evaluation constitutes exhaustive enumeration, then changes the representation of the clause inputs through parameterized replacement forms so that a different organization of the calculation becomes possible. At $T=0$, the transformed family restores the original count through $H(0)=F$. Thus, both architectures begin by escaping the original global search representation and constructing another representation that preserves the original task.

The search objective itself is part of this correspondence. Rosario was not merely proposing “a faster search” in the abstract. His construction attempts to make a large state space navigable through a structured geometric representation. A target symbol acquires a membership label according to which region or cell of the manifold contains it. Across successive rounds, those local memberships form a signature. Each new observation or membership decision refines the remaining candidate set, and the final intersection identifies the intended target. This is a structured search through geometry rather than exhaustive traversal of every candidate state. The ENI6MA formalization expresses the process through partitions, fibers, slices, and successive intersections. OpenAI likewise replaces a monolithic search through all Boolean assignments with a transformed representation in which bounded local groups can be evaluated using controlled information and later recombined. The common computational idea is therefore more specific than “reduce exhaustive search”: both systems reduce global combinatorial traversal by reorganizing the state into locally searchable regions whose information progressively determines the required global answer.

The partition stage makes the structural map particularly concrete. Rosario-Wang ENI6MA divides a finite alphabet into a complete disjoint collection of cells. Every symbol belongs to exactly one cell during a particular frame, the cells cover the entire alphabet, and their sizes are controlled. In the balanced case the construction has the form

$$
\mathcal L=\bigsqcup_{i=0}^{H-1}B_{t,i},
\qquad
|B_{t,i}|=\frac{N}{H}.
$$

The construction also supports near-equal slicing when exact divisibility is unavailable. Rotation changes which symbols occupy which cells while preserving the size constraints. OpenAI’s construction later imposes

$$
[n]=S_1\sqcup\cdots\sqcup S_r,
\qquad
|S_g|\leq \frac{2n}{r},
$$

and its auxiliary coordinate construction produces exactly balanced fibers of size $D/r$. It also assigns every clause to one designated group. The normalized operation is the same: maintain a fixed global state, divide it into mutually exclusive bounded local pieces, give each relevant object a local home, and use those pieces as the units through which the next stage of the computation operates.

The correspondence continues through the rearrangement mechanism. Rosario’s rotating alphabets change the membership relation between symbols and cells while preserving the cardinality of the cells. This permits the system to expose a new pattern of relationships without changing the size of the state or violating the partition guarantee. OpenAI’s auxiliary construction uses commuting permutation matrices that swap entries of paired labels. Those swaps likewise preserve the coordinate population while changing which relationships are compatible with the local group structure at a given evaluation point. In both cases the computational state is reindexed through cardinality-preserving transformations so that different local relationships become visible while the partition structure remains controlled.

The information-flow stage also aligns. Rosario’s earlier framework requires the transformed representation to preserve the information required for the task, and ENI6MA realizes that principle through local membership information, fibers, slices, and successive resolving data. A local cell label is sufficient to answer the membership question assigned to that stage, while successive labels refine the answer further. OpenAI expresses the corresponding principle algebraically. A transformed clause assigned to one group may depend directly on that group’s variables, while information from another group must arrive through bounded measurements $y_h=C_hx_h$. Once those summaries are fixed, the clause becomes locally evaluable. Both systems therefore reduce the quantity of global information required at each local operation. The common rule is: preserve exactly the information necessary for the local predicate or contribution, then let that restricted information carry the computation forward.

The composition stage follows the same architecture. Rosario-Wang treats each relevant local membership as a Boolean predicate. If $\mu_t\in0,1$ records whether a required membership relation holds, the complete relation can be written as

$$
Y=\prod_t \mu_t.
$$

For Boolean indicators, multiplication implements logical conjunction: the complete result succeeds when the required local conditions succeed. OpenAI’s original SAT representation likewise uses clause-satisfaction indicators whose product represents simultaneous satisfaction of the complete formula. Its transformed computation then extends the same local-to-global principle by summing contributions within groups, multiplying group sums, and accumulating the resulting global value. The objects being tested differ, but the computational sequence remains aligned: evaluate local predicates or contributions, combine them according to the global rule, and use the combined result as the input to the final recovery stage.

Both constructions then return from the reorganized representation to the original target. Rosario’s 2024 sequence culminates in solution extraction from the projected and grouped problem space. In ENI6MA, repeated partition queries and intersections identify the target state. OpenAI collects the information generated at selected transformed evaluation points and reconstructs the original quantity $H(0)=F$ using Taylor coefficients and interpolation. Thus the transformed representation is intermediate in both systems. The architecture begins with an original difficult problem, moves into a representation that makes localized processing possible, and ends by recovering the answer defined by the original problem.

The entire comparison therefore forms one dependency chain rather than thirteen isolated similarities. The representation transformation exists so partitioning becomes useful. The partition exists so computation can become local. The cardinality guarantees maintain control over those local pieces. The permutations expose different local relationships while preserving the structure. The information restrictions make those pieces computationally manageable. The local results are combined. The combined information is then used to recover the original answer. Finally, the total process is analyzed for a reduction in computational work. Rosario’s stated objective was a polynomial-time route through projection and grouping; OpenAI’s 2026 paper claims a subexponential exact-counting result for fixed-width SAT. The complexity claims have different quantitative endpoints, but they occupy the same final position in the architecture: demonstrate that the transformed and partitioned route reduces the cost of the original global search.

The chronology makes the structural correspondence consequential. Rosario’s supplied August 2024 manuscript and the September 2024 Rosario-Wang manuscript precede OpenAI’s October 2026 paper. The normalized sequence is already present in Rosario’s earlier record. The comparison therefore supports the affirmative conclusion that the architectural blueprint predates the OpenAI result: representation change, preservation, partitioning, bounded cardinality, permutation-based reindexing, controlled cross-group information, local processing, local-to-global composition, refinement, recovery, and reduction of exhaustive search all appear in Rosario’s earlier research program and reappear in corresponding functional positions in OpenAI’s 2026 construction.

## The Sequence Created by Rosario and Adopted in OpenAI’s 2026 Construction

1. **Replace exhaustive traversal with structured navigation of the problem space.** Rosario reorganizes a large geometric or informational state so a person or algorithm can navigate locally through meaningful regions instead of enumerating the entire state. OpenAI begins from a $2^n$ Boolean search space and replaces global enumeration with a transformed local-group computation.
2. **Transform the representation before solving the problem.** Rosario projects $I_H$ into $I_L=P(I_H)$. OpenAI replaces original variable occurrences with parameterized linear forms. In both, the computational solution begins in a new representation rather than the original one.
3. **Preserve the information required to return to the original task.** Rosario requires retention of critical relationships and solution-relevant information through the transformation. OpenAI preserves the exact SAT target through $H(0)=F$.
4. **Partition the transformed state into disjoint local regions.** Rosario-Wang ENI6MA uses

$$
\mathcal L=\bigsqcup_i B_{t,i}.
$$

OpenAI uses

$$
[n]=S_1\sqcup\cdots\sqcup S_r
$$

and an analogous disjoint decomposition of its auxiliary coordinate set.

5. **Impose explicit group-size guarantees.** Rosario’s balanced construction gives

$$
|B_{t,i}|=\frac{N}{H},
$$

with near-equal bounds in the general slicing case. OpenAI bounds actual variable groups by

$$
|S_g|\leq \frac{2n}{r}
$$

and constructs auxiliary fibers of exact size

$$
\frac{D}{r}.
$$

6. **Give each relevant object a unique local home.** Every ENI6MA symbol occupies one cell per frame. OpenAI places each variable in one group and assigns each clause to one designated group.
7. **Reindex the state through cardinality-preserving transformations.** Rosario rotates alphabets so symbol-to-cell membership changes while balance is preserved. OpenAI uses pair-swap permutation matrices so compatibility relations change while the auxiliary coordinate population is preserved.
8. **Restrict what information crosses partition boundaries.** Rosario uses projected information, fibers, slices, and membership signatures so local computation proceeds from the information required at that stage. OpenAI requires cross-group dependence to pass through bounded shared measurements

$$
y_h=C_hx_h.
$$

9. **Perform the substantive computation locally.** Rosario evaluates cell membership and progressively refines the candidate state from local geometric information. OpenAI evaluates each transformed clause and group contribution using its assigned group plus fixed shared summaries.
10. **Combine local results into a global result.** Rosario-Wang combines membership indicators through

$$
Y=\prod_t \mu_t,
\qquad
\mu_t\in\{0,1\}.
$$

OpenAI sums local assignments within groups, multiplies group contributions, and accumulates the transformed global value.

11. **Use successive refinement instead of one monolithic search.** Rosario’s geometry narrows a candidate state through successive intersections,

$$
C_0\supseteq C_1\supseteq\cdots\supseteq C_T.
$$

OpenAI replaces one global enumeration with a controlled family of transformed evaluations and restricted local sums.

12. **Recover the original answer from the reorganized representation.** Rosario extracts the target from the projected, partitioned, and refined structure. OpenAI reconstructs the original count by recovering

$$
H(0)=C_F
$$

Here $C_F$ is the exact number of satisfying assignments of the original formula, which OpenAI writes with a hash sign.

from transformed evaluations through Taylor information and interpolation.

13. **Use the entire reorganization to reduce the cost of exponential search.** Rosario’s stated objective is to replace exhaustive traversal of a large geometric or computational state with efficient navigation through a projected and grouped representation. OpenAI uses the corresponding architecture to obtain a subexponential fixed-width SAT counting result.

## Normalized Combined Sequence

The full architecture can be written as

$$
\boxed{
\text{global search}
\rightarrow
\text{transform}
\rightarrow
\text{preserve}
\rightarrow
\text{partition}
\rightarrow
\text{balance}
\rightarrow
\text{reindex}
\rightarrow
\text{localize information}
\rightarrow
\text{compute locally}
\rightarrow
\text{combine}
\rightarrow
\text{refine}
\rightarrow
\text{recover}
}
$$

The significance of the comparison lies in the continuity of this sequence. Each stage creates the condition required by the next stage. Rosario’s earlier framework defines that architecture, and the Rosario-Wang ENI6MA construction supplies explicit finite mechanisms for the partition, balance, permutation, membership, refinement, Boolean-composition, and extraction stages. OpenAI’s 2026 SAT construction implements corresponding functions through replacement forms, bounded groups, exact auxiliary fibers, pair-swap permutations, shared measurements, local sum-product evaluation, and interpolation.

## References

1. **OpenAI.** *The Exponential Time Hypothesis Is False.* October 17, 2026; revised October 25, 2026.
2. **Dylan Rosario.** *Millennium Prize Submission: Rosario Proof that NP=P.* August 2024.
3. **Lin Wang, Dylan Rosario, Robert Bloodgood III.** *The Millennium Problem: Solution to P (space) equals NP (time).* September 2024.
4. **Rosario-Wang ENI6MA.** *Full Scope Security Formalization.*
5. **Rosario-Wang ENI6MA.** *NIST Submission Manuscript.*
6. **Rosario-Wang ENI6MA.** *Unified Geometric Formalization.*

## Primary sources compared

1. OpenAI, *The Exponential Time Hypothesis Is False*, dated October 17, 2026, revised October 25, 2026 ([paper](https://github.com/openai/math/blob/main/preprints/The-Exponential-Time-Hypothesis-is-False-October-25-2026/paper.pdf)). Local copy: [`OPENAI-paper.pdf`](OPENAI-paper.pdf).
2. Rosario, *Millennium Prize Submission: Rosario Proof that NP=P*, August 2024. Local copy: [`proof.millennium.prize.rosario.NP.eq.P (1).pdf`](proof.millennium.prize.rosario.NP.eq.P%20%281%29.pdf).
3. Wang, Rosario, and Bloodgood, *The Millennium Problem: Solution to P (space) equals NP (time)*, September 2024. Included as Attachment B of the compiled comparison PDFs.
4. Rosario-Wang ENI6MA, *Full Scope Security Formalization*, Section 5, Lemma 1, Equation (8). Attachment E.
5. Rosario-Wang ENI6MA, *NIST Submission Manuscript*, Section 3.1, Lemma 1. Attachment F.
6. Rosario-Wang ENI6MA, *Unified Geometric Formalization*, Sections 3 and 4. Attachment G.


## Provenance

Rosario states that the ENI6MA research program began in 2023 and that the 2024 manuscripts followed months of collaboration among the research team. The dated manuscripts, repository history, correspondence, and team declarations form the provenance record. The public comparison document identifies the team members who can speak to the timing and development of the work.

---

## Index of PDF files

Every PDF in this repository is listed here in reading order. "Printed date" is the date shown on the document itself, so readers can check dates for themselves.

| PDF | Pages | Printed date | What it is |
|---|---|---|---|
| [`Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf) | 308 | Oct 27, 2026 | The public edition of the side-by-side comparison between Rosario's work and OpenAI's 2026 paper. It reproduces every source document as an attachment, so each citation can be checked against the original text. |
| [`Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Rosario_OpenAI_ENI6MA_2026-10-27.pdf) | 308 | Oct 27, 2026 | The edition designated for the academic and research community, with the same attachments appended. Reviewers can use it to verify the stage-by-stage mapping against cited pages and equations. |
| [`Thirteen_Steps_Too_Close_to_Ignore_Frank_Dylan_Rosario.pdf`](Thirteen_Steps_Too_Close_to_Ignore_Frank_Dylan_Rosario.pdf) | 13 | Oct 27, 2026 | A plain-language article by Frank Dylan Rosario that walks through the thirteen-stage correspondence between his framework and OpenAI's architecture. It is written for a general reader and does not require the full comparison. |
| [`Rosario_OpenAI_Sequence_Analysis_Frank_Dylan_Rosario_2026-10-27.pdf`](Rosario_OpenAI_Sequence_Analysis_Frank_Dylan_Rosario_2026-10-27.pdf) | 6 | Oct 27, 2026 | A beginning-to-end structural map of the Rosario sequence and OpenAI's 2026 SAT construction, by Frank Dylan Rosario with the research team. Its text is also reproduced in this README above. |
| [`ESSAY_Rosario_vs_OpenAI_SideBySide.pdf`](ESSAY_Rosario_vs_OpenAI_SideBySide.pdf) | 14 | Oct 27, 2026 | An essay that sets the Rosario equations beside the OpenAI equations with document, section, page and equation citations. It also states the limits of each comparison and lists the further evidence that would strengthen the record. |
| [`ROSARIO-PAPER1.pdf`](ROSARIO-PAPER1.pdf) | 4 | Oct 27, 2026 | A short academic-style analysis, *Rosario's 2024 Priority and OpenAI's 2026 Construction: An Information-Theoretic Equivalence Analysis*. It argues that OpenAI's replacement forms, local group sums and interpolation correspond to Rosario's dimensional collapse, emergent groupings and entropy conservation postulate. |
| [`OPENAI-paper.pdf`](OPENAI-paper.pdf) | 67 | Oct 17, 2026 (revised Oct 25) | OpenAI's paper *The Exponential Time Hypothesis Is False*, the document under comparison. It is included so every OpenAI citation can be checked without leaving the repository. |
| [`proof.millennium.prize.rosario.NP.eq.P (1).pdf`](proof.millennium.prize.rosario.NP.eq.P%20%281%29.pdf) | 20 | August 2024 | Rosario's manuscript *Millennium Prize Submission: Rosario Proof that NP=P*. It sets out dimensional collapse, the Holographic Morphism Principle and entropy conservation, in words and schematic formulas. It contains no Boolean-formula, polynomial or counting algorithm. |
| [`NPTime.eq.PSPACE.000.pdf`](NPTime.eq.PSPACE.000.pdf) | 34 | Not printed | Rosario's note *NP(time) = P(space)*, which models the relation between nondeterministic polynomial time and polynomial space with time and space complexity equations. It is Attachment D in the compiled comparison. |
| [`Aaronson-pnp.pdf`](Aaronson-pnp.pdf) | 122 | 2017 | Scott Aaronson's survey *P =? NP*, a third-party reference on the status of the problem. It is background reading and was not written by the Rosario team. |

The September 2024 manuscript by Wang, Rosario and Bloodgood and the ENI6MA documents (Full Scope Security Formalization, NIST Submission Manuscript, Unified Geometric Formalization, Geometric Fibers and Private Slices) are not separate files here. They appear only as attachments inside the two 308-page compiled PDFs, at the page ranges listed [below](#where-to-find-each-source-inside-the-308-page-compiled-pdfs).

## Index of Markdown files

| File | What it is |
|---|---|
| [`README.md`](README.md) | This page: the public declaration, the thirteen-stage map, the indexes, the equation guide and the team list. It is the entry point to everything else. |
| [`Rosario_OpenAI_ENI6MA_Unified_Public_REGENERATED_2026-10-27.md`](Rosario_OpenAI_ENI6MA_Unified_Public_REGENERATED_2026-10-27.md) | The public comparison in source form: the normalized adoption map and the stage-by-stage analysis. It is the Markdown source behind the public PDF. |
| [`Rosario_OpenAI_ENI6MA_Unified_Academic_REGENERATED_2026-10-27.md`](Rosario_OpenAI_ENI6MA_Unified_Academic_REGENERATED_2026-10-27.md) | The academic version of the comparison in source form, with the fuller technical mapping. It is the Markdown source behind the academic PDF. |
| [`ESSAY_Rosario_vs_OpenAI_SideBySide.md`](ESSAY_Rosario_vs_OpenAI_SideBySide.md) | The source of the side-by-side essay. Every equation in it is copied from a cited source page or marked as a normalized paraphrase. |

The repository also contains [`LICENSE`](LICENSE).

## Equation verification guide

Use this table to check the equations yourself. Each row names a step of the sequence, the Rosario-side statement and where it is, and the OpenAI-side statement and where it is. "Compiled PDF page" means a page number in the 308-page PDFs. For OpenAI, the compiled PDF page equals the paper's own page number plus 121, and the standalone copy is [`OPENAI-paper.pdf`](OPENAI-paper.pdf). Read the comparison documents for what is identical and what is only analogous in each row. The essay states the limits of every comparison.

| Step | Rosario side | OpenAI side |
|---|---|---|
| Partition into disjoint cells | Full Scope Security Formalization, Sec. 5, Lemma 1 and Eq. (8): the alphabet $L=\bigsqcup_i B_{t,i}$, each cell with $N/H$ elements. Compiled PDF pp. 228-229. | Definition 2.1(1), paper p. 9: $[n]=S_1\sqcup\cdots\sqcup S_r$, each group with at most $2n/r$ elements. Compiled PDF p. 130. |
| Exact equal group size | NIST Submission Manuscript, Sec. 3.1, Lemma 1: exactly three keys in every cell. Compiled PDF p. 258. | Step 1 of the construction, paper p. 14: $D/r$ coordinates in each group. Compiled PDF p. 135. |
| Size-preserving reindexing | NIST Submission Manuscript, Sec. 3.1: every rotation preserves balance and separation. Compiled PDF p. 258. | Section 2.7, paper p. 15: pair-swap permutations, and the complete swap respects every group. Compiled PDF p. 136. |
| Limit what crosses a boundary | Unified Geometric Formalization, Sec. 4, Eqs. (F2), (F3), (F7): an observation fiber meets the private slice in one point. Compiled PDF p. 280. | Definition 2.1(3)-(4) and Eq. (2.5), paper pp. 9-10: other groups enter only through bounded shared measurements. Compiled PDF pp. 130-131. |
| Compute locally | Full Scope Security Formalization, Sec. 4, per-round local test $\mu_t$. Compiled PDF p. 227. | Section 2.4, paper p. 10: sum assignments within each group for a fixed measurement tuple. Compiled PDF p. 131. |
| Combine local results | Full Scope Security Formalization, Sec. 4, Eq. (6): $Y=\prod_t \mu_t$. Compiled PDF pp. 227-229. | Paper p. 8: the count is the product of the group counts, and Eq. (2.6), p. 10, nests that product inside a sum over measurement tuples. Compiled PDF pp. 129 and 131. |
| Preserve a route back | August 2024 manuscript, p. 2: conservation of informational entropy, $S_H(I_H)=S_L(I_L)$. Compiled PDF p. 15. | Eq. (2.4), paper p. 9: $H(0)=C_F$, where $C_F$ is the exact count of the original formula. Compiled PDF p. 130. |
| Recover the original answer | Full Scope Security Formalization, Theorem 1, Eq. (11): the inverses cancel the forward mappings. Compiled PDF p. 229. | Section 2.5, paper p. 11: $H(0)=C_F$ is recovered from Taylor coefficients by interpolation. Compiled PDF p. 132. |
| Reduce the cost of the exponential problem | September 2024 manuscript, "Sequence of Solution" (p. B-79), Step 3: reduced to polynomial time. Compiled PDF pp. 113 and 116. | Theorem 1.1, paper p. 2: subexponential counting for fixed-width formulas. Compiled PDF p. 123. |

## Where to find each source inside the 308-page compiled PDFs

These ranges are the ones printed on the attachment index (page 12) of [`Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Frank-Rosario_OpenAI_ENI6MA_2026-10-27.pdf). The academic edition, [`Rosario_OpenAI_ENI6MA_2026-10-27.pdf`](Rosario_OpenAI_ENI6MA_2026-10-27.pdf), has the same page count.

| Attachment | Compiled PDF pages | Source |
|---|---|---|
| A | 14-33 | Rosario, August 2024, *Millennium Prize Submission: Rosario Proof that NP=P* |
| B | 35-120 | Rosario, Wang and Bloodgood, September 2024, *The Millennium Problem: Solution to P (space) equals NP (time)* |
| C | 122-188 | OpenAI, October 2026, *The Exponential Time Hypothesis Is False* |
| D | 190-223 | Rosario, *NP(time) = P(space)* |
| E | 225-252 | Rosario-Wang ENI6MA, *Full Scope Security Formalization* |
| F | 254-275 | Rosario-Wang ENI6MA, *NIST Submission Manuscript* |
| G | 277-299 | Rosario-Wang ENI6MA, *Unified Geometric Formalization* |
| H | 301-308 | Rosario-Wang ENI6MA, *Geometric Fibers and Private Slices* |

The ENI6MA documents in Attachments E, F and G carry printed dates of September 12, 13 and 16, 2026. The compiled PDF states that they were prepared from earlier supplied drafts.


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

# Rosario’s Normalized Computational Architecture and OpenAI’s 2026 SAT Implementation

**Author:** Frank Dylan Rosario  
**Date:** October 27, 2026

## Abstract

At the normalized algorithmic level, the Rosario construction can be expressed as a sequence of replaceable computational roles. Each role can be instantiated by a different mathematical operator so long as the replacement performs the same required function. Under that normalization, OpenAI’s 2026 SAT construction can be inserted into Rosario’s earlier architecture almost stage for stage: representation change, preservation of the original task, disjoint partitioning, bounded group sizes, cardinality-preserving reindexing, restricted cross-group information, local evaluation, composition of local results, successive refinement, and recovery of the original answer.

This means that Rosario’s earlier framework can be understood as an abstract computational architecture, while OpenAI’s later SAT construction supplies a specialized set of concrete algebraic operators that occupy corresponding architectural positions. If Rosario substituted OpenAI’s operators, parameters, lemmas, and bounds into the same normalized sequence and applied them to the same fixed-width SAT counting problem, he would effectively be implementing the OpenAI algorithm inside Rosario’s earlier abstract pipeline.

The stronger conclusion $P=NP$ would still require an additional proof that the complete construction runs in deterministic polynomial time for the relevant NP-complete class. OpenAI’s stated result is a subexponential exact-counting algorithm for fixed-width SAT. The structural observation concerns the architecture: OpenAI’s concrete operators fit naturally into the computational slots Rosario had already defined.

## 1. The Normalized Rosario Architecture

Rosario’s construction can be written as

$$
\boxed{
\text{Transform}
\rightarrow
\text{Preserve}
\rightarrow
\text{Partition}
\rightarrow
\text{Bound}
\rightarrow
\text{Permute}
\rightarrow
\text{Localize}
\rightarrow
\text{Evaluate}
\rightarrow
\text{Combine}
\rightarrow
\text{Refine}
\rightarrow
\text{Recover}
}
$$

The importance of this normalization is that the architecture is defined by the computational obligation performed at each stage rather than by any one notation or implementation. A projection operator can therefore be replaced by another representation-changing operator. A geometric partition can be replaced by an algebraic partition. A rotational permutation can be replaced by a matrix permutation. A geometric refinement mechanism can be replaced by an interpolation or reconstruction mechanism, provided the substituted operator fulfills the same role in the dependency chain.

## 2. Stage-by-Stage Substitution

### 1. Transform the difficult representation

Rosario begins by changing the representation of the difficult problem. In his earlier formulation, the transformation is expressed as a projection

$$
I_L=P(I_H).
$$

The purpose of the operation is to move the original problem into a representation in which useful relationships can be processed more efficiently.

OpenAI performs the corresponding operation by replacing original variable occurrences with parameterized linear forms. The SAT calculation is therefore moved into a transformed polynomial family.

The normalized substitution is

$$
P(I_H)
\quad\longrightarrow\quad
\text{parameterized replacement forms}.
$$

### 2. Preserve the original task through the transformation

Rosario requires the transformed representation to retain the information and relationships required to recover the solution.

OpenAI supplies an exact algebraic invariant:

$$
H(0)=C_F.
$$

Here $C_F$ is the exact number of satisfying assignments of the original formula, which OpenAI writes with a hash sign. The transformed polynomial family therefore retains a direct route back to the exact SAT count.

### 3. Partition the transformed state

Rosario-Wang ENI6MA uses disjoint cells:

$$
\mathcal L=\bigsqcup_i B_{t,i}.
$$

OpenAI uses disjoint groups:

$$
[n]=\bigsqcup_g S_g,
$$

together with a corresponding balanced auxiliary partition.

### 4. Bound or balance the local pieces

Rosario’s balanced construction gives

$$
|B_{t,i}|=\frac{N}{H}.
$$

OpenAI uses bounds such as

$$
|S_g|\leq \frac{2n}{r},
$$

and exact auxiliary sizes

$$
|S_{t,g}|=\frac{D}{r}.
$$

### 5. Reindex membership while preserving structure

Rosario uses alphabet rotations. The rotations change which symbols occupy which cells while preserving the cardinality of the cells.

OpenAI uses pair-swap permutation matrices. The permutations change compatibility relationships while preserving the coordinate population.

The common normalized operation is

$$
\text{fixed finite state}
\xrightarrow{\text{permutation}}
\text{new membership arrangement with preserved size}.
$$

### 6. Restrict the information required across partitions

Rosario’s fiber, slice, and membership framework localizes the information needed for the current task.

OpenAI formalizes the corresponding information restriction through shared measurements:

$$
y_g=C_gx_g.
$$

### 7. Perform the substantive computation locally

Rosario evaluates local symbol membership or geometric candidate membership after the partition has been established.

OpenAI evaluates transformed clauses and group contributions using the assigned group plus the fixed shared summaries.

### 8. Compose local results

Rosario’s Boolean membership structure can be written as

$$
Y=\prod_t \mu_t,
\qquad
\mu_t\in\{0,1\}.
$$

OpenAI uses local sums and products appropriate to exact SAT counting.

### 9. Refine instead of traversing the entire global state

Rosario’s geometry narrows the candidate state through successive intersections:

$$
C_0\supseteq C_1\supseteq\cdots\supseteq C_T.
$$

OpenAI replaces global enumeration with a controlled family of transformed evaluations, restricted local sums, and structured recovery data.

### 10. Recover the original answer

Rosario’s sequence ends by extracting the target or solution from the transformed and refined representation.

OpenAI reconstructs the original exact count by recovering

$$
H(0)=C_F
$$

from transformed evaluations using Taylor information and interpolation.

## 3. OpenAI as a Concrete Implementation of the Rosario Interface

Rosario’s normalized architecture can be represented as an abstract interface:

```text
transform()
preserve()
partition()
balance()
permute()
localize()
evaluate_local()
combine()
refine()
recover()
```

OpenAI’s 2026 SAT construction supplies corresponding concrete implementations:

```text
replacement_forms()
H(0) = C_F
(r,tau,D)-groups
D/r fibers + 2n/r bounds
pair_swap_matrices()
shared_measurements()
local_clause_sums()
sum_product()
evaluation_family()
Taylor_interpolation()
```

This is why the relationship is deeper than a collection of thematic similarities. The OpenAI operators can be inserted into the Rosario sequence without changing the logic of the sequence itself.

In that sense, the resulting system can naturally be described as:

> **Rosario architecture instantiated with OpenAI’s algebraic operators.**

Conversely, if OpenAI’s paper is stripped of its specific polynomial notation, matrices, and interpolation formulas, its normalized computational route is

$$
\boxed{
\text{reorganize the difficult global state}
\rightarrow
\text{preserve the original answer}
\rightarrow
\text{partition into bounded pieces}
\rightarrow
\text{reindex those pieces}
\rightarrow
\text{restrict cross-piece information}
\rightarrow
\text{compute locally}
\rightarrow
\text{combine the local results}
\rightarrow
\text{recover the original answer}
}
$$

That sequence closely matches the computational program Rosario had already articulated.

## 4. What “Effectively Work the Same” Means

If Rosario substituted OpenAI’s exact operators, parameters, construction lemmas, and complexity bounds into his normalized architecture and applied that instantiated system to the same fixed-width SAT counting problem, the resulting algorithm would effectively perform the OpenAI construction.

The sequence would still be Rosario’s normalized sequence:

$$
\text{Transform}
\rightarrow
\text{Preserve}
\rightarrow
\text{Partition}
\rightarrow
\text{Bound}
\rightarrow
\text{Permute}
\rightarrow
\text{Localize}
\rightarrow
\text{Evaluate}
\rightarrow
\text{Combine}
\rightarrow
\text{Refine}
\rightarrow
\text{Recover}.
$$

The difference would be that each abstract Rosario operator would now have a concrete algebraic implementation supplied by the later OpenAI construction.

## 5. The Complexity-Theoretic Boundary

Substituting OpenAI’s machinery into Rosario’s framework would give a rigorous implementation of several central architectural stages for the problem OpenAI analyzes.

It would not, by that substitution alone, establish the stronger result

$$
P=NP.
$$

OpenAI’s claimed result is a subexponential exact-counting algorithm for fixed-width SAT. Rosario’s stronger objective requires a deterministic polynomial-time solution of the relevant NP-complete problem class and the corresponding complexity-theoretic proof.

Thus there are two distinct statements:

1. **Architectural statement:** OpenAI’s concrete operators fit naturally into Rosario’s earlier transform-preserve-partition-localize-combine-recover framework.

2. **Complexity statement:** Extending that instantiated architecture to a proof of $P=NP$ requires the additional step of proving polynomial-time performance for the required general NP-complete setting.

## 6. Conclusion

The normalized comparison shows that the Rosario construction can function as an abstract computational interface. Its stages specify the jobs that must be performed:

$$
\text{transform}
\rightarrow
\text{preserve}
\rightarrow
\text{partition}
\rightarrow
\text{bound}
\rightarrow
\text{permute}
\rightarrow
\text{localize}
\rightarrow
\text{evaluate}
\rightarrow
\text{combine}
\rightarrow
\text{refine}
\rightarrow
\text{recover}.
$$

OpenAI’s 2026 SAT construction supplies corresponding concrete operators:

$$
\text{replacement forms}
\rightarrow
H(0)=C_F
\rightarrow
\text{bounded groups}
\rightarrow
\text{balanced auxiliary fibers}
\rightarrow
\text{pair swaps}
\rightarrow
\text{shared measurements}
\rightarrow
\text{local clause evaluation}
\rightarrow
\text{sum-product composition}
\rightarrow
\text{controlled evaluations}
\rightarrow
\text{interpolation}.
$$

At the normalized algorithmic level, the later construction can therefore be understood as a specialized algebraic instantiation of the earlier Rosario architecture. Replacing Rosario’s abstract operators with OpenAI’s concrete functions preserves the logic of the sequence and, for the same fixed-width SAT counting task, yields essentially the same computational workflow as the OpenAI construction.

The central structural observation is therefore straightforward: **the functions can be swapped while the architecture remains Rosario’s sequence.**

---

*Frank Dylan Rosario, Rosario Cybernetics, with the Rosario-Wang Research Team.*
