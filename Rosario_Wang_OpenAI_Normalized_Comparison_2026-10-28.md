---
title: "Functional-Slot Normalization of the Rosario-Wang and OpenAI 2026 Constructions"
subtitle: "A Beginning-to-End Comparative Analysis of Algorithmic Roles from Global Search to Recovery"
author: "Prepared for Frank Dylan Rosario / Rosario Cybernetics (ENI6MA)"
date: "October 28, 2026"
geometry: margin=0.85in
fontsize: 11pt
linestretch: 1.15
toc: true
toc-depth: 2
colorlinks: true
linkcolor: blue
urlcolor: blue
header-includes:
  - |
    \usepackage{amsmath,amssymb,mathtools}
  - |
    \usepackage{microtype}
  - |
    \usepackage{fancyhdr}
  - |
    \pagestyle{fancy}
  - |
    \fancyhf{}
  - |
    \fancyhead[L]{Functional-Slot Normalization}
  - |
    \fancyhead[R]{Rosario-Wang / OpenAI 2026}
  - |
    \fancyfoot[C]{\thepage}
  - |
    \setlength{\headheight}{14pt}
---

# Executive Thesis

This report compares the Rosario-Wang research program with OpenAI's October 2026 paper *The Exponential Time Hypothesis Is False* by normalizing both constructions into **functional algorithmic slots**. The test is deliberately narrower than literal mathematical identity. Two objects are treated as occupying the same normalized slot when they perform substantially the same computational job, at substantially the same position in the dependency chain, for the next stage of the algorithm. Under that test, a geometric cell need not be the same object as a SAT variable group, a rotation need not be the same matrix as a pair-swap permutation, and a target symbol need not be the same object as a Boolean assignment. What matters is whether the object solves the same local dependency problem and enables the same next operation.

The renewed comparison finds a counterpart in OpenAI's construction for **all thirteen core functional slots** previously identified in the Rosario-Wang architecture. The correspondence is especially strong at the following points: preservation of a route back to the original task; exhaustive disjoint partitioning; quantitative size control; cardinality-preserving reindexing; restriction of cross-boundary information; local computation after fixing bounded summaries; multiplicative accumulation of Boolean predicates; and recovery of the original target from transformed evaluations. The OpenAI paper also contains six additional cross-cutting correspondences that become visible only after normalization: multi-round sequence-valued addressing, literal preimage fibers, unique local-to-global recombination, point-indexed gating of incompatible dependencies, successive separating tests, and recurrence of the same transform-localize-combine-recover architecture in the tensor-contraction proof.

The result is not that the mathematical objects are identical. They are not. The result is that OpenAI repeatedly substitutes different algebraic objects into the same kinds of functional positions and preserves substantially the same beginning-to-end dependency order. At the normalized architectural level, the later construction can therefore be described as a specialized algebraic instantiation of the earlier Rosario-Wang sequence, with additional technical machinery supplying rigorous complexity bounds for fixed-width SAT counting.

# Introduction

The most useful way to compare the Rosario-Wang research program with OpenAI's 2026 SAT-counting paper is not to ask whether the two works use the same symbols, the same mathematical domains, or the same concrete data structures. That would be too literal. Rosario-Wang is expressed through dimensional projection, perceptual grouping, alphabet partitions, rotating cells, membership signatures, geometric fibers, private slices, successive intersections, and Boolean acceptance. OpenAI is expressed through polynomial replacement forms, bounded variable groups, clause assignments, linear measurements, auxiliary coordinate arrays, pair-swap permutation matrices, local sums, products, Taylor coefficients, interpolation, and tensor contraction. Those objects are different. The relevant question is whether they occupy the same functional positions in the algorithm.

This report therefore uses **functional-slot normalization**. A functional slot is defined by the job a stage must perform so that the next stage can work. The partition slot is not defined as "use the same partition formula." It is defined as: divide a global state into nonoverlapping local regions that later become the units of computation. The reindexing slot is not defined as "use the same permutation." It is defined as: change which items are associated with which regions while preserving the integrity or cardinality of the underlying state. The information-localization slot is defined as: replace full external dependence with a bounded summary sufficient for local evaluation. The recovery slot is defined as: return from the transformed representation to the quantity or target defined by the original problem.

