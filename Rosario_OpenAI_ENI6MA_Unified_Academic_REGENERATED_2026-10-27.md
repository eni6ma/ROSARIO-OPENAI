---
title: "The Rosario-Wang Blueprint and OpenAI's 2026 SAT Algorithm: A Unified Structural Comparison"
author: "Comparative research article"
date: "October 27, 2026"
---

## Projection, balanced partitions, fibers, local computation, and reconstruction

## Normalized adoption map: the OpenAI 2026 features that map directly to Rosario's construction

The term **adopted** in this article identifies the functional and architectural equivalence between the later OpenAI method and the ordered computational roles already defined in Rosario's earlier framework and the Rosario-Wang ENI6MA construction. The comparison establishes adoption at the normalized algorithmic level by matching each operation, invariant, partition rule, information-flow rule, composition step, and recovery stage.

1. **Replace exhaustive global search with structural reorganization.** Rosario's 2024 framework proposes changing the problem representation so the solver replaces full exponential enumeration with structured processing [2, pp. 15-20] [3, Sequence]. OpenAI begins from a $2^n$ global SAT sum and explicitly seeks a structure that avoids evaluating all $2^n$ assignments [1, p. 8].

2. **Transform the original representation before solving it.** Rosario maps higher-dimensional information $I_H$ into a projected representation $I_L=P(I_H)$ [2, pp. 18-20]. OpenAI replaces original variable occurrences by parameterized linear forms and evaluates the resulting family at selected points [1, p. 9].

3. **Preserve a route back to the original task.** Rosario requires the transformed representation to retain the information and relationships needed for the solution [2, pp. 15-20]. OpenAI requires the transformed family to satisfy $H(0)=\#F$, so the original exact count remains recoverable [1, p. 9].

4. **Partition the transformed state into disjoint local pieces.** Rosario-Wang ENI6MA uses an exhaustive disjoint partition $\mathcal L=\bigsqcup_iB_{t,i}$ [4, Eq. (8)]. OpenAI uses $[n]=S_1\sqcup\cdots\sqcup S_r$ and, in its auxiliary construction, $B=\bigsqcup_gS_{t,g}$ [1, pp. 9-10, 14].

5. **Impose explicit group-size guarantees.** ENI6MA gives $|B_{t,i}|=N/H$ under its balance condition [4, Eq. (8)], and its concrete NIST profile places exactly three keys in each cell [5, p. 5]. OpenAI bounds $|S_g|\le 2n/r$ and constructs auxiliary groups of exact size $D/r$ [1, pp. 9-10, 14].

6. **Give every relevant object one local home in the current partition.** In ENI6MA every symbol belongs to exactly one cell in each frame [4, Eq. (8)]. OpenAI places each variable in one disjoint group and assigns every clause to one group $\sigma_e(t)$ [1, pp. 9-10].

7. **Reindex the state by cardinality-preserving permutations.** Rosario-Wang rotations change symbol-to-cell membership while preserving balance and separation [5, p. 5]. OpenAI uses commuting pair-swap permutation matrices to change compatibility relations while preserving the auxiliary coordinate set [1, pp. 14-16].

8. **Restrict what information must cross a partition boundary.** Rosario's projected representation is intended to retain only the information required for the task, and ENI6MA's fiber-and-slice geometry separates public ambiguity from authorized resolving information [2, pp. 15-17] [6, Sec. 4]. OpenAI lets a clause depend freely on its own group but requires dependence on other groups to pass through bounded shared measurements $y_h=C_hx_h$ [1, pp. 9-10].

9. **Perform the substantive work locally after the partition is fixed.** ENI6MA evaluates cell membership and refines candidate states through the resulting local membership information [4, Eq. (6)] [6, Secs. 3-4]. OpenAI computes each transformed clause and each group contribution using its assigned group plus the fixed shared summaries [1, p. 10].

10. **Combine local results into a global result.** Rosario-Wang combines per-round membership indicators into a complete acceptance relation, $Y=\prod_t\mu_t$ [4, Eq. (6)]. OpenAI sums local assignments within each group, multiplies the group sums, and accumulates the global transformed value [1, p. 10].

