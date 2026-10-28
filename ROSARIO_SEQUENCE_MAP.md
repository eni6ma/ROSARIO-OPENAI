[Back to the main README](README.md)

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
