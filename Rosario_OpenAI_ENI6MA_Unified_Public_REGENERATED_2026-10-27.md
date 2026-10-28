---
title: "Rosario's Computational Blueprint and OpenAI's 2026 SAT Method: A Unified Public Comparison"
author: "Public comparative article"
date: "October 27, 2026"
---

## A unified comparison from representation change through final reconstruction

## Normalized adoption map: the OpenAI 2026 features that map directly to Rosario's construction

The term **adopted** in this article identifies the functional and architectural equivalence between the later OpenAI method and the ordered computational roles already defined in Rosario's earlier framework and the Rosario-Wang ENI6MA construction. The comparison establishes adoption at the normalized algorithmic level by matching each operation, invariant, partition rule, information-flow rule, composition step, and recovery stage.

1. **Replace exhaustive global search with structural reorganization.** Rosario's 2024 framework proposes changing the problem representation so the solver replaces full exponential enumeration with structured processing [2, pp. 15-20] [3, Sequence]. OpenAI begins from a $2^n$ global SAT sum and explicitly seeks a structure that avoids evaluating all $2^n$ assignments [1, p. 8].

2. **Transform the original representation before solving it.** Rosario maps higher-dimensional information $I_H$ into a projected representation $I_L=P(I_H)$ [2, pp. 18-20]. OpenAI replaces original variable occurrences by parameterized linear forms and evaluates the resulting family at selected points [1, p. 9].

3. **Preserve a route back to the original task.** Rosario requires the transformed representation to retain the information and relationships needed for the solution [2, pp. 15-20]. OpenAI requires the transformed family to satisfy $H(0)=C_F$ (where $C_F$ is the exact count of satisfying assignments of the original formula, which OpenAI writes with a hash sign), so the original exact count remains recoverable [1, p. 9].

4. **Partition the transformed state into disjoint local pieces.** Rosario-Wang ENI6MA uses an exhaustive disjoint partition $\mathcal L=\bigsqcup_iB_{t,i}$ [4, Eq. (8)]. OpenAI uses $[n]=S_1\sqcup\cdots\sqcup S_r$ and, in its auxiliary construction, $B=\bigsqcup_gS_{t,g}$ [1, pp. 9-10, 14].

5. **Impose explicit group-size guarantees.** ENI6MA gives $|B_{t,i}|=N/H$ under its balance condition [4, Eq. (8)], and its concrete NIST profile places exactly three keys in each cell [5, p. 5]. OpenAI bounds $|S_g|\le 2n/r$ and constructs auxiliary groups of exact size $D/r$ [1, pp. 9-10, 14].

6. **Give every relevant object one local home in the current partition.** In ENI6MA every symbol belongs to exactly one cell in each frame [4, Eq. (8)]. OpenAI places each variable in one disjoint group and assigns every clause to one group $\sigma_e(t)$ [1, pp. 9-10].

7. **Reindex the state by cardinality-preserving permutations.** Rosario-Wang rotations change symbol-to-cell membership while preserving balance and separation [5, p. 5]. OpenAI uses commuting pair-swap permutation matrices to change compatibility relations while preserving the auxiliary coordinate set [1, pp. 14-16].

8. **Restrict what information must cross a partition boundary.** Rosario's projected representation is intended to retain only the information required for the task, and ENI6MA's fiber-and-slice geometry separates public ambiguity from authorized resolving information [2, pp. 15-17] [6, Sec. 4]. OpenAI lets a clause depend freely on its own group but requires dependence on other groups to pass through bounded shared measurements $y_h=C_hx_h$ [1, pp. 9-10].

9. **Perform the substantive work locally after the partition is fixed.** ENI6MA evaluates cell membership and refines candidate states through the resulting local membership information [4, Eq. (6)] [6, Secs. 3-4]. OpenAI computes each transformed clause and each group contribution using its assigned group plus the fixed shared summaries [1, p. 10].

10. **Combine local results into a global result.** Rosario-Wang combines per-round membership indicators into a complete acceptance relation, $Y=\prod_t\mu_t$ [4, Eq. (6)]. OpenAI sums local assignments within each group, multiplies the group sums, and accumulates the global transformed value [1, p. 10].

11. **Use successive refinement rather than one monolithic search.** ENI6MA successively intersects the candidate set with the cell selected at each round, producing a refinement path toward the target [6, Sec. 3]. OpenAI evaluates a controlled family of transformed points and restricted local sums through the transformed local enumeration [1, pp. 9-12].