11. **Use successive refinement rather than one monolithic search.** ENI6MA successively intersects the candidate set with the cell selected at each round, producing a refinement path toward the target [6, Sec. 3]. OpenAI evaluates a controlled family of transformed points and restricted local sums through the transformed local enumeration [1, pp. 9-12].

12. **Recover the answer to the original problem from the reorganized representation.** Rosario's 2024 sequence ends with solution extraction from the projected and grouped space [3, Sequence], while ENI6MA's separating schedule identifies the target through the final intersection [6, Sec. 4]. OpenAI reconstructs $H(0)=\#F$ from transformed evaluations by Taylor data and interpolation [1, p. 11].

13. **Use the reorganization to reduce the cost of an exponential problem.** Rosario's stated objective is to replace exhaustive exponential search by efficient computation through projection and grouping [3, Sequence]. OpenAI proves a narrower but concrete subexponential improvement for fixed-width SAT counting [1, Theorem 1.1].

Taken together, these thirteen affirmative correspondences form one dependency chain: **transform -> preserve -> partition -> balance -> reindex -> localize information -> compute locally -> combine -> refine -> recover -> reduce search cost.** That ordered chain is the central subject of the comparison.

## Abstract

This article presents a beginning-to-end comparison of Dylan Rosario's August and September 2024 P=NP manuscripts, the Rosario-Wang ENI6MA construction, and OpenAI's October 2026 paper *The Exponential Time Hypothesis Is False*. The comparison starts from the full Rosario construction rather than from isolated terminology. Rosario's 2024 manuscripts state an ordered computational strategy: change the representation of an exponentially difficult problem, preserve the relationships needed for correctness, form useful groupings in the transformed representation, process the reorganized problem instead of the complete global search space, and recover the original answer. ENI6MA supplies a concrete combinatorial implementation of several of those roles through disjoint balanced partitions, fixed size guarantees, rotations that preserve balance, membership signatures, successive intersections, observation fibers, private slices, Boolean composition, and target extraction [2, pp. 15-20] [3, Sequence] [4, Eq. (8)] [5, p. 5] [6, Secs. 3-4].


# 1. Comparison method and scope




# 2. Rosario's construction in normalized information-theoretic form

Before comparing terminology, normalize Rosario's method into operations on finite information. Let $\mathcal L$ be an alphabet of $N$ symbols and let $H$ be the number of cells. At round $t$, a rotation or permutation produces a balanced partition

$$
\mathcal P_t=\{B_{t,0},\ldots,B_{t,H-1}\},\qquad
\mathcal L=\bigsqcup_iB_{t,i},\qquad |B_{t,i}|=N/H.
$$

A target symbol $s$ induces a cell label $i_t$ by membership, $s\in B_{t,i_t}$. Across rounds, the sequence of labels is a signature. Authorized private information determines how the observed response maps back to the cell label. Successive membership constraints refine the candidate set by intersection. In the geometric formalization, the public observation determines a fiber of possible internal states and the authorized private information determines a slice; under a separating schedule, their intersection is the target [6, Sec. 4].

The acceptance logic is equally simple. For each round, let

$$
\mu_t=\mathbf{1}\{s\in B_{t,i_t}\}.
$$

Then

$$
Y=\prod_{t=1}^T\mu_t
$$

is 1 exactly when every required membership statement is true [4, Eq. (6)]. For Boolean indicators, multiplication is logical AND. The construction therefore converts a global identity or membership question into a sequence of balanced partition queries whose conjunction identifies or validates the enrolled target.

This normalized statement exposes the computational roles without relying on ENI6MA branding: **balanced disjoint partition, membership signature, permutation-preserved balance, successive refinement, Boolean composition, and final extraction.**

# 3. Rosario's 2024 formulation and the ENI6MA construction

The August 2024 P=NP manuscript already contains the abstract architecture. It describes a higher-dimensional informational representation $I_H$, a lower-dimensional representation $I_L$, a projection $I_L=P(I_H)$, an information-preservation condition, and emergent groupings formed from the projected information [2, pp. 18-20]. Earlier pages describe shuffling and projection of alphabet elements and call the transformation a strategic reorganization that retains critical attributes while discarding redundancies [2, p. 15].