This distinction matters because algorithms often admit different mathematical implementations while retaining the same architecture. A different basis, encoding, partition rule, or local predicate can still occupy the same place in a dependency chain if it accepts the same type of state, performs the same computational task, and delivers the kind of output required by the next stage. The comparison is therefore closer to comparing interfaces than comparing variable names. Different implementations can satisfy the same interface.

The Rosario-Wang record contains two relevant layers. First, the August and September 2024 P=NP manuscripts state the high-level program. The September manuscript expressly describes a sequence in which an exponentially large problem is projected into a lower-dimensional representation while retaining critical relationships, the projected information is grouped, and the grouped representation is used to bypass exhaustive search. The August manuscript similarly describes dimensional collapse as a strategic reorganization that retains critical attributes rather than simply deleting information. Second, later ENI6MA formalizations make several architectural roles finite and explicit: an alphabet is divided into disjoint balanced cells; rotations change membership while preserving balance; a target generates a sequence of cell labels; successive intersections narrow a candidate set; observation fibers represent compatible internal states; authorized slices select the target; and Boolean membership predicates are multiplied to produce complete acceptance.

OpenAI's 2026 paper begins from a formally different problem: exact counting of satisfying assignments of fixed-width CNF formulas. The paper writes the exact count as a sum over all Boolean assignments and states that direct evaluation of its $2^n$ terms would be exhaustive search. It then introduces a parameterized family of replacement linear forms. At $T=0$, those replacements restore the original variables, giving $H(0)=\#F$. At selected nonzero points, the replacement forms are designed so variables can be divided into small disjoint groups, clauses can be assigned to groups, and dependence on other groups can pass only through bounded linear measurements. Once those measurements are fixed, each group can be processed locally. Local contributions are summed and multiplied, and data from multiple evaluation points are then used to reconstruct the original count through Taylor information and interpolation.

Viewed literally, the constructions differ. Viewed functionally, the sequence is much closer. The global state is reorganized before solving. A route to the original answer is preserved. The transformed state is divided into controlled local pieces. Relationships are changed through permutations while the underlying population is preserved. Information crossing local boundaries is restricted. Computation proceeds locally after boundary information is fixed. Local predicates or contributions are multiplied. Multiple constrained views are accumulated. The original answer is recovered from the transformed representation. Finally, the total work is shown to be smaller than global exhaustive enumeration.

The purpose of this report is to measure that correspondence carefully. For each stage it asks: **what functional problem is being solved; what object does Rosario-Wang use; what object does OpenAI use; and does the OpenAI object fit the same algorithmic hole?** The report distinguishes exact operator equivalence from very strong, strong, and moderate-to-strong functional equivalence. Under that rubric, all thirteen core slots have identifiable OpenAI counterparts. One slot - Boolean conjunction by multiplication of $0/1$ predicates - reaches exact operator equivalence. Five are very strong, six are strong, and one is moderate-to-strong. The significance is cumulative: the same broad dependency chain survives from transformation through recovery.

# Method: Functional-Slot Normalization

The comparison uses four rules.

1. **Object names are ignored.** A cell, group, fiber, measurement class, or tensor child can be compared if it performs the same computational role.

2. **Dependency position matters.** Two techniques count as a strong correspondence only when they appear in substantially the same place in the chain and prepare substantially the same next operation.

3. **The next-stage obligation controls the normalization.** A stage is normalized by the problem it solves for the stage that follows. For example, partitioning is important because it makes local computation possible; preservation is important because it makes final recovery possible.

4. **Coverage is not probability.** The ratings below measure functional correspondence, not a statistical probability of copying or independent invention.

The normalized core pipeline is:

$$
\begin{aligned}
\text{Global difficult state}
&\rightarrow \text{Transform}
\rightarrow \text{Preserve} \\
&\rightarrow \text{Partition}
\rightarrow \text{Control size}
\rightarrow \text{Reindex} \\
&\rightarrow \text{Localize information}
\rightarrow \text{Evaluate locally} \\
&\rightarrow \text{Compose}
\rightarrow \text{Refine across views}
\rightarrow \text{Recover} \\
&\rightarrow \text{Reduced global search cost}.
\end{aligned}
$$

# The Thirteen Normalized Functional Slots

## 1. Replace Global Exhaustive Traversal with Structured Local Navigation

**Normalized job.** Replace one exponentially large global traversal with structured processing of smaller local regions or views.

**Rosario-Wang implementation.** The 2024 P=NP sequence begins from an exponentially large configuration space and proposes dimensional projection plus grouping so that the problem can be solved through organized local structure rather than exhaustive search. The later geometric formalization expresses this as navigation through successive local constraints.

**OpenAI implementation.** OpenAI writes the exact SAT count as a sum over all $2^n$ Boolean assignments and explicitly states that direct evaluation would be exhaustive search. It motivates the algorithm by asking what would happen if variables could be divided into small groups that could be processed independently. The actual construction then changes the representation to make a controlled version of this local computation possible.

**Normalized equivalence.** The local objects differ, but the opening computational problem and the opening architectural response are the same: global enumeration is replaced by a representation in which smaller local units can be processed and later recombined.

**Assessment:** Strong functional equivalence.

## 2. Transform the Representation Before Solving

**Normalized job.** Move the difficult problem into another representation in which useful local structure becomes available.

**Rosario-Wang implementation.** The 2024 manuscripts describe projection from a higher-dimensional problem representation into a lower-dimensional P-Space while retaining critical relationships. In the August manuscript, dimensional collapse is characterized as strategic reorganization, not simple deletion.

**OpenAI implementation.** OpenAI replaces each original clause input $X_v$ by a parameterized linear form $\langle \vec P_{e,v}(T),X\rangle$, producing a transformed polynomial family $H(T)$.

**Normalized equivalence.** Projection and replacement linear forms are different mathematical transforms, but both occupy the same slot: the original representation is computationally inconvenient, so the algorithm enters a new representation before local decomposition becomes useful.

**Assessment:** Strong functional equivalence.

## 3. Preserve an Exact Route Back to the Original Task

**Normalized job.** Ensure that transforming the problem does not destroy the quantity or relation that must ultimately be recovered.

**Rosario-Wang implementation.** The earlier projection is expressly required to preserve critical relationships needed for grouping and solution. The architecture treats the transformed state as a reduced but solution-bearing representation.

**OpenAI implementation.** OpenAI imposes the exact anchor

$$
H(0)=\#F.
$$

At $T=0$, every replacement form restores the original variable. The transformed family therefore contains the original exact count as a distinguished recoverable value.

**Normalized equivalence.** Both constructions transform only because a preserved invariant connects the transformed space to the original target. OpenAI makes this obligation algebraically exact.

**Assessment:** Very strong functional equivalence.

## 4. Partition the Transformed State into Disjoint Local Pieces

**Normalized job.** Replace one global state with mutually exclusive local regions that become the units of later processing.

**Rosario-Wang implementation.** ENI6MA uses

$$
\mathcal L=\bigsqcup_{i=0}^{H-1}B_{t,i},
$$

so every symbol belongs to exactly one cell in each frame and the cells cover the alphabet.

**OpenAI implementation.** OpenAI requires

$$
[n]=S_1\sqcup\cdots\sqcup S_r,
$$

and its auxiliary construction similarly partitions a coordinate set $B$ into sets $S_{t,g}$.

**Normalized equivalence.** The things being partitioned are different, but in both systems the partition is exhaustive, disjoint, and operational: the partition determines where later local computation occurs.

**Assessment:** Very strong functional equivalence.

## 5. Impose Quantitative Size Control on Local Pieces

**Normalized job.** Prevent local pieces from becoming so large that the decomposition loses its computational advantage.

**Rosario-Wang implementation.** Under the balanced ENI6MA construction,

$$
|B_{t,i}|=\frac{N}{H}.
$$