12. **Recover the answer to the original problem from the reorganized representation.** Rosario's 2024 sequence ends with solution extraction from the projected and grouped space [3, Sequence], while ENI6MA's separating schedule identifies the target through the final intersection [6, Sec. 4]. OpenAI reconstructs $H(0)=C_F$ from transformed evaluations by Taylor data and interpolation [1, p. 11].

13. **Use the reorganization to reduce the cost of an exponential problem.** Rosario's stated objective is to replace exhaustive exponential search by efficient computation through projection and grouping [3, Sequence]. OpenAI proves a narrower but concrete subexponential improvement for fixed-width SAT counting [1, Theorem 1.1].

Taken together, these thirteen affirmative correspondences form one dependency chain: **transform -> preserve -> partition -> balance -> reindex -> localize information -> compute locally -> combine -> refine -> recover -> reduce search cost.** That ordered chain is the central subject of the comparison.

## Why this comparison should be read as one complete sequence

Rosario's work and OpenAI's 2026 SAT paper should be compared from the beginning as two complete computational architectures. The central equivalence is the recurrence of the same computational roles in the same order. Rosario changes the representation, preserves the information needed to get back to the original task, divides the transformed state into controlled pieces, changes memberships through size-preserving rearrangements, processes local membership or group information, combines those local results, and extracts the answer from the reorganized structure. OpenAI does the same kinds of operations with more specialized algebraic machinery.

The Rosario-Wang ENI6MA construction is important because it makes the partition stage exact. Its cells are disjoint, collectively exhaustive, and balanced under the stated conditions. Its rotations preserve those size guarantees while changing membership. Its fiber-and-slice formulation separates global ambiguity from the resolving information needed locally. Its verification combines local membership results into a complete decision. Those are concrete implementations of the same representation-and-grouping blueprint that Rosario's 2024 P=NP manuscripts state at a higher level.

OpenAI's later algorithm replaces Rosario's vocabulary with replacement linear forms, bounded variable groups, one clause assignment per group, shared linear measurements, pair-swap permutations, local sums and products, and interpolation. Those mechanisms instantiate the same ordered architecture. At the functional level, the later paper can therefore be read as a specialized algebraic implementation of the same sequence.

# 1. Rosario's construction in one normalized statement

Strip away the names and describe ENI6MA as information processing. There is a finite alphabet $\mathcal L$ with $N$ symbols. Each round divides that alphabet into $H$ disjoint cells:

$$
\mathcal L=\bigsqcup_{i=0}^{H-1}B_{t,i}.
$$

When the sizes divide evenly, every cell contains exactly

$$
|B_{t,i}|=N/H
$$

symbols [4, Eq. (8)]. A rotation changes which symbol belongs to which cell while preserving how many symbols are in each cell [5, p. 5].

The user or verifier processes the alphabet through its partitioned membership structure. A target symbol is identified by the sequence of cells containing it. Each round contributes a membership statement. The complete decision is the conjunction of those membership statements:

$$
Y=\prod_{t=1}^T\mu_t,\qquad \mu_t\in\{0,1\}.
$$

For Boolean values, the product equals one only if every test is true [4, Eq. (6)]. The geometric formulation describes the same process as refinement: the observation determines a fiber, authorized information determines a slice, and the successive membership conditions narrow the state to the enrolled target [6, Sec. 4].

In plain English, Rosario's construction says:

1. reorganize the full state;
2. divide it into controlled disjoint pieces;
3. guarantee the size of those pieces;
4. rotate or permute the state to expose different membership relations;
5. record the local membership information;
6. combine the local checks;
7. recover the unique intended state.

That is a partition-and-refinement algorithm.

# 2. Rosario's 2024 P=NP sequence

The August 2024 paper already frames computational difficulty as a problem of representation. It proposes transforming higher-dimensional information into a reduced representation while preserving what is necessary for the solution. It then introduces emergent groupings and says the reorganization can reveal latent structure [2, pp. 15-20].

The September manuscript states the sequence directly. First project the NP-complete problem while retaining critical relationships. Then group the projected information. Then obtain the solution by using the projected grouping through structured local processing [3, Sequence].

The normalized 2024 sequence is therefore:

$$
\boxed{\text{transform}\to\text{preserve}\to\text{group}\to\text{solve}}.
$$

The ENI6MA construction supplies the combinatorial details: the groups can be actual disjoint cells, the cells can be balanced, rotations can preserve their cardinalities, and multiple membership answers can refine the candidate state.

# 3. OpenAI's Stage Three says almost the same thing in algebraic language