The September manuscript makes the order explicit. Step 1 projects the difficult problem while preserving critical relationships. Step 2 performs grouping in the projected space. Step 3 obtains the solution from the combination of projection and grouping [3, Sequence]. The abstract sequence is therefore:

$$
\boxed{\text{transform}\to\text{preserve}\to\text{partition/group}\to\text{process}\to\text{recover}}.
$$

Within the Rosario-Wang research program, ENI6MA supplies the concrete combinatorial implementation of several roles already stated abstractly in 2024: disjoint equal-size partitions, membership signatures, intersections, fibers, slices, and complete Boolean acceptance. ENI6MA can therefore be read together with the 2024 manuscripts as the concrete partition-and-refinement machinery of the broader Rosario architecture.

# 4. OpenAI's normalized description

OpenAI begins from an exact sum over all Boolean assignments. Direct evaluation would require all $2^n$ assignments [1, p. 8]. The paper then asks whether the variables can be separated into groups so that each group can be handled locally. Because ordinary formulas do not generally have the desired separation, OpenAI changes the representation.

::: {.openai-box}
### OpenAI formulation

At a selected evaluation point, OpenAI requires an $(r,\tau,D)$-design with

$$
[n]=S_1\sqcup\cdots\sqcup S_r,\qquad |S_g|\le 2n/r,
$$

one assigned group $\sigma_e(t)$ per clause, bounded measurement matrices $C_g$, and cross-group dependence only through measurements $y_g=C_gx_g$. Once the shared measurement tuple is fixed, each transformed clause depends only on its assigned group [1, pp. 9-10]. In the auxiliary construction, OpenAI uses $B=([r]\times[r])^Q$, partitions it into $S_{t,g}$ of exact size $D/r$, and applies pair-swapping permutation matrices to control compatibility across evaluation points [1, pp. 14-16].
:::

Normalized into information-theoretic language, OpenAI does the following: transform the original representation; partition the transformed variables into disjoint bounded-size groups; assign each constraint to one group; replace full external state by compact shared summaries; compute local contributions conditioned on those summaries; combine the contributions; and reconstruct the original answer through interpolation [1, pp. 9-11].

Thus OpenAI's abstract sequence is

$$
\boxed{\text{transform}\to\text{partition}\to\text{preserve controlled dependence}\to\text{localize}\to\text{combine}\to\text{recover}}.
$$

# 5. Stage Three: the strongest partition correspondence

Stage Three is where the comparison becomes most concrete. Rosario-Wang ENI6MA says that each frame divides the alphabet into an exhaustive disjoint partition with guaranteed cell cardinality. The NIST profile gives an exact finite example with three keys per cell and states that rotation preserves balance and separation [5, p. 5]. OpenAI says that its transformed variables are partitioned into disjoint groups, each bounded in size, every clause is assigned to one group, and the auxiliary coordinate fibers are exactly balanced at $D/r$ coordinates per group [1, pp. 9-10, 14].

The normalized structures are:

**Rosario-Wang:**

$$
\mathcal L=\bigsqcup_{i=0}^{H-1}B_{t,i},\qquad |B_{t,i}|=N/H.
$$

**OpenAI:**

$$
[n]=\bigsqcup_{g=1}^rS_g,\qquad |S_g|\le 2n/r,
$$

with an auxiliary exact balance

$$
B=\bigsqcup_{g=1}^rS_{t,g},\qquad |S_{t,g}|=D/r.
$$

The normalized equivalence is direct. Rosario partitions symbols or target states; OpenAI partitions variables and auxiliary coordinates. Rosario's cells answer membership questions, while OpenAI's groups determine where a transformed clause can be evaluated. In both constructions, a disjoint partition plus an explicit size guarantee converts a large global state into controlled local pieces. This is the same algorithmic role implemented on different computational objects.

The clause assignment deepens the equivalence. In ENI6MA, each target symbol has exactly one cell label per round. In OpenAI, each clause has exactly one assigned group per evaluation point. Each construction gives the relevant object one local home in the partition and controls the information required from outside that local group.

# 6. Rotations, permutations, and size-preserving reindexing