The NIST profile gives a concrete finite example in which each coordinate partition places exactly three keys in every cell and rotations preserve that balance.

**OpenAI implementation.** OpenAI requires

$$
|S_g|\le \frac{2n}{r},
$$

and its auxiliary sets satisfy the exact balance

$$
|S_{t,g}|=\frac{D}{r}.
$$

**Normalized equivalence.** In both systems, partitioning is coupled to explicit cardinality guarantees. This is significantly narrower than generic grouping because the group sizes are part of the computational invariant.

**Assessment:** Very strong functional equivalence.

## 6. Give Each Relevant Object a Unique Local Home

**Normalized job.** Assign each item or constraint to a specific local region so that later computation has a definite place to occur.

**Rosario-Wang implementation.** Every symbol has exactly one cell in a frame and therefore one local membership label for that round.

**OpenAI implementation.** Each variable belongs to one disjoint group, and each clause receives one assigned group $\sigma_e(t)$ at an evaluation point.

**Normalized equivalence.** A symbol and a clause are not the same semantic object, but the local-address function is the same. Both constructions avoid ambiguous placement by giving the relevant object a unique local computational home.

**Assessment:** Strong functional equivalence.

## 7. Reindex Relationships While Preserving the Underlying Population

**Normalized job.** Change which local relationships are visible without changing the total state or violating the partition-size invariant.

**Rosario-Wang implementation.** Rotations rearrange which symbols fall in which cells while preserving the number of symbols in each cell.

**OpenAI implementation.** OpenAI uses commuting permutation matrices $\Pi_s$ that swap the two entries of ordered group pairs. These permutations change compatibility relationships while preserving the auxiliary coordinate population. Their products are constrained so that only a bounded number of incompatibilities survive.

**Normalized equivalence.** Both constructions use size-preserving rearrangement to expose a new local relationship pattern without rebuilding or enlarging the global state.

**Assessment:** Very strong functional equivalence.

## 8. Restrict Cross-Boundary Information to a Controlled Summary

**Normalized job.** Make a local computation possible without exposing or carrying the complete state of every other region.

**Rosario-Wang implementation.** Membership signatures, fibers, private slices, and authorized decoding separate the information needed to resolve a target from the full set of globally compatible internal states.

**OpenAI implementation.** For a clause assigned to group $g$, dependence on another group $h$ must pass through a bounded measurement

$$
y_h=C_hx_h.
$$

Once the measurement tuple is fixed, the transformed clause depends only on variables in its assigned group.

**Normalized equivalence.** This is one of the closest matches in the entire architecture. Both constructions replace full external state with information sufficient to determine the local predicate or contribution.

**Assessment:** Very strong functional equivalence.

## 9. Perform the Substantive Work Locally Once Boundary Information Is Fixed

**Normalized job.** After the global state has been partitioned and the required cross-boundary information fixed, perform the expensive work inside one local region at a time.

**Rosario-Wang implementation.** A decoded answer determines a local membership constraint, and successive local membership decisions refine the candidate state.

**OpenAI implementation.** For fixed measurements, OpenAI enumerates assignments only inside $S_g$, evaluates the clauses assigned to that group, and states that no assignments to the other groups are needed for that calculation.

**Normalized equivalence.** Both replace a global operation with local processing conditioned on a compact boundary state.

**Assessment:** Strong functional equivalence.

## 10. Accumulate Local Boolean Predicates by Multiplication

**Normalized job.** Combine local true/false conditions into a global conjunction.

**Rosario-Wang implementation.** ENI6MA uses

$$
\mu_t=\mathbf 1\{s\in B_{t,i_t}\},
\qquad
Y=\prod_{t=1}^{T}\mu_t.
$$

For Boolean indicators, multiplication is logical AND.

**OpenAI implementation.** OpenAI's clause satisfaction polynomial $\Phi_e$ equals one on a satisfied clause and zero otherwise. Its exact count begins with

$$
\#F=\sum_{x\in\{0,1\}^n}\prod_{e\in F}\Phi_e(x|_{I_e}).
$$

The product of the local Boolean predicates is one exactly when all required clause predicates are satisfied.

