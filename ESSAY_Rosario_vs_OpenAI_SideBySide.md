# Side by Side: The Rosario and Rosario-Wang Construction and OpenAI's "The Exponential Time Hypothesis Is False"

**An essay setting the two formulations next to each other, step by step**

*Prepared 27 October 2026 for the public evidence repository ROSARIO-OPENAI. This is a statement of Rosario's position together with an account of what the documentary record does and does not support. It is not a legal finding, and it does not assert that any party copied any other.*

---

## 1. Thesis

Rosario's position is that the October 2026 OpenAI paper "The Exponential Time Hypothesis Is False" follows, role by role and in a recognizable order, the architecture of the Rosario and Rosario-Wang construction: change the representation, preserve a route back to the original task, partition the state into disjoint equal-sized pieces, keep size-preserving rearrangements, confine cross-piece information to a bounded interface, compute locally, combine by product, and recover a distinguished value.

This essay lays each step of Rosario's construction beside the corresponding OpenAI step, quotes or cites both, and states for each pair what is identical and what is only analogous. The comparison supports a precise and limited conclusion. The two works share a common functional skeleton, and in several places they share the same notation and the same size condition. The matches are real, but individually they are of low to moderate distinctiveness, because the skeleton is also the skeleton of published algorithms that OpenAI itself cites. The record read for this essay contains no shared constants, no shared errors, and no shared specialized terminology. Section 8 states what additional evidence would be needed to move from "closely parallel" to a showing that excludes independent derivation.

## 2. Sources, dates, and how every equation is cited

Every equation in Sections 3 and 4 is copied from the source text read for this essay, or is marked as a normalized paraphrase. Page numbers for OpenAI are the paper's own page numbers. Rosario references use the printed page, section or equation number of the document named.