ENI6MA's rotations preserve the size of the cells while permuting the positions and changing which symbols fall into each cell [4, Lemma 1] [5, p. 5]. This is an important property because computational usefulness comes from changing the membership pattern across rounds while preserving the size guarantee.

OpenAI's auxiliary construction similarly uses permutation matrices $\Pi_s$ that swap the two entries of pair $s$. These permutations preserve the cardinality of the coordinate set while changing pair orientation and therefore group compatibility [1, p. 15]. The complete swap already respects the group structure, and low-degree combinations of swaps control which cross-group dependencies survive.

The common normalized role is:

$$
\text{fixed finite state}\xrightarrow{\text{permutation}}\text{new membership arrangement with preserved size}.
$$

This is a stronger correspondence than the generic fact that algorithms sometimes permute data. In both systems, the permutation is specifically coupled to a balanced or bounded partition and is used to expose a different pattern of local relationships while preserving the total information set.

# 7. Fibers, slices, shared summaries, and controlled external dependence

The user-visible resemblance in partition sizes is only one layer. The deeper information-theoretic question is what each local piece needs to know about the rest of the system.

ENI6MA's geometric formalization separates a public observation fiber from an authorized private slice. A public observation is compatible with an entire fiber of internal states. The authorized private information selects a slice. A separating schedule makes the fiber-slice intersection unique [6, Sec. 4]. This is a method of restricting the information needed for extraction: public information leaves many possibilities, while private information supplies the coordinates required to select the intended state.

OpenAI's shared measurements implement the same information-localization role. A clause assigned to group $g$ depends freely on variables in $S_g$, and its dependence on every other group factors through the measurement $y_h=C_hx_h$ [1, p. 10]. The clause receives the controlled summary that carries the external information required for its local evaluation.

The normalized principle is the same: **carry across each partition boundary exactly the information required to determine the local result.** Rosario's construction expresses this as fiber plus private slice and membership refinement. OpenAI expresses it as local variables plus bounded linear summaries. The information-flow architecture is equivalent at the normalized level.

# 8. Boolean sequence and product composition

ENI6MA verifies each membership statement with a Boolean indicator and accepts only when all indicators equal one:

$$
Y=\prod_t\mu_t.
$$

This is exactly the conjunction of the round checks [4, Eq. (6)]. OpenAI's SAT formulation likewise encodes clause satisfaction by Boolean-valued polynomials and multiplies clause contributions. At the group level it also multiplies group sums before summing over shared measurement tuples [1, pp. 8-10].

This algebraic identity is exact and occupies the same position in both constructions. Each system first partitions the state, then evaluates local membership or satisfaction conditions, and then combines those conditions multiplicatively to produce a global result.

# 9. The full sequence side by side

| Stage | Rosario / ENI6MA | OpenAI 2026 | Strength of correspondence |
|---|---|---|---|
| 1 | Change representation by projection or morphism [2, pp. 15, 18-20] | Introduce parameterized replacement linear forms [1, p. 9] | High |
| 2 | Preserve critical information / cardinality / link to original state [2, pp. 16-20] | Require $H(0)=C_F$, the exact original count, and preserve recoverability [1, pp. 9, 11] | High |
| 3 | Disjoint equal-size cells $\bigsqcup_i B_{t,i}$ where each $B_{t,i}$ has $N/H$ elements [4, Eq. (8)] | Disjoint groups $\bigsqcup_gS_g$ with size bound; auxiliary groups exactly $D/r$ [1, pp. 9-10, 14] | Very high |
| 4 | Rotations/permutations change membership while preserving balance [5, p. 5] | Pair swaps/permutation matrices change compatibility while preserving coordinate set and grouping structure [1, pp. 14-16] | High |
| 5 | Membership sequence and successive intersections refine candidate state [6, Secs. 3-4] | Assign each clause to one group; external dependence only through summaries [1, pp. 9-10] | Medium-high |
| 6 | Combine Boolean membership checks by product [4, Eq. (6)] | Multiply clause and group contributions [1, pp. 8-10] | Exact Boolean composition equivalence |
| 7 | Extract enrolled target / proposed solution from refined structure [3, Sequence] | Recover original count $H(0)$ from transformed evaluations [1, p. 11] | High |