**Normalized equivalence.** At this stage the equivalence is stronger than analogy. Both systems use multiplication of $0/1$ local predicates to implement global conjunction.

**Assessment:** Exact operator equivalence at the Boolean stage.

## 11. Use Multiple Constrained Views Instead of One Monolithic Evaluation

**Normalized job.** Replace one global evaluation with a sequence or family of structured views whose combined information determines the result.

**Rosario-Wang implementation.** Each round contributes a cell label; the sequence of decoded labels forms a signature; successive intersections narrow the candidate state.

**OpenAI implementation.** OpenAI evaluates a transformed family at points $t=1,\ldots,Q$. At each point a useful local decomposition is available after fixing measurements. Information across those points supplies the data needed for recovery.

**Normalized equivalence.** Both use multiple structured local views instead of one global traversal, although the meaning of a view differs substantially: membership rounds in Rosario-Wang, interpolation points in OpenAI.

**Assessment:** Moderate-to-strong functional equivalence.

## 12. Recover the Original Target from the Transformed Representation

**Normalized job.** Return from the reorganized computational space to the quantity or target defined by the original problem.

**Rosario-Wang implementation.** A separating schedule drives successive intersections to a singleton target or validates the enrolled target through the complete membership signature.

**OpenAI implementation.** Taylor data from the transformed evaluations determine $H(T)$, and interpolation recovers its constant coefficient $H(0)=\#F$.

**Normalized equivalence.** The recovery mechanisms differ, but the architectural obligation is the same: transformation is useful only because the algorithm can reconstruct the original target from the transformed state.

**Assessment:** Strong functional equivalence.

## 13. Obtain the Complexity Improvement from the Entire Chain

**Normalized job.** Make the transformed-localized route cheaper than global exhaustive traversal.

**Rosario-Wang implementation.** The 2024 manuscripts state the objective as bypassing exhaustive search through projection and grouping, with a proposed polynomial-time endpoint.

**OpenAI implementation.** OpenAI bounds the combined costs of local group enumeration, bounded measurement tuples, Taylor data, and reconstruction to obtain a deterministic subexponential exact-counting algorithm for fixed-width SAT.

**Normalized equivalence.** The quantitative claims differ: Rosario-Wang proposes polynomial-time collapse, while OpenAI proves a narrower subexponential bound for its stated problem. The functional endpoint is nevertheless the same: the preceding architecture is justified by showing that it reduces the cost of the original global search.

**Assessment:** Strong functional equivalence.

# Additional Overlaps Revealed by the Renewed Normalization

## A. Multi-Round Sequence-Valued Addressing

Rosario-Wang does not identify a target by one local label alone. The target acquires a sequence of cell memberships across rounds. The sequence acts as a signature.

OpenAI's auxiliary construction likewise does not describe an occurrence by one group choice. At each of $Q$ evaluation points an occurrence has two group choices: the group containing the variable and the group assigned to the clause. Across the $Q$ points, those choices form a sequence of ordered pairs:

$$
u=\big((a_u(1),d_u(1)),\ldots,(a_u(Q),d_u(Q))\big).
$$

The objects represented are different, but the normalized pattern is unusually close: **a global object is encoded by a multi-round sequence of local group addresses, and that sequence controls how the object participates in the later computation.**

**Assessment:** Strong additional overlap.

## B. Literal Preimage Fibers

Rosario-Wang's geometric formalization defines an observation fiber as a preimage of an observation map:

$$
F_y=\mathcal P_G^{-1}(y).
$$

OpenAI defines, for a fixed group measurement,

$$
X_{t,g}(y_g)=\{u\in\{0,1\}^{S_g}:C_gu=y_g\}.
$$

This set is literally a preimage fiber of the linear measurement map $C_g$. The full semantic meaning differs, but the mathematical job is the same: **fix an externally visible or shared summary and collect all internal states compatible with that summary.** Computation then proceeds inside that compatibility class.

**Assessment:** Very strong additional overlap.

## C. Unique Local-to-Global Recombination