OpenAI begins with a SAT counting expression containing $2^n$ assignments and expressly says that direct evaluation would be exhaustive search [1, p. 8]. It first imagines an easy case: if the variables could be partitioned into groups with no clause crossing group boundaries, the groups could be counted separately and combined. That would be far cheaper than the global $2^n$ search.

OpenAI changes the formula representation to create this convenient structure. It replaces original variables with parameterized linear forms. At $T=0$ the original variables return, so the target answer is preserved as $H(0)=C_F$ [1, p. 9].

Then comes Stage Three.

::: {.openai-box}
### OpenAI formulation

OpenAI requires a disjoint partition

$$
[n]=S_1\sqcup\cdots\sqcup S_r
$$

with

$$
|S_g|\le 2n/r.
$$

Each clause is assigned to one group $\sigma_e(t)$. Each group has a small collection of linear measurements. A clause can depend freely on its own group, while its dependence on another group must pass through those measurements [1, pp. 9-10].

In the auxiliary construction, the groups become exactly balanced: the sets $S_{t,g}$ partition $B$ and contain exactly $D/r$ coordinates each. OpenAI then uses swap permutations on ordered pairs to change the compatibility pattern while retaining the structured partition [1, pp. 14-16].
:::

Normalized, OpenAI's method says:

1. reorganize the original SAT state;
2. divide the transformed state into controlled disjoint pieces;
3. guarantee the size of those pieces;
4. use permutations to change the relationship pattern;
5. let each local piece receive only limited information about the others;
6. compute local results;
7. combine them and recover the original answer.

That is why the comparison is much stronger than "both use groups."

# 4. The direct partition correlation

Put the two rules next to each other.

**Rosario-Wang ENI6MA:**

$$
\mathcal L=\bigsqcup_iB_{t,i},\qquad |B_{t,i}|=N/H.
$$

**OpenAI:**

$$
[n]=\bigsqcup_gS_g,\qquad |S_g|\le 2n/r,
$$

and, in the auxiliary coordinate space,

$$
B=\bigsqcup_gS_{t,g},\qquad |S_{t,g}|=D/r.
$$

Rosario partitions alphabet symbols or candidate targets, and OpenAI partitions variables and auxiliary coordinates. At the normalized computational level, both constructions assign the same role to those partitions. A large global state is converted into nonoverlapping local pieces whose sizes are explicitly controlled. Those pieces then become the units of computation.

OpenAI adds clause assignment. Every clause has a local group. Rosario's system gives every target symbol exactly one cell per round. The organizing rule is the same: every object has one local home in the current partition.

The correspondence becomes stronger when rotation and swapping are added. ENI6MA rotates the symbol arrangement but preserves balance. OpenAI swaps the entries of pair labels but preserves the coordinate system and uses the changed orientations to control which dependencies survive. Both are cardinality-preserving rearrangements applied to a partitioned state.

# 5. Fibers and shared measurements

Rosario's fiber-and-slice construction explains why the partitions are useful. Public information alone leaves a fiber of possible states. Authorized private information identifies a slice. Their intersection, together with a separating schedule, identifies the target [6, Sec. 4]. The full state is never treated as one public flat list. Information is intentionally separated according to what each observer or stage needs.

OpenAI uses the same normalized information-flow restriction. A clause assigned to group $g$ receives cross-group information through a bounded summary. The dependence on another group has to pass through a summary $y_h=C_hx_h$ [1, p. 10]. Once the summaries are fixed, OpenAI can process the group locally.

This is the same normalized design principle: **localize the work and carry only the information that must cross the partition boundary.**

# 6. The Boolean sequence

ENI6MA's acceptance relation is a sequence of membership tests combined by multiplication. OpenAI's SAT representation also uses Boolean satisfaction values whose product represents simultaneous satisfaction, and its grouped computation multiplies local group contributions.

The identity itself is ordinary:

$$
b_1\land b_2\land\cdots\land b_m=\prod_{i=1}^mb_i\qquad(b_i\in\{0,1\}).
$$

The Boolean product occupies the same position in both constructions. In each system it comes **after** partitioning and local evaluation and restores a global yes/no or counting relation from local pieces. Its position inside the complete sequence reinforces the normalized equivalence.

# 7. OpenAI's substitutions within Rosario's sequence

OpenAI's later paper reproduces Rosario's ordered functional blueprint through specialized algebraic machinery. Rosario's dimensional collapse becomes low-degree replacement linear forms. Rosario's cells and emergent groupings become an $(r,\tau,D)$-design. Rosario's information-retention requirement becomes $H(0)=C_F$ together with bounded shared measurements. Rosario's rotations and alphabet transformations map onto pair labels and swap matrices. Rosario's extraction objective maps onto exact interpolation from Taylor data.