| Label | Document | Date shown in the document | Content |
|---|---|---|---|
| R-Aug | "Millennium Prize Submission: Rosario Proof that NP=P" (20 pp.) | August 2024 | Holographic Morphism Principle, Dimensional Collapse, Emergent Groupings, entropy conservation. Conceptual, no SAT algorithm. |
| R-Sep | "The Millennium Problem: Solution to P (space) equals NP (time)" (Attachment B of the compiled edition, pp. B-1 to B-80) | September 2024 | NP-Time Gestalt Algorithm, "Sequence of Solution for P=NP" (p. B-79). Conceptual, no SAT algorithm. |
| E-Sec | "Rosario-Wang ENI6MA Full Scope Security Formalization" (Attachment E) | "Prepared 12 September 2026 from the supplied drafts" | Rings, rotations, cells, release masks. The document counts 72 numbered equations, 7 numbered lemmas and further theorems. |
| E-NIST | "Rosario-Wang ENI6MA: A Proposed Membership-Response Primitive" (Attachment F), submission manuscript v1.0 | 16 September 2026 | Twelve-key profile, Lemma 1 on balance and separation, rotation by nonce. |
| E-Geo | "ENI6MA Unified Geometric Formalization" (Attachment G) | 13 September 2026 | Axiom A1, fibers and slices, Eqs. (F1) to (F7), Theorem 2. |
| OAI | "The Exponential Time Hypothesis Is False," OpenAI (67 pp.) | 17 October 2026, revised 25 October 2026 (as reported by OpenAI's repository and press accounts) | Deterministic exact counting of satisfying assignments of k-CNF formulas in subexponential time. |

Two facts about this table bear directly on how far the comparison can go, and they are stated here at the outset rather than buried.

First, the August and September 2024 manuscripts describe a cognitive and geometric framework in words and in a handful of schematic formulas. They contain no clause, no formula over Boolean variables, no interpolation, no polynomial, and no counting procedure. The precise combinatorial mechanics (disjoint cells, equal sizes, rotations, products of membership indicators) appear in the ENI6MA documents, and those carry dates in September 2026, about five weeks before OpenAI's paper. Rosario's account, recorded in the repository, is that the ENI6MA research program began in 2023 and that the 2024 manuscripts followed months of collaboration. That account is his testimony. The dated documents in the record do not by themselves carry the ENI6MA mechanics back to 2024 or 2023.

Second, the ENI6MA documents are cryptographic. They construct a membership-response authentication primitive. They do not count anything and they do not address satisfiability.

## 3. Rosario's construction, step by step

The construction is presented in the order in which the repository's normalized map lists it. Each step gives the plain statement first and the cited equation second.

### Step R1. Replace one monolithic object by a family of sub-objects

R-Aug describes the Holographic Morphism Principle as a map from a higher-dimensional informational space $\mathcal I_H$ to a lower-dimensional projection $\mathcal I_L$, expressed as a sum of component projections (R-Aug, abstract, p. 2):

$$
\mathcal P(\mathcal I_H)=\sum_{j=1}^{m}\mathcal P_j(\mathcal I_H),\qquad m<n.
$$

The same page states emergent groupings by the equation

$$
\mathcal G_k=\sum_{j=1}^{m}\mathcal P_j(\mathcal I_{H,j}),
$$

where $k$ is the number of emergent groupings. R-Sep restates the idea as the first step of its sequence: project the NP-complete problem from $\mathbb R^d$ to $\mathbb R^n$ with $d>n$ while keeping proximity relationships, written $d_{proj}(f(x_i),f(x_j))\approx d(x_i,x_j)$ (R-Sep, p. B-79, Step 1).

### Step R2. Preserve a route back to the original task

R-Aug states that "the conservation of informational entropy during this collapse, denoted by $S_H(\mathcal I_H)=S_L(\mathcal I_L)$, ensures that no critical information is lost in the transformation" (R-Aug, p. 2). The corresponding equation is

$$
S_H(\mathcal I_H)=S_L(\mathcal I_L).
$$

R-Aug also states an emergent solution pathways map $\mathcal E_P:\mathcal S_{NP}\to\mathcal S_P$ (R-Aug, p. 2).

### Step R3. Partition the state into disjoint, equal-sized cells

E-Sec constructs, for each round $t$, a partition of the master alphabet $\mathcal L$ into $H$ cells $B_{t,i}$ by rotating each ring by an offset and cutting it into $H$ equal consecutive pieces (E-Sec, Sec. 4, Eq. (3)). Its Lemma 1 states the resulting partition and the size of each cell (E-Sec, Sec. 5, Eq. (8)):

$$
\mathcal L=\bigsqcup_{i=0}^{H-1}B_{t,i},\qquad |B_{t,i}|=q=N/H.
$$

E-NIST gives a concrete case: "Each coordinate partition places exactly three displayed keys in every cell, and the ordered pair of answers identifies every key uniquely" (E-NIST, Sec. 3.1, Lemma 1). R-Aug's verbal counterpart is the principle of "preserving cardinality" (R-Aug, p. 2) and the treatment of morphisms applied to "cardinally equal alphabets (alphabets with the same number of elements)" (R-Aug, pp. 15 to 17). The word "partition" does not occur in R-Aug or in the September 2024 manuscript of Attachment D.

### Step R4. Rearrange by size-preserving permutations

E-Sec rotates each ring by an independent uniform offset $o_{j,t}$ in every round (E-Sec, Sec. 3, A2 and Eq. (3)). E-NIST states the invariant directly: "For a public nonce $\nu$, rotate the assignment by mapping key index $i$ to pair index $(i+\nu)\bmod 12$. Every rotation preserves balance and separation" (E-NIST, Sec. 3.1).

### Step R5. Confine what crosses the partition to a declared interface

E-Sec limits the passive observer to the declared view $O=(G,Z)$ (E-Sec, Sec. 2, symbol table). E-Geo separates the internal state from its observable projection and from the private slice. For an actual valid observation $y$, the intersection of the observation fiber and the private slice is a single point (E-Geo, Sec. 4, Eqs. (F2), (F3) and (F7)):

$$
F_y\cap K_{\varphi_*,m_*}=\{(s_*,\varphi_*,m_*)\}.
$$

### Step R6. Compute locally, then combine by product

E-Sec defines a per-round local test and the global result as a product (E-Sec, Sec. 4, Eq. (6)):

$$
\widehat i_t=h^{-1}\!\left(\varphi^{-1}\!\left(\pi_t^{-1}(z_t)\right)\right),\qquad
\mu_t=\mathbf 1\{k_{r(t)}\in B_{t,\widehat i_t}\},\qquad
Y=\prod_{t=1}^{T}\mu_t.
$$

E-Sec's accompanying note on notation states that "for bits, product and AND agree."

### Step R7. Recover the intended value from the reorganized representation

E-Sec proves perfect completeness (E-Sec, Sec. 5, Theorem 1, Eq. (11)):

$$
\Pr[Y=1\mid\text{honest matching enrollment, correct delivery}]=1.
$$

The proof is that "the inverses cancel the three forward mappings." E-NIST's Theorem 2 states that, given the schedule, the masks and an accepted calibrated response, the reconstruction "returns exactly the enrolled pair" (E-NIST, Sec. 4.1). R-Sep's closing step states the aim in 2024 terms: the exponential-time problem "is now reduced to polynomial time," written $\mathcal O(n^2)$ (R-Sep, p. B-79, Step 3).

## 4. The OpenAI construction, mapped onto the same steps

### Step O1 (matches R1, R2). A transformed family with the original recoverable at zero

OpenAI starts from an exact but exponential expression (OAI, Sec. 2.2, p. 8, Eq. (2.2)). Here $C_F$ denotes the exact number of satisfying assignments of $F$, which OpenAI writes with a hash sign:

$$
C_F=\sum_{x\in\{0,1\}^n}\ \prod_{e\in F}\Phi_e\big((x_v)_{v\in I_e}\big).
$$

It then replaces each variable occurrence by a parameterized linear form, defines a polynomial family, and requires that the original be restored at the parameter value zero (OAI, Sec. 2.3, p. 9, Eqs. (2.3) and (2.4)):

$$
H(0)=C_F,\qquad \deg H\le MR\le 3nR.
$$

The paper states the requirement in words: "At $T=0$, the replacements must restore the original clause inputs."

### Step O2 (matches R3). A partition into disjoint small groups

Before the polynomial family appears, OpenAI motivates the method with a hypothetical partition of the variables into $r$ groups with at most $2n/r$ variables each, so that the count factors (OAI, Sec. 2.2, p. 8):

$$
C_F=\prod_{g=1}^{r}N_g .
$$

The formal requirement is Definition 2.1 (OAI, p. 9), condition (1): "Partition the variables into disjoint groups $[n]=S_1\sqcup\cdots\sqcup S_r$, with $|S_g|\le 2n/r$." In the auxiliary construction of Section 2.7, the paper states that "the sets $S_{t,g}$ partition $B$, with $D/r$ coordinates in each group" (OAI, Step 1, p. 14).

### Step O3 (matches R5). Cross-group dependence only through bounded measurements

Definition 2.1, conditions (3) and (4) (OAI, pp. 9 to 10), give each group an integer matrix $C_g$, write $y_g=C_gx_g$ for the measurements, bound the rows by $2\tau n$ in total and the absolute coefficient sum of each row by $D$, and require that a clause's replacement forms depend on other groups only through those measurements (Eq. (2.5)).

### Step O4 (matches R6). Sum within groups, multiply across groups

The algorithm sums assignments within each group for a fixed measurement tuple, multiplies the group sums, and accumulates over tuples (OAI, Sec. 2.4, p. 10, Eq. (2.6)):

$$
H(t)=\sum_{\vec y\in\mathcal Y}\ \prod_{g=1}^{r}\left(\sum_{u\in X_{t,g}(y_g)}A_{t,g}(u;\vec y)\right).
$$

### Step O5 (matches R4). Commuting pair-swap permutations

For the construction of the low-degree replacement forms, OpenAI defines (OAI, Sec. 2.7, p. 15): "Let $\Pi_s$ be the permutation matrix that swaps the two entries of pair $s$ in every index, leaving all other pairs unchanged. These matrices commute and satisfy $\Pi_s^2=I_D$." It then puts

$$
V_0=\prod_{s=1}^{Q}\Pi_s,\qquad W_0=\frac12\sum_{s=1}^{Q}(I_D-\Pi_s),\qquad M_0=V_0\,f(W_0),
$$

and observes that "the complete swap $V_0$ already respects every group." The paper describes the construction as interpolating $(-1)^j$ on a short interval and relates it to earlier interpolation work on low-rank approximation of Walsh-Hadamard matrices (OAI, Sec. 1.1.5, p. 6, citing [AW17, Section 3] and [AW15, Lemma 3.1]).

### Step O6 (matches R7). Recovery from Taylor coefficients

OpenAI recovers $H(0)=C_F$ from Taylor coefficients at the points $t=1,\dots,Q$, with $q=\lfloor 3nR/Q\rfloor$ and $J=q+1$ (OAI, Sec. 2.5, p. 11). It states that it uses "the same recovery principle" as Bhargava, Ghosh, Kumar and Mohapatra (OAI, Sec. 1.1.4, p. 6).

### Step O7. Reduction of the search cost

The running time is $n^{O(1)}\,2^{O\left(n(\log\log n)^2/\sqrt{\log n}\right)}$ in the bounded-occurrence case (OAI, Eq. (2.12), p. 13). The main theorem states the sharper bound with a single factor of $\log\log n$ in the exponent (OAI, Theorem 1.1, p. 2).

## 5. The distinctive matches, ranked

The matches are ranked by how specific and how unlikely to be repeated by a team working alone, which is the criterion Rosario set. For each, the table gives the two statements, followed by a plain account of what is identical and what is only analogous. The distinctiveness rating is a qualitative judgment, not a probability.

### Match 1 (strongest available). The partition as the first structural condition, with an equal-size rule

| | Rosario-Wang (E-Sec) | OpenAI (OAI) |
|---|---|---|
| Statement | L = $\bigsqcup$ of the cells B(t,i), i = 0 to H-1, each of size N/H, Eq. (8) | $[n]=S_1\sqcup\cdots\sqcup S_r$ with size $\le 2n/r$, Def. 2.1(1), p. 9 |
| Auxiliary form | exactly three keys per cell (E-NIST, Lemma 1) | $D/r$ coordinates in each group (OAI, p. 14) |
| Notation | disjoint union symbol, equal cell size written as total divided by number of cells | disjoint union symbol, size written as total divided by number of groups |
| Role of the partition | cells define one response symbol per cell, so that each secret symbol has one answer | groups limit the cost of local enumeration, so that each group is searched exhaustively |

Identical: the object (a finite set cut into disjoint cells), the symbol for disjoint union, and the form of the size rule (a total divided by the number of cells), which in OpenAI's auxiliary construction is an exact equality as in Eq. (8). E-Sec makes the equal size an assumption (A1, "$H$ divides every $n_j$," Sec. 3).

Only analogous: the purposes differ. In Rosario-Wang the equal sizes make each answer carry the same amount of information. In OpenAI the sizes bound the work. In the main design OpenAI's bound is an inequality with a factor of two, while E-Sec's is an equality. The later E-Geo document drops the requirement: "The general theory does not require equal cell sizes" (E-Geo, Sec. 2, Axiom A1).

Distinctiveness: low to moderate. A partition with a size bound is the standard first step of any divide-and-combine algorithm, and OpenAI cites Williams's split-and-list algorithm, which "partitions the variables" into groups (OAI, Sec. 1.1.4, p. 5).

### Match 2. A global result formed as a product of local results justified by disjointness

| | Rosario-Wang (E-Sec) | OpenAI (OAI) |
|---|---|---|
| Statement | $Y=\prod_{t=1}^{T}\mu_t$, Eq. (6) | count of F = $\prod_{g=1}^{r}N_g$, p. 8, and the product over groups in Eq. (2.6) |
| Factors | one 0 or 1 membership indicator per round | one count per group, and one group sum per group |
| Why a product is valid | bits: "product and AND agree" | "no clause connects different groups" |

Identical: the final combination is a product over the parts of a quantity computed from one part only.

Only analogous: Rosario-Wang's product runs over rounds that all test the same credential and is a logical conjunction. OpenAI's product runs over disjoint groups of variables and is a count factorization, and in Eq. (2.6) it is nested inside a sum over measurement tuples, which has no counterpart in ENI6MA. R-Aug's earlier sum $\mathcal P(\mathcal I_H)=\sum_j\mathcal P_j(\mathcal I_H)$ is a sum of projections, not a product.

Distinctiveness: low. Products of local factors over independent parts are ubiquitous. OpenAI attributes the sum-product formulation to Koivisto (OAI, p. 5).

### Match 3. Size-preserving rearrangement chosen so that the partition's invariants survive

| | Rosario-Wang | OpenAI |
|---|---|---|
| Operation | rotate ring by offset, key index i to (i + nu) mod 12 | swap the two entries of pair s in every index |
| Property stated | "Every rotation preserves balance and separation" (E-NIST, Sec. 3.1) | "The complete swap $V_0$ already respects every group" (OAI, p. 15) |
| Algebra | cyclic shift, order 12 in the example | commuting involutions, square of each swap is the identity |
| Purpose | randomize which symbols share a cell, for privacy | build $M_0=V_0f(W_0)$ so that substitution degrees stay below $R$ |

Identical: both use a permutation of positions, and both state that the permutation preserves the structure of the partition.

Only analogous: a cyclic rotation of a ring and a commuting family of coordinate-pair involutions are different objects with different algebra, and their purposes are unrelated. OpenAI relates its device to the matrix-rigidity literature on interpolating $(-1)^j$ (OAI, Sec. 1.1.5, p. 6). Anthropic's separate route also rests on swaps: its README summarizes the method as "the two diagonals of each rectangle form a swap. Per bit, SWAP = I $-$ 2 $\cdot$ singlet." Two laboratories converging on swap operators indicates that this device arises naturally from the problem. The repository's normalized phrase "cardinality-preserving permutation" describes the shared property at a level of abstraction at which it applies to nearly any permutation.

Distinctiveness: low.

### Match 4. A transformed representation from which a distinguished value is recovered

| | Rosario and Rosario-Wang | OpenAI |
|---|---|---|
| Statement | S_H = S_L (R-Aug, p. 2); Pr[Y = 1 given honest enrollment] = 1 (E-Sec, Eq. (11)) | H(0) = count of F, Eq. (2.4), p. 9 |
| Mechanism | inverses cancel the forward mappings (E-Sec, Theorem 1) | Taylor coefficients at t = 1 to Q determine H, whose constant coefficient is the count (OAI, Sec. 2.5) |

Identical: at the level of the normalized phrase "transform, keep a route back, recover," and nothing more specific.

Only analogous: R-Aug's entropy equation is a verbal conservation claim with no recovery procedure. E-Sec's recovery is the inversion of a bijection. OpenAI's recovery is polynomial interpolation from derivative data, for which it cites Björklund, Bhargava et al., and Woodruff and Yekhanin (OAI, Sec. 1.1.4, pp. 5 to 6). No interpolation, Taylor expansion or counting polynomial appears in the Rosario or ENI6MA documents read. The only polynomial there is a one-time authentication tag (E-Sec, Sec. 12, Lemma 7 and Theorem 9), which serves a different purpose.

Distinctiveness: low.

### Match 5. Information crossing the partition only through a bounded interface

| | Rosario-Wang | OpenAI |
|---|---|---|
| Statement | observer sees only $O=(G,Z)$; fiber meets private slice in one point, Eq. (F7) | other groups enter only through $y_h=C_hx_h$, rows bounded by $D$, Eq. (2.5) |
| Direction of purpose | hide information from an observer | compress information so that local computation can proceed |

Identical: both describe a restricted channel between parts of a structured state.

Only analogous: the channel is a security boundary in one and a computational summary in the other. The mathematics differs entirely (conditional distributions and fibers against integer linear measurements and row spaces).

Distinctiveness: very low. This match is listed because the repository's normalized map relies on it, not because it is specific.

### Summary table

| Rank | Match | Identical element | Distinctiveness |
|---|---|---|---|
| 1 | Disjoint equal-size partition, same notation and size-rule form | object, symbol, form of size rule | low to moderate |
| 2 | Product of local results justified by disjointness | form of the final combination | low |
| 3 | Size-preserving permutation that respects the partition | shared stated property | low |
| 4 | Transform, keep a way back, recover a distinguished value | normalized phrase only | low |
| 5 | Bounded interface across the partition | normalized phrase only | very low |

No match in this list involves a shared constant, a shared numerical bound, a shared error, or a shared specialized term. The vocabulary of R-Aug and R-Sep (Gestalt, dimensional collapse, holographic morphism, emergent groupings, proximity, centroid) does not occur in OpenAI's paper, and OpenAI's vocabulary (replacement linear forms, design, Taylor coefficients, Hasse derivatives, Tanner code) does not occur in any Rosario or ENI6MA document read. The word "measurement" appears in the Rosario documents only in the sense of quantum or physical measurement, which is not OpenAI's sense of integer linear measurements. The overlapping words are "partition," "group," "disjoint," "bounded," and "measurement," all common technical terms.

## 6. Dependency order: what is forced and what is not

The repository describes one ordered chain: transform, preserve, partition, balance, reindex, localize information, compute locally, combine, refine, recover, reduce cost. The question is how much of that order any algorithm of this type would impose.

**Forced by the logic of divide-and-combine.**

- A partition must exist before local work can be assigned to its pieces.
- Local work must precede combination of local results.
- A distinguished value can be recovered only after the transformed quantities exist.
- A size rule on the pieces must accompany the partition, since the cost of local enumeration depends on it.

These four constraints produce a skeleton of the form partition, then compute locally, then combine, then recover. They apply equally to Williams's 2005 split-and-list, Koivisto's 2006 sum-product formulation, and Björklund's 2016 interpolation method, all of which OpenAI cites (OAI, Sec. 1.1.4, pp. 5 to 6). Agreement of the two works on this skeleton is therefore not informative.

**Not forced, and where the two orders actually differ.**

- In OpenAI's presentation the partition is introduced first as a hypothetical in Section 2.2, the polynomial family with $H(0)=C_F$ in Section 2.3, the design (partition plus measurements) in Section 2.4, recovery in Section 2.5, and the permutation device last, in Section 2.7. In the repository's chain the transform comes first, before any partition.
- In ENI6MA the rotation is part of the definition of the partition (Eq. (3) cuts the rotated ring into cells, and Lemma 1 then proves that the cells partition the alphabet). In OpenAI the partition $S_{t,g}$ is fixed first, and the pair-swap permutations are applied afterward to a coefficient matrix to control degrees. The order of "reindex" and "partition" is thus reversed between the two.
- Bounded measurements, which sit in the middle of OpenAI's chain, have no counterpart in any Rosario or ENI6MA text read, and neither do interpolation and Taylor recovery. Stages 9 to 13 of the repository's map are matched to Rosario's text only through verbal statements (for example "successive refinement") rather than through any equation.

The honest reading is that the shared order is almost entirely the forced order, and that the places where order is not forced do not line up.

## 7. What an independent derivation would have to explain

A team working alone would have to account for the following common features, and the record offers an account for each.

1. **Partition into disjoint cells with a size rule.** Explained by the forced logic above and by prior published use (Williams 2005, Koivisto 2006), which OpenAI cites.
2. **Product of local results.** Explained by Koivisto's sum-product formulation and by elementary independence.
3. **Permutation that respects the partition.** Explained by OpenAI's own account of its source in the matrix-rigidity literature (Alman and Williams, and others, OAI Sec. 1.1.5).
4. **Recovery of a distinguished value.** Explained by OpenAI's cited interpolation and local-correction antecedents (Björklund, Bhargava et al., Woodruff and Yekhanin, Kopparty et al.).
5. **The same symbol for disjoint union.** The symbol is standard notation in mathematics.

One further matter cannot be explained from the documents alone, and it is the center of Rosario's position. It is the question of access: whether the Rosario and Rosario-Wang materials reached any system or person involved in producing the OpenAI paper. Nothing in the technical comparison speaks to that question, and nothing in the record read for this essay documents it.

### A fairness note: a second, different route to a similar bound

Anthropic separately published, within hours of OpenAI's public release, a paper titled "A $2^{o(n)}$ Time Algorithm for 3-SAT" with a Lean 4 formalization (Hexagon 2610.00577v1; repository anthropics/formal-math, folder eth). Its provenance statement says the core algorithm "was found on October 16 by an internal Claude research model with 14M output tokens and no human input" and that, "independently and concurrently, an internal model at OpenAI claims to have proven a similar result." Its description of the method refers to tensor-network contraction, rank bounds and swap operators, which differs from OpenAI's replacement linear forms and Taylor-coefficient recovery, and it reaches the same bound shape, $2^{O(n\log\log n/\sqrt{\log n})}$ for counting. Two laboratories reaching the same exponent by different methods in the same period is evidence that the result was reachable from the existing literature without any single outside source, and a fair reader will weigh it that way. It does not speak to whether OpenAI's particular route resembles Rosario's, since Anthropic's route is a different one. Rosario's comparison concerns OpenAI's paper only.

## 8. Limits and open items

These items are ranked from the most to the least damaging to the claim.

1. **Dates of the mechanics.** The ENI6MA documents that contain the partition, rotation, product and fiber equations are dated 12, 13 and 16 September 2026. The 2024 manuscripts contain none of those equations. The repository's statement that the 2024 manuscripts "establish documentary priority" for the ENI6MA mechanics is not supported by the dated documents. It rests on Rosario's testimony and on any earlier drafts that the ENI6MA documents say they were prepared from ("Two Channels and One Bijection" and "UNICITY"), whose dates are not in the record read.
2. **No algorithmic content in 2024.** R-Aug and R-Sep do not contain a #SAT, k-CNF, polynomial, interpolation or measurement construction. R-Sep's own "Sequence of Solution" has three steps (project, group by proximity with $P(d_{ij})=e^{-\alpha d_{ij}}$, solve in $\mathcal O(n^2)$), and none of them is the OpenAI method.
3. **The shared skeleton is published prior art.** OpenAI's related-work section credits the partition, local-sum, product and interpolation architecture to earlier authors (OAI, Secs. 1.1.4 and 1.1.5, pp. 5 to 6).
4. **Rosario's own documents qualify the geometry.** E-Geo states that equal cell sizes are not required (Sec. 2, Axiom A1) and that "symmetries alone do not establish a newly discovered manifold. Group actions and orbits are established tools" (E-Geo, Sec. 5). E-NIST states that "Historical distinctiveness requires comparison with earlier constructions."
5. **AI-assisted preparation.** E-NIST's transparency statement says that "AI assistance was used in manuscript drafting, consolidation, mathematical analysis, code preparation, and reference review." That does not bear on authorship of the ideas, but a reviewer will ask about the origin of the September 2026 formalizations, and the record should address it.
6. **A document-type correction.** The four-page file named ROSARIO-PAPER1 is a 27 October 2026 analysis document, not a 2024 manuscript, and should not be cited as an August 2024 source.
7. **The normalized map is a reading, not a quotation.** Stages 9 to 13 of the repository's thirteen-stage chain ("refine," "reduce search cost") are matched through paraphrase.

### Evidence that would close the gap

- Time-stamped originals of any pre-October 2026 drafts that contain the partition, rotation or product mechanics (file system metadata, email headers, version-control history, cloud-storage revision logs).
- Exports with timestamps of any conversations in which the manuscripts or ENI6MA drafts were provided to an OpenAI product, and the account settings that governed retention and training use at the time.
- Signed declarations from the research team members named in the repository, stating what each saw and when.
- A declaration from a complexity-theory expert on which of the five matches above, if any, are non-standard in the literature, and whether the combination of order and notation is unusual for a 2026 algorithm of this type.
- Any documentary link between a person or system with access to the Rosario materials and the OpenAI team or its models.

## 9. Conclusion

Laid side by side, the two formulations share a functional skeleton and, at one point, a notation and a size rule: a finite set cut into disjoint cells whose sizes are a total divided by a count. The remaining matches (product of local results, size-preserving permutation, recovery of a distinguished value, bounded interface) are shared at the level of a normalized phrase. The record read contains no shared constant, no shared error and no shared specialized terminology, and the places where the order of steps is not forced by the logic of the method do not line up between the two works.

Rosario's position is that this correspondence, together with the dated manuscripts and his account of the program's 2023 origin, shows that the OpenAI architecture follows his. What the documentary record supports today is narrower: a documented, ordered, functional parallelism, with at most one moderately specific structural coincidence, set against prior art that explains most of it. The step from parallelism to a showing that excludes independent derivation depends on evidence of access and on earlier dated drafts, which Section 8 lists. Until that evidence is assembled, the claim should be presented as Rosario's position supported by a close structural comparison, and not as a proven case of copying.