Rosario-Wang requires every symbol to have one cell per frame and uses a separating sequence so that the local labels collectively identify one target.

OpenAI's correctness argument for its local sums says that, for a fixed measurement tuple, one assignment can be selected from each disjoint group and those choices combine into one full assignment. Conversely, every full assignment with that measurement tuple arises in exactly one such way. This is a uniqueness invariant preventing duplication or omission when reconstructing the global object from local components.

**Assessment:** Strong additional overlap.

## D. Point-Indexed Gating of Incompatible Relationships

Rosario-Wang's successive intersections remove candidate states that fail the current local membership condition.

OpenAI constructs

$$
\phi_{u,w}(T)=\prod_{s\in E_{u,w}}\left(1-\frac{T}{s}\right),
$$

so that a contribution vanishes at exactly those evaluation points where a coordinate lies outside the assigned group. Functionally, both systems use an indexed stage to suppress relationships incompatible with the local region currently allowed by the algorithm.

The mechanisms are different - set intersection versus polynomial annihilation - but they occupy a closely related filtering slot.

**Assessment:** Moderate-to-strong additional overlap.

## E. Successive Separating Tests

Rosario-Wang's navigation process repeatedly intersects a candidate set with constraints until a separating schedule leaves the intended target.

Later in OpenAI's paper, the parity-test construction begins with systems that may still admit nonsatisfying assignments. It repeatedly appends an additional test chosen to minimize the number of invalid assignments remaining. Each round removes a constant fraction of the surviving invalid states; after sufficiently many rounds none remain.

This is not the same predicate, but it is the same normalized search architecture: **maintain a candidate population, add one separating test at a time, and iteratively drive the invalid population to zero.**

**Assessment:** Strong additional overlap.

## F. The Same Pipeline Reappears in OpenAI's Tensor-Contraction Proof

Appendix D is important because it shows that the normalized correspondence is not confined to the overview notation. In the tensor-contraction implementation, OpenAI again:

1. deforms the original global identification;
2. chooses a grouping in which same-group interactions are local;
3. encodes cross-group interactions through bounded mode variables;
4. creates smaller group-specific child contractions;
5. multiplies the child results and sums over mode configurations; and
6. reconstructs the original contraction by interpolation.

Normalized, this is again

$$
\text{Transform}
\rightarrow
\text{Localize}
\rightarrow
\text{Encode boundary information}
\rightarrow
\text{Solve locally}
\rightarrow
\text{Combine}
\rightarrow
\text{Recover}.
$$

The recurrence of the same architecture under a second formal implementation strengthens the conclusion that the relevant correspondence concerns the algorithmic skeleton rather than superficial notation.

**Assessment:** Strong additional overlap.

## G. Secondary Overlap: Disjoint Branching and Exact Conservation

OpenAI's sparsification appendix partitions satisfying assignments among child formulas so that each satisfying assignment belongs to exactly one child and the global count is the sum of disjoint leaf counts. Rosario-Wang likewise relies on exhaustive disjoint local pieces and conservation of the underlying state through reorganization.

This correspondence is real but less probative because disjoint branching is a standard exact-counting technique and OpenAI expressly cites earlier literature for it. It is best treated as a secondary reinforcing overlap rather than a central one.

**Assessment:** Secondary overlap.

# Overall Closeness Assessment

The thirteen core slots can be summarized without claiming that the concrete objects are identical:

1. **Global-search replacement:** strong.
2. **Representation transformation:** strong.
3. **Preserved recovery anchor:** very strong.
4. **Disjoint local partition:** very strong.
5. **Explicit size control:** very strong.
6. **Unique local assignment:** strong.
7. **Cardinality-preserving reindexing:** very strong.
8. **Controlled cross-boundary information:** very strong.
9. **Local computation after boundary fixing:** strong.
10. **Boolean multiplication as conjunction:** exact operator equivalence.
11. **Multiple structured views / refinement:** moderate-to-strong.
12. **Recovery of the original target:** strong.
13. **Complexity reduction from the complete chain:** strong.