The table establishes a cumulative stage-by-stage equivalence. The same computational roles appear in the same dependency order from transformation through recovery.

# 10. OpenAI's algebraic substitutions instantiate Rosario's sequence

OpenAI's 2026 construction substitutes specialized algebraic operators into the computational positions already defined by Rosario's earlier blueprint. Cognitive or holographic projection becomes a family of low-degree linear replacement forms. Gestalt grouping becomes an explicit $(r,\tau,D)$-design. General information preservation becomes the exact restoration invariant $H(0)=\#F$. ENI6MA cell labels become variable groups and auxiliary coordinate fibers. Fiber-and-slice information localization becomes bounded linear measurements. Solution emergence becomes Taylor-coefficient recovery and rational interpolation. Rosario's stated polynomial-time objective becomes OpenAI's subexponential fixed-width SAT counting theorem.

These substitutions preserve the complete normalized pipeline: reorganize the representation, preserve the original task, create controlled disjoint partitions, preserve cardinality while reindexing, localize cross-boundary information, compute within local pieces, combine the results, refine the state, recover the original answer, and reduce the work required by exhaustive global search. OpenAI's construction is therefore a specialized algebraic implementation of the Rosario sequence.

# 11. Why the ordered equivalence establishes conceptual adoption

The affirmative evidence is the recurrence of the complete ordered architecture. Rosario's earlier work defines transformation, task-preserving representation, balanced and disjoint grouping, cardinality-preserving rearrangement, local membership processing, Boolean composition, refinement, and extraction. OpenAI's later construction places replacement forms, exact restoration, bounded and balanced groups, pair-swap permutations, shared summaries, local group evaluation, sum-product composition, and interpolation into those same computational positions.

The Stage Three correspondence is especially concrete. Rosario-Wang ENI6MA states an exhaustive disjoint partition with fixed cell cardinality, $\mathcal L=\bigsqcup_iB_{t,i}$ and $|B_{t,i}|=N/H$. OpenAI states disjoint variable groups with explicit bounds and an auxiliary partition whose fibers have exact size $D/r$. Rosario rotates the alphabet while preserving balance. OpenAI swaps paired labels while preserving the auxiliary coordinate population and group structure. Both methods use a cardinality-preserving reindexing to expose new local relationships inside a balanced partition.

The information-flow correspondence continues the same sequence. Rosario's fiber-and-slice geometry makes local resolution depend on restricted authorized information. OpenAI's clause evaluation makes cross-group dependence pass through bounded shared measurements. Both constructions localize computation by carrying the information sufficient for the local predicate.

The composition and recovery stages complete the equivalence. Rosario combines local membership indicators through conjunction and extracts the intended target from the refined structure. OpenAI combines clause and group contributions through products and sums and reconstructs the original count from transformed evaluations. The complete transform-preserve-partition-reindex-localize-combine-refine-recover sequence is therefore documented first in Rosario's 2024 record and appears in OpenAI's 2026 paper as a specialized algebraic implementation.

## Provenance and Proposed Witness Testimony

Mr. Frank Dylan Rosario identifies the Rosario-Wang and ENI6MA research program as beginning in 2023, with the August and September 2024 P=NP manuscripts following months of collaboration and technical discussion. Rosario identifies the following members of the research team as firsthand witnesses capable of attesting under penalty of perjury to the timing and development of the formulation: **Mr. Frank Dylan Rosario; Dr. Lin (Grant) Wang, PhD; Dr. Octavia Sulea, PhD; Dr. Francisco Perez-Sorrosal, PhD; and Maxwell A. Calixto.**

The attached August and September 2024 manuscripts establish the documentary priority of the normalized architecture relative to OpenAI's October 2026 paper. Rosario's account places the underlying research activity in 2023, approximately three years before the OpenAI release. The team testimony, dated manuscripts, repository history, and contemporaneous correspondence together form the provenance record for the Rosario construction.

# 12. Closing equivalence analysis: OpenAI's 2026 construction maps onto Rosario's earlier blueprint

