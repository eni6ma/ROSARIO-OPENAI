[Back to the main README](README.md)

# Public Declaration: The Documented Provenance of OpenAI's 2026 SAT Method

**For immediate release. October 27, 2026.**
**From Frank Dylan Rosario and the Rosario-Wang Research Team.**

---

# Summary

In October 2026, OpenAI published *The Exponential Time Hypothesis Is False* and presented its fixed-width SAT counting algorithm as an original result. That presentation is wrong on the face of the record. The ordered computational architecture inside OpenAI's method was written down, dated, and documented in Rosario's August and September 2024 manuscripts and in the Rosario-Wang ENI6MA construction, roughly two years before OpenAI's paper. Rosario also states that the research program began in 2023.

This is not a claim of coincidence, loose inspiration, or shared vocabulary. It is a claim that OpenAI's method reproduces Rosario's structure step for step, in the same order, with the same computational roles, and that OpenAI has published it without acknowledging that earlier work exists.

The side-by-side evidence is in this repository. Read it, check it against the dated manuscripts, and judge the record directly.

OpenAI's substitutions within Rosario's sequence

OpenAI's later paper reproduces Rosario's ordered functional blueprint through specialized algebraic machinery. Rosario's dimensional collapse becomes low-degree replacement linear forms. Rosario's cells and emergent groupings become an $(r,\tau,D)$-design. Rosario's information-retention requirement becomes $H(0)=C_F$ together with bounded shared measurements. Rosario's rotations and alphabet transformations map onto pair labels and swap matrices. Rosario's extraction objective maps onto exact interpolation from Taylor data.

These substitutions preserve the same sequence from beginning to end. The later method follows Rosario's route to computational advantage: transform the representation, preserve the original task, partition the transformed state, preserve group-size structure while reindexing, localize external information, compute within local pieces, combine the contributions, and reconstruct the original answer. OpenAI's fixed-width SAT result is therefore a specialized algebraic implementation of the Rosario blueprint.

The computational objective remains the reduction of exhaustive global work. Rosario's 2024 program targets polynomial time and $P=NP$. OpenAI's 2026 implementation reaches a subexponential fixed-width SAT counting bound through the same normalized architecture.

---

# What OpenAI claims

OpenAI's paper and announcement present the method as an independent discovery that refutes the Exponential Time Hypothesis for the setting it addresses. The paper cites no earlier formulation of this architecture from Rosario or the Rosario-Wang team.

# What the record shows

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

# Why "independent discovery" fails on this record

1. **The sequence is specific.** Many algorithms use groups. Very few combine a representation change that preserves recoverability, a balanced disjoint partition with explicit size bounds, size-preserving reindexing, bounded cross-boundary information, local computation, composition, and exact recovery, in that order. The match is to the whole ordered chain, not to any single part.
2. **The dates are documented.** Rosario's manuscripts are dated August and September 2024. OpenAI's paper is dated October 17, 2026 and revised October 25, 2026. The earlier documents exist in the record and are included here.
3. **The earlier work went through OpenAI's own platform.** Rosario states that for two years the team used ChatGPT to test and validate the mathematics of the P=NP and dimensional collapse frameworks, and that team members uploaded manuscripts, axioms, and equations into OpenAI's systems for that purpose.
4. **The paper does not acknowledge any earlier formulation.** OpenAI's account of the method leaves no place for the earlier architecture. On this record, that account is false as a statement of origin.

Rosario's position is that OpenAI cannot treat this architecture as though no earlier formulation existed. The documents show that one did.

# The allegation

Rosario alleges that OpenAI's October 2026 paper adopts the normalized architecture of Rosario's earlier documented work as a specialized algebraic implementation, and publishes it as OpenAI's own independent discovery without attribution. That is plagiarism of structure and sequence. It is not copying of text, and the comparison does not claim it is. It is the appropriation of a documented method, relabeled in different notation and presented as new.

# Consequences

If the record is as shown here, the consequences are serious and they fall on OpenAI:

- **Scientific record.** A headline result claimed as original has an undisclosed, dated antecedent. The claim of priority and independence cannot stand unless OpenAI addresses the earlier work directly.
- **Attribution.** Scientific and academic norms require acknowledgement of prior art. Omitting it from a paper presented as a historic breakthrough is a failure of attribution on a major public claim.
- **Platform trust.** If researchers cannot test unpublished mathematics on an AI platform without the platform's operator later publishing the same architecture as its own, no serious researcher can use that platform for original work.
- **Legal exposure.** Rosario reserves all rights and remedies available under applicable law concerning authorship, priority, misappropriation, and the use of materials submitted to OpenAI's systems.