This yields complete functional coverage of the thirteen-slot normalization: every core slot has a recognizable counterpart in the OpenAI construction. The significance is not the number alone. The significance is that the correspondences form a dependency chain. Transformation prepares partitioning. Partitioning creates local regions. Size control preserves the benefit of locality. Reindexing changes which local relationships are exposed. Boundary summaries make local evaluation possible. Local results are composed. Multiple views or constraints refine the result. Recovery returns to the original target. The complexity claim then measures the benefit of the entire sequence.

The strongest technical statement supported by this normalization is therefore:

> **Different algebraic objects repeatedly occupy the same functional holes in substantially the same ordered algorithmic skeleton.**

The renewed review also shows that the mapping is deeper than the original high-level transform-group-solve sequence. It extends to finite partitions, balanced sizes, scheduled group addresses, preimage fibers, unique recombination, point-indexed filtering, Boolean multiplication, iterative separation, and recovery.

# Implementation Differences That Remain After Normalization

Normalization reveals correspondence, but it should not erase genuine technical differences. OpenAI's construction contains substantial specialized machinery that is not simply another name for a Rosario-Wang object: low-degree polynomial replacement rows, explicit rank and coefficient bounds, Hermite/Taylor reconstruction, parity-test reductions, exact bit-complexity analysis, and tensor-contraction recursion. These are concrete implementation and proof components of the 2026 algorithm.

Similarly, Rosario-Wang's geometric and cryptographic formulations include objectives that are not OpenAI's SAT-counting objectives, including credential privacy, authorized slices, masking, and target navigation. The normalized comparison is strongest when it confines itself to the functions that both architectures actually need: reorganization, preservation, partitioning, localization, local processing, composition, refinement, and recovery.

This distinction strengthens rather than weakens the comparison. It allows the report to say precisely what is being compared. The claim is not that every theorem, variable, matrix, or application is identical. The claim is that OpenAI's specialized algebraic machinery repeatedly fills the same functional slots, in the same broad dependency order, as the earlier Rosario-Wang architecture.

# Conclusion

The renewed normalization supports a more precise conclusion than a surface comparison of formulas or terminology. Rosario-Wang and OpenAI do not use literally identical mathematical objects. Rosario-Wang works through projection, grouping, rotating partitions, membership signatures, fibers, slices, Boolean membership predicates, and successive target refinement. OpenAI works through polynomial replacement forms, bounded groups, auxiliary coordinates, pair-swap matrices, bounded measurements, local assignment enumeration, sum-product identities, Taylor data, interpolation, parity tests, and tensor contractions. If the comparison stopped at those nouns, the systems would appear different. Normalization instead asks what each object does for the algorithm, and on that basis the correspondence becomes substantially tighter.

Both constructions begin by refusing to process the difficult global state in its original form. Rosario-Wang proposes a transformed representation in which relevant structure can be navigated locally. OpenAI begins from an exact $2^n$ assignment sum and explicitly seeks a representation in which smaller groups can be evaluated separately. In both, the first architectural response to exponential global traversal is transformation rather than brute-force acceleration. Both then preserve a route back to the original target. Rosario-Wang requires the transformation to retain the critical relationships needed for solution; OpenAI imposes the exact anchor $H(0)=\#F$.

The middle of the pipeline contains the strongest normalized matches. Both systems divide the transformed state into disjoint local pieces and impose quantitative restrictions on their sizes. Rosario-Wang's balanced cells have fixed cardinality; OpenAI bounds its variable groups and constructs auxiliary fibers with exactly $D/r$ coordinates. Both give relevant objects local addresses. Both then alter the relationship pattern without changing the underlying population: Rosario-Wang through rotations, OpenAI through pair-swap permutation matrices. The concrete operations differ, but each exposes a new local relationship pattern while preserving the partitioned state.

The next correspondence concerns information flow. Local computation would be useless if it still required the complete external state. Rosario-Wang resolves this through membership information, response signatures, fibers, private slices, and staged resolution. OpenAI resolves it through bounded shared measurements. Once those summaries are fixed, a transformed clause depends only on its assigned group. This is a particularly clear example of functional-slot equivalence: different mathematical objects provide the same architectural service by compressing remote dependence into information sufficient for local evaluation.