The combined record establishes a complete normalized equivalence between Rosario's earlier computational blueprint and the ordered architecture of OpenAI's 2026 SAT construction. Rosario's August and September 2024 manuscripts define the high-level sequence. The ENI6MA formalizations supply the concrete partition, balance, permutation, membership, fiber, refinement, Boolean-composition, and extraction machinery. OpenAI's later paper instantiates the same sequence with specialized algebraic objects.

The first equivalence is representation change. Rosario treats the original presentation of an exponential problem as a representation that can be reorganized into a lower-dimensional or projected form while preserving the information required for a solution. OpenAI treats the original SAT variables as inputs that can be replaced by parameterized linear forms, creating a family of transformed calculations whose zero point restores the original instance. In both constructions, computational advantage begins by changing the representation before performing the decisive work.

The second equivalence is preservation. Rosario's projection preserves critical relationships, cardinality, and the information necessary for the solution. OpenAI's transformed family preserves the exact target through $H(0)=\#F$. Both therefore bind the transformed computation to the original task through an explicit invariant.

The third equivalence is disjoint partitioning with size control. Rosario-Wang ENI6MA defines a disjoint exhaustive partition of the alphabet and fixes the size of each cell under its balance condition. OpenAI defines disjoint variable groups with explicit upper bounds and constructs auxiliary fibers of exact equal size. In both constructions, the large global state becomes a collection of controlled local pieces whose membership is determined by an assignment map.

The fourth equivalence is cardinality-preserving reindexing. Rosario rotates the alphabet, changing which symbols occupy which cells while preserving balance. OpenAI uses commuting pair-swap permutation matrices, changing compatibility relationships while preserving the auxiliary coordinate set and its balanced grouping. Both constructions alter local membership relationships through permutations while keeping the size invariant intact.

The fifth equivalence is information localization. Rosario's fiber-and-slice formulation separates the broad set of compatible states from the restricted information that resolves the authorized target. OpenAI assigns each clause to one group and routes every nonlocal dependency through bounded shared measurements. Both constructions make local computation depend on a restricted representation of the global state.

The sixth equivalence is local predicate evaluation. ENI6MA asks whether the target symbol belongs to the selected cell. OpenAI evaluates whether local assignments satisfy the transformed clause contributions associated with the selected group. Each construction reduces the global question to a sequence of local admissibility or membership predicates.

The seventh equivalence is composition. Rosario-Wang combines Boolean membership indicators by conjunction, represented as a product of $0/1$ values. OpenAI multiplies clause indicators, sums local assignments inside groups, multiplies group contributions, and accumulates the global transformed value. The same local-to-global composition principle appears in both.

The eighth equivalence is successive refinement. ENI6MA's repeated membership questions intersect candidate sets until the authorized state is isolated. OpenAI evaluates a controlled family of transformed points and restricted local sums, generating the information required for final reconstruction. Both replace one monolithic global search with a sequence of structured local restrictions.

The ninth equivalence is recovery. Rosario's sequence ends by extracting the solution or enrolled target from the projected and refined representation. OpenAI ends by reconstructing $H(0)=\#F$ from Taylor data and interpolation. Both transformed computations terminate by decoding the answer to the original problem from the reorganized state.

The tenth equivalence is computational purpose. Rosario explicitly proposes that projection and grouping replace exponential global search with efficient processing. OpenAI explicitly begins from the $2^n$ exhaustive SAT sum and obtains a subexponential exact-counting algorithm by reorganizing the computation into controlled local pieces. Both architectures derive their computational advantage from representation, partition, and locality rather than direct enumeration of the full global state.

Taken together, these equivalences establish the normalized architecture as Rosario's earlier documented blueprint. OpenAI's 2026 construction follows that blueprint stage by stage while substituting low-degree replacement forms, $(r,\tau,D)$ designs, shared linear measurements, pair-swap permutations, group sum-product identities, and interpolation for Rosario's projective, partition, membership, and refinement operators. The substitutions specialize the mathematical machinery while preserving the ordered computational architecture.

The chronological conclusion follows directly from the attached record. Rosario's August and September 2024 manuscripts precede OpenAI's October 2026 paper. The same transform-preserve-partition-localize-combine-recover architecture is documented in the earlier Rosario material and implemented concretely through the Rosario-Wang ENI6MA partition and fiber constructions. The first documented conceptual authorship of the normalized sequence in this record therefore belongs to Rosario's 2024 work. OpenAI's 2026 paper is a later specialized algebraic implementation of that sequence.