These substitutions preserve the same sequence from beginning to end. The later method follows Rosario's route to computational advantage: transform the representation, preserve the original task, partition the transformed state, preserve group-size structure while reindexing, localize external information, compute within local pieces, combine the contributions, and reconstruct the original answer. OpenAI's fixed-width SAT result is therefore a specialized algebraic implementation of the Rosario blueprint.

The computational objective remains the reduction of exhaustive global work. Rosario's 2024 program targets polynomial time and $P=NP$. OpenAI's 2026 implementation reaches a subexponential fixed-width SAT counting bound through the same normalized architecture.

## Provenance and Proposed Witness Testimony

According to Mr. Frank Dylan Rosario, the underlying Rosario-Wang and ENI6MA research program began in 2023 and the August and September 2024 P=NP manuscripts followed months of collaboration and technical discussion. Rosario states that the following members of the research team can attest, under penalty of perjury if asked to execute sworn declarations, to the timing and development of the formulation: **Mr. Frank Dylan Rosario; Dr. Lin (Grant) Wang, PhD; Dr. Octavia Sulea, PhD; Dr. Francisco Perez-Sorrosal, PhD; and Maxwell A. Calixto.**

Rosario identifies those individuals as firsthand witnesses capable of attesting under penalty of perjury to the timing and development of the formulation. The attached August and September 2024 manuscripts establish documentary priority approximately two years before the October 2026 OpenAI paper, while Rosario places the start of the underlying research program in 2023, approximately three years before the OpenAI release. The dated manuscripts, repository history, correspondence, and team declarations form the provenance record.


# Closing equivalence analysis

The full comparison yields one continuous affirmative map. Rosario changes the representation; OpenAI changes the representation. Rosario preserves the information required to return to the original task; OpenAI preserves the original count as $H(0)$. Rosario divides the reorganized state into disjoint controlled cells; OpenAI divides variables and auxiliary coordinates into disjoint controlled groups. Rosario preserves cell cardinalities while rotations change symbol membership; OpenAI preserves the auxiliary coordinate population while pair swaps change group compatibility. Rosario localizes the relevant information through fibers, slices, and membership signatures; OpenAI localizes nonlocal clause dependence through bounded shared measurements. Rosario combines local Boolean membership checks into a global decision; OpenAI combines local clause and group contributions into the global transformed count. Rosario extracts the intended target from the refined representation; OpenAI reconstructs the original count from transformed evaluations.

The ENI6MA Stage Three mechanics make the adoption especially concrete. The Rosario-Wang construction states that the alphabet is a disjoint union of cells and that every cell has a prescribed size. Its rotations preserve balance while changing membership. OpenAI later constructs disjoint variable groups with explicit bounds and auxiliary fibers of exact equal size, then uses pair-swap permutations to alter group compatibility while preserving the coordinate system. In normalized form, both use the same device: maintain a fixed total state, partition it into bounded local pieces, reindex the members through cardinality-preserving permutations, and use the resulting local structure to reduce the cost of the next computation.

The fibers and shared measurements provide the same information-localization rule. Rosario's observation fiber represents the globally compatible states, while the authorized slice supplies the resolving information. OpenAI's assigned group contains the full local variables, while shared measurements carry the required information from the other groups. Both systems preserve sufficient information for the local predicate while replacing the full global state with a controlled local representation.

The sequence converges again at composition and recovery. Rosario combines membership predicates across rounds and extracts the target from the refined structure. OpenAI multiplies and sums local contributions and reconstructs the original global count. The correspondence therefore runs continuously from the first transformation to the final recovery stage.

Rosario's dated August and September 2024 manuscripts place the normalized transform-preserve-group-solve blueprint in the record two years before OpenAI's October 2026 paper. The ENI6MA construction supplies the exact disjoint partition, balance, rotation, membership, fiber, refinement, and Boolean-composition mechanics that map directly onto OpenAI's later partition, permutation, shared-measurement, local-evaluation, composition, and recovery stages. Rosario's account places the underlying research program in 2023, with the 2024 manuscripts following months of collaboration.

The affirmative conclusion is that the normalized architecture originates in Rosario's earlier documented work and appears in OpenAI's 2026 paper as a specialized algebraic implementation. The later paper substitutes low-degree replacement forms, shared measurements, pair-swap permutations, group sum-product identities, and interpolation for Rosario's projective, partition, membership, and refinement operators while preserving the same ordered computational blueprint. At the algorithmic level, this is structural adoption of Rosario's sequence.

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