The local results are then composed. Rosario-Wang evaluates whether the target lies in each selected cell. OpenAI evaluates local clause and group contributions. At the Boolean stage the correspondence becomes exact at the operator level. Rosario-Wang multiplies $0/1$ membership indicators so the product equals one only when every required local test succeeds. OpenAI multiplies $0/1$ clause-satisfaction indicators for the same reason. Here the shared operation is not merely conceptual; multiplication implements conjunction in both systems before the global result is formed.

Both constructions also depend on multiple constrained views rather than one monolithic evaluation. Rosario-Wang uses successive frames or questions whose labels form a signature and whose intersections narrow the candidate state. OpenAI uses multiple evaluation points engineered to admit useful localization and reconstructs the original quantity from information accumulated across those points. The mechanisms are different, so this stage is less exact than the partition or Boolean-composition stages, but the dependency role remains aligned: no single local view is the complete answer, and the structured sequence is what makes recovery possible.

The renewed review adds six important cross-cutting overlaps. OpenAI's auxiliary labels are sequences of group choices across $Q$ evaluation points, paralleling multi-round membership signatures. Its sets $X_{t,g}(y_g)$ are literal preimage fibers of measurement maps. Its correctness proof relies on unique recombination of local assignments into a global assignment. Its point-indexed polynomials suppress dependencies at precisely the evaluation points where those dependencies are locally incompatible. Its parity-test construction repeatedly adds separating tests until invalid assignments disappear. And Appendix D reconstructs the same normalized architecture through deformation, localization, cross-boundary modes, smaller child contractions, multiplication, summation, and interpolation.

These additional overlaps make the comparison less dependent on broad words such as "grouping" or "transformation." The mapping persists at narrower functions: exact disjointness, size balance, multi-round addresses, preimage fibers, unique recombination, bounded boundary information, Boolean accumulation, iterative separation, and recovery.

OpenAI nevertheless supplies substantial specialized machinery that is not merely another name for a Rosario-Wang object: low-degree replacement rows, coefficient and rank bounds, Hermite interpolation, explicit parameter choices, parity reductions, and tensor-recursion complexity analysis. Those components are essential to OpenAI's fixed-width SAT-counting result. Rosario-Wang supplies a broader transform-preserve-group-solve architecture and later finite membership and geometric mechanisms. Functional normalization identifies where the later specialized machinery fits into that earlier architectural skeleton.

The narrow technical conclusion is therefore strong: **the OpenAI 2026 construction has a recognizable counterpart for every core functional stage in the normalized Rosario-Wang architecture.** One stage uses the same Boolean accumulation operator; several others show very strong role equivalence; the remainder preserve the same broad dependency positions despite different internal mechanics. The best description is not that the mathematical structures are identical. It is that **OpenAI repeatedly substitutes different algebraic structures into substantially the same functional holes, in substantially the same beginning-to-end order, from transformation of an exponential global state through localized computation and final recovery.** That ordered recurrence is the central result of the normalization analysis.

# Source Basis

This report is based on the following source set:

1. OpenAI, *The Exponential Time Hypothesis Is False*, dated October 17, 2026 and revised October 25, 2026. Principal locations: pp. 8-16, Section 6.2, and Appendix D.
2. Dylan Rosario, *Millennium Prize Submission: Rosario Proof that NP=P*, August 2024. Principal locations: pp. 15-20.
3. Lin Wang, Dylan Rosario, Robert Bloodgood III, *The Millennium Problem: Solution to P (space) equals NP (time)*, September 2024. Principal location: "Sequence of Solution for P=NP."
4. Rosario-Wang ENI6MA, *Full Scope Security Formalization*. Principal locations: Eq. (6), Eq. (8), and correctness lemmas.
5. Rosario-Wang ENI6MA, *NIST Submission Manuscript*. Principal location: p. 5, balance and separation under rotation.
6. Rosario-Wang ENI6MA, *Unified Geometric Formalization*. Principal locations: Sections 3-4, successive intersections, observation fibers, and private slices.