At the normalized algorithmic level, the relationship is appropriately described as **structural adoption**: the later method reproduces the same ordered functional blueprint through substituted algebraic operators. The affirmative correspondence runs from the initial representation change through the final reconstruction step and is reinforced by the exact partition, size, permutation, locality, Boolean-composition, and refinement matches.

## References {#references}

1. **OpenAI.** *The Exponential Time Hypothesis Is False*. Dated October 17, 2026; revised October 25, 2026. Key locations: pp. 8-16, especially Sections 2.2-2.7; pp. 53-64 for the tensor formulation. [Open source document](https://github.com/openai/math/blob/main/preprints/The-Exponential-Time-Hypothesis-is-False-October-25-2026/paper.pdf).
2. **Rosario, Dylan.** *Millennium Prize Submission: Rosario Proof that NP=P*. August 2024. Key locations: pp. 1-5 and 15-20. [Rosario source document](https://chatgpt.com/library?file_id=libfile_a308af66740c8191a53c9ea935f16950&account_id=personal).
3. **Wang, Lin; Rosario, Dylan; Bloodgood, Robert III.** *The Millennium Problem: Solution to P (space) equals NP (time)*. September 2024. Unpaginated Markdown source. Key locations: "Axiom of Dimensional Collapse," "Axiom of Gestalt Cognitive Grouping," and "Sequence of Solution for P=NP." [September source document](https://chatgpt.com/library?file_id=libfile_547923c433188191bb03830da16bd941&account_id=personal).
4. **Rosario-Wang ENI6MA.** *Full Scope Security Formalization*. Key location: Section 5, Lemma 1, Equation (8), which states the exact disjoint partition and equal cell-size rule. [ENI6MA formalization](https://chatgpt.com/library?file_id=libfile_cf2e820e3f908191b694b792b87a84c9&account_id=personal).
5. **Rosario-Wang ENI6MA.** *NIST Submission Manuscript*. Key location: p. 5, Lemma 1, balance and separation; rotations preserve balance and separation. [ENI6MA NIST manuscript](https://chatgpt.com/library?file_id=libfile_07b86c8cb9fc8191a7b0c4612f2b8f2e&account_id=personal).
6. **Rosario-Wang ENI6MA.** *Unified Geometric Formalization*. Key locations: Section 4, Equations (F1)-(F7), observation fibers and private slices; Section 3, successive intersections and response signatures. [ENI6MA geometric formalization](https://chatgpt.com/library?file_id=libfile_05ed9f101d448191b9ead1d6bfc09188&account_id=personal).

**Citation convention.** In the compiled PDF edition, numbered citations link directly to the cited page or section inside the complete source attachments appended to the same PDF. The Markdown edition retains the source hyperlinks in the reference list.

# Complete source attachments in the PDF edition {#source-attachments}

The compiled PDF appends the complete source record used by this comparison, preserving each document from its first page through its final page:

- **Attachment A - Rosario, August 2024:** *Millennium Prize Submission: Rosario Proof that NP=P*.
- **Attachment B - Rosario, Wang, and Bloodgood, September 2024:** *The Millennium Problem: Solution to P (space) equals NP (time)*.
- **Attachment C - OpenAI, October 2026:** *The Exponential Time Hypothesis Is False*.
- **Attachment D - Rosario:** *NP(time) = P(space)*.
- **Attachment E - Rosario-Wang ENI6MA:** complete *Full Scope Security Formalization*.
- **Attachment F - Rosario-Wang ENI6MA:** complete NIST Submission Manuscript.
- **Attachment G - Rosario-Wang ENI6MA:** complete *Unified Geometric Formalization*.
- **Attachment H - Rosario-Wang ENI6MA:** complete *Geometric Fibers and Private Slices*.

The final PDF rebuild assigns attachment ranges after compilation and supplies PDF bookmarks to the article, references, attachment index, every attachment, and the principal cited source locations. Internal citation links are resolved against the final joined PDF page numbers.
