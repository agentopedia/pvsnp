# P vs NP Knowledge Wiki
> Generated: 2026-05-03 | Papers indexed: 203 | Sources: arXiv, ECCC, Semantic Scholar, DBLP, ACM

---

## Executive Summary



---

## Concept Taxonomy

The wiki is organized into **27 concepts** across 4 layers:

### Core Complexity Theory
- **P vs NP Problem** (14 papers indexed)
- **NP-completeness** (20 papers indexed)
- **Boolean Satisfiability (SAT)** (19 papers indexed)
- **Circuit Complexity** (21 papers indexed)
- **Proof Complexity** (11 papers indexed)
- **Natural Proofs Barrier** (17 papers indexed)
- **Algebrization Barrier** (11 papers indexed)
- **Relativization / Oracle Separations** (7 papers indexed)
- **Polynomial Hierarchy** (6 papers indexed)

### Adjacent Mathematics
- **Geometric Complexity Theory** (21 papers indexed)
- **Permanent vs Determinant** (10 papers indexed)
- **Algebraic Circuit Complexity** (2 papers indexed)
- **Interactive Proofs & PCPs** (16 papers indexed)
- **Randomized Complexity & Derandomization** (16 papers indexed)
- **Counting Complexity (#P)** (12 papers indexed)

### Proof Techniques
- **Switching Lemma & Random Restrictions** (0 papers indexed)
- **Communication Complexity** (0 papers indexed)
- **Sunflower Lemma** (0 papers indexed)
- **Diagonalization & Hierarchy Theorems** (0 papers indexed)

### Cross-Domain Bridges
- **Phase Transitions in CSPs** (0 papers indexed)
- **Quantum Complexity** (0 papers indexed)
- **Cryptography & One-Way Functions** (0 papers indexed)
- **Spin Glasses & Statistical Physics** (0 papers indexed)
- **Finite Model Theory & Descriptive Complexity** (0 papers indexed)
- **Extremal Combinatorics** (0 papers indexed)
- **Game Theory & PPAD** (0 papers indexed)
- **Hardness of Approximation** (0 papers indexed)

---

## Cluster Syntheses

### Core Complexity Theory
This cluster deeply engages with the P vs NP problem, exploring its facets through various lenses. A significant portion of research focuses on establishing lower bounds for specific circuit models and proof systems, which are foundational to proving P != NP. Concurrently, the cluster grapples with major theoretical barriers like Natural Proofs, Algebrization, and Relativization, with some papers attempting to circumvent these limitations while others define new ones. The work also extends to understanding the structure of related complexity classes, such as the Polynomial Hierarchy and its quantum counterparts, and identifying the NP-completeness of diverse problems, all contributing to a comprehensive assault on one of computer science's most profound open questions.

**Key techniques:**
- Reductions (from 3-SAT, Clique, etc.): Used extensively to prove NP-hardness/completeness for various problems, including games and specific polynomial equivalence tests.
- Random Restrictions / Random Projections: Key for proving circuit lower bounds and oracle separations, particularly for classes like AC0 and TC0, and quantum query complexity.
- Diagonalization: A fundamental technique for separating complexity classes, often associated with relativization, with new variants like 'semi-relativization' being explored to evade known barriers.
- Proof Complexity techniques: Analyzing the length and structure of proofs in formal systems (e.g., Resolution, Frege, Bounded Arithmetic) to understand the inherent hardness of tautologies and unsatisfiable formulas.
- Algebraization / Arithmetization: Converting Boolean problems into algebraic ones, often used to define or analyze barriers to circuit lower bounds, especially for multilinear circuits.

**Open problems:**
- The ultimate resolution of the P vs NP problem (P=NP or P!=NP).
- Whether techniques like 'semi-relativization' can truly evade all major barriers (relativization, algebrization, natural proofs) to prove P != NP.
- Developing new and effective proof complexity generators, as explored in 'ON THE EXISTENCE OF STRONG PROOF COMPLEXITY GENERATORS' and 'Hardness of Range Avoidance and Proof Complexity Generators from Demi-Bits'.
- Finding polynomial-time algorithms for challenging problems like Simple Stochastic Games, as highlighted by 'Simple Stochastic Stopping Games'.
- A complete theoretical understanding of the efficiency benefits of restarts in CDCL SAT solvers, building on initial separations shown in 'Towards a Complexity-theoretic Understanding of Restarts in SAT solvers'.

**Most promising direction:** In my assessment, the most promising line of research in this cluster for yielding progress on P vs NP is the development of new techniques that explicitly aim to circumvent the established barriers, particularly the Natural Proofs and Algebrization barriers. The 'Hardness Magnification' framework ('Beyond Natural Proofs') is a strategic approach that seeks to reduce major complexity separations to lower bounds against weaker circuit models, where the required lower bounds might be more tractable. If successful, this could provide a structured way to bypass the limitations imposed by natural proofs. Similarly, the ambitious 'semi-relativization' technique ('Diagonalization Without Relativization'), if rigorously validated, could offer a fundamentally new form of diagonalization that evades all three major barriers, potentially opening an entirely new path to separating P and NP.

### Adjacent Mathematics
This cluster investigates the P vs NP problem by leveraging advanced mathematical tools, primarily from algebraic complexity theory, geometric complexity theory (GCT), and counting complexity (#P). Researchers aim to establish explicit lower bounds for fundamental problems like the permanent by analyzing the structure of algebraic circuits and tensors, while also exploring the power and limitations of randomized algorithms and interactive proof systems. A significant aspect involves identifying and overcoming barriers to current proof techniques, such as black-box methods and specific GCT approaches, to ultimately understand the inherent computational difficulty of core problems in theoretical computer science.

**Key techniques:**
- Algebraic Geometry & Representation Theory (GCT): Utilized in Geometric Complexity Theory to prove lower bounds by studying orbit closures of polynomials and using representation-theoretic obstructions.
- Algebraic Circuit Complexity Measures: Techniques like polynomial coefficient matrices, maximum rank under variable substitution, shifted partials, and affine projections of partials are developed to prove lower bounds for various arithmetic circuit classes.
- Symmetry Analysis & Group Theory: Employed to analyze the structure of polynomials (e.g., permanent, determinant) and computational models, leading to unconditional separations in symmetric complexity classes and optimality results for representations.
- Pseudorandom Generators (PRGs) & Derandomization: Construction of PRGs for specific computational models (e.g., CFLs, combinatorial rectangles) and analysis of their limitations, including black-box barriers.
- Interactive Proof Systems (IPS) & Probabilistically Checkable Proofs (PCPs): Development of new IPS/PCP models (e.g., quantum, distributed, resolution-based) to characterize complexity classes (e.g., PSPACE) and prove hardness of approximation.

**Open problems:**
- Resolution of P vs NP and Valiant's Conjecture: GCT is presented as a research plan for P vs NP ('On P vs. NP, Geometric Complexity Theory, and the Riemann Hypothesis', 2009), and Valiant's conjecture (Permanent vs Determinant) remains a central open problem ('Permanent v. determinant: an exponential lower bound assumingsymmetry and a potential path towards Valiant's conjecture', 2015).
- Beyond Black-Box Derandomization: The barrier results for black-box PRG constructions ('On Hardness Assumptions Needed for 'Extreme High-End'' PRGs and Fast Derandomization', 2023) imply a need for non-black-box techniques to achieve stronger derandomization.
- PCP for PPAD: The 'PCP Theorem for PPAD' is identified as a conjecture whose proof is required to establish hardness for certain approximation problems in Fisher markets ('Fisher Markets with Approximately Optimal Bundles and the Need for a PCP Theorem for PPAD', 2026).
- Reverse Direction in Communication Complexity: A significant challenge is establishing structural properties of Boolean matrices given bounds on their analytic or algebraic parameters, which is the reverse of known implications ('Structure in Communication Complexity and Constant-Cost Complexity Classes', 2024).
- Efficient Algorithms for Optimal Isoperimetric Tilings: Identified as a barrier in the context of replicable learning algorithms ('Replicability in High Dimensional Statistics', 2024).

**Most promising direction:** The **Algebraic Circuit Complexity** line of research, particularly the development of new complexity measures and the study of restricted circuit classes, appears to be the most promising direction. Papers like 'Low-depth arithmetic circuit lower bounds via shifted partials' (2022) and 'Arithmetic Circuit Lower Bounds via MaxRank' (2013) demonstrate concrete progress in proving super-polynomial lower bounds for important classes of circuits. The 'Strongly Exponential Separation Between Monotone VP and Monotone VNP' (2019) shows that for restricted models, full exponential separations are achievable. Furthermore, the introduction of 'Symmetry and Homomorphism Polynomials' (2026) leading to unconditional separations in symmetric algebraic complexity classes offers a novel path forward by leveraging structural properties. While Geometric Complexity Theory is a grander vision, it has faced significant internal barriers and refutations. The steady, incremental, and often unconditional progress in algebraic circuit complexity, by refining techniques and exploring specific structural constraints, seems more likely to yield breakthroughs that could eventually inform the broader P vs NP question.

---

## Paper Index

Total: 203 papers

- **Some conditions implying if P=NP then P=PSPACE** (2026) — Ismael Rodriguez [arxiv](http://arxiv.org/abs/2602.10073v1)
  > The paper identifies specific conditions X such that if P=NP and these conditions X hold, then P=PSPACE.
- **Implementation of Polynomial NP-Complete Algorithms Based on the NP Verifier Simulation Framework** (2026) — Changryeol Lee [arxiv](http://arxiv.org/abs/2602.10991v3)
  > The paper constructs fully specified deterministic Turing Machines (DTMs) for SAT and Subset-Sum within an improved NP verifier simulation framework, demonstrating polynomial-time bounds for these NP-
- **Wataridori is NP-Complete** (2026) — Suthee Ruangwises [arxiv](http://arxiv.org/abs/2601.09345v2)
  > Deciding whether a given Wataridori puzzle has a solution is NP-complete.
- **Proofdoors and Efficiency of CDCL Solvers** (2026) — Sunidhi Singh, Vincent Liew, Marc Vinyals et al. [arxiv](http://arxiv.org/abs/2603.26286v1)
  > Formulas with small proofdoors, a new parameter characterizing chunked clause decompositions with interpolants, are shown to have short resolution proofs and can be solved efficiently by certain CDCL 
- **An Exponential Separation between Deterministic CDCL and DPLL Solvers** (2026) — Sahil Samar, Marc Vinyals, Vijay Ganesh [arxiv](http://arxiv.org/abs/2603.16156v1)
  > A specific deterministic configuration of CDCL SAT solvers using a variant of the VSIDS branching heuristic solves Ordering Principle (OP) CNF formulas in polynomial time, demonstrating an exponential
- **Tetris is Hard with Just One Piece Type** (2026) — MIT Hardness Group, Josh Brunner, Erik D. Demaine et al. [arxiv](http://arxiv.org/abs/2603.09958v1)
  > The computational problems of Tetris clearing and survival are NP-hard for any non-O tetromino piece type under the standard Super Rotation System, even when restricted to a single piece type.
- **Convergent Gate Elimination and Constructive Circuit Lower Bounds** (2026) — M. Carmosino, Ngu Dang, Tim Jackman [semantic_scholar](https://www.semanticscholar.org/paper/8ba89ea87303232d2b654c641664481060eeb1e4)
  > This work formalizes circuit simplification as a convergent term graph rewriting system over certain bases and uses it to give the first constructive circuit lower bound proved via gate elimination, g
- **Diagonalization Without Relativization A Closer Look at the Baker-Gill-Solovay Theorem** (2026) — Baruch Garcia [semantic_scholar](https://www.semanticscholar.org/paper/c7ef4848c31d324f0beb64f08d784f79bffc55e1)
  > The paper claims that the separation of R and RE, as well as P and NP, can be proven using a new technique called 'semi-relativization', which does not relativize but evades the relativization, algebr
- **Obstruction theory and the complexity of counting group homomorphisms** (2026) — Eric Samperton, Armin Weiß [arxiv](http://arxiv.org/abs/2602.02885v2)
  > The paper establishes that counting homomorphisms from a group Γ to a finite group G is #P-hard for non-abelian G and finitely presented Γ, but is polynomial time solvable for class 2 nilpotent G unde
- **Lower Bounds in Algebraic Complexity via Symmetry and Homomorphism Polynomials** (2026) — P. Dwivedi, Benedikt Pago, Tim Seppelt [semantic_scholar](https://www.semanticscholar.org/paper/b4ad6d66cf083f747fddf0bcaad9d93b464cf9e9)
  > The paper introduces symmetric algebraic complexity classes symVP, symVBP, and symVF, and unconditionally proves their strict separation: symVF ⊊ symVBP ⊊ symVP.
- **On the Principal Minor Expansion and Complexity of the Symmetrized Determinant** (2026) — Sanyam Agarwal, Markus Blaser, M. Gupta [semantic_scholar](https://www.semanticscholar.org/paper/4cbfc4cd00e9f2136dda5c5ed3b71cb355214237)
- **Fisher Markets with Approximately Optimal Bundles and the Need for a PCP Theorem for PPAD** (2026) — Argyrios Deligkas, John Fearnley, Alexandros Hollender et al. [arxiv](http://arxiv.org/abs/2604.27276v1)
  > The problem of computing a competitive equilibrium with approximately optimal bundles in Fisher markets with SPLC utility functions is PPAD-hard for some constant $δ> 0$, assuming the PCP-for-PPAD con
- **A Relativizing MIP for BQP** (2026) — Scott Aaronson, Anand Natarajan, Avishay Tal et al. [semantic_scholar](https://www.semanticscholar.org/paper/a7d86f538e8419b20eee61a5fb07423e9a6e7ee9)
- **Computational Complexity of Physical Counting** (2026) — Tristan Simas [arxiv](http://arxiv.org/abs/2601.15571v4)
  > The paper characterizes which coordinates of a factored state space determine optimal actions and establishes the computational complexity of determining and finding minimal sets of such sufficient co
- **Have Large Language Models Learned to Reason? A Characterization via 3-SAT Phase Transition** (2025) — Rishi Hazra, Gabriele Venturato, Pedro Zuidberg Dos Martires et al. [arxiv](http://arxiv.org/abs/2504.03930v1)
  > LLM accuracy significantly drops on harder 3-SAT instances, indicating struggles without statistical shortcuts, though DeepSeek R1 uniquely shows signs of having learned underlying reasoning unlike ot
- **Quantum circuit lower bounds in the magic hierarchy** (2025) — Natalie Parham [arxiv](http://arxiv.org/abs/2504.19966v3)
  > The paper proves new lower bounds for the approximate preparation of certain explicit quantum states, including ground states of topologically ordered Hamiltonians and nonstabilizer quantum codes, by 
- **Boolean Circuit Complexity and Two-Dimensional Cover Problems** (2025) — Bruno Cavalar, Igor C. Oliveira [semantic_scholar](https://www.semanticscholar.org/paper/6f216526b4c9d001781cbe05ea6cb49f308a0631)
  > The paper reduces the problem of proving deterministic and nondeterministic Boolean circuit size lower bounds to the analysis of two-dimensional combinatorial cover problems, utilizing a 'discrete com
- **Hardness of Range Avoidance and Proof Complexity Generators from Demi-Bits** (2025) — Hanlin Ren, Yichuan Wang, Yan Zhong [semantic_scholar](https://www.semanticscholar.org/paper/bcdf335e472f92615092a78dc35680e7bf05d4c2)
  > The paper demonstrates that the existence of demi-bits generators implies the hardness of the Range Avoidance problem for nondeterministic algorithms, enables the construction of pseudo-surjective pro
- **Fine-Grained Complexity via Quantum Natural Proofs** (2025) — Yanlin Chen, Yilei Chen, Rajendra Kumar et al. [arxiv](http://arxiv.org/abs/2504.10363v2)
  > This paper shows how the 'compression oblivious' requirement in the QSETH framework can often be replaced by the existence of quantum-secure pseudorandom functions, and specifically proves that proper
- **New Algebrization Barriers to Circuit Lower Bounds via Communication Complexity of Missing-String** (2025) — Lijie Chen, Yang Hu, Hanlin Ren [arxiv](http://arxiv.org/abs/2511.14038v1)
  > This work establishes several new algebrization barriers to circuit lower bounds for PostBPE, BPE, and a natural subclass of MA_E, by constructing specific oracles and their multilinear extensions usi
- **Adversarial Barrier in Uniform Class Separation** (2025) — Milan Rosko [semantic_scholar](https://www.semanticscholar.org/paper/f69ad4e9fb2f12f746cc2379968467a2e78b6149)
  > A strong structural obstruction to Uniform Separation in constructive arithmetic is identified, emerging from the parallel existence of distinct evaluator predicates and uniformly representable infere
- **Toward P vs NP: An Observer-Theoretic Separation via SPDP Rank and a ZFC-Equivalent Foundation within the N-Frame Model** (2025) — D. Edwards [semantic_scholar](https://www.semanticscholar.org/paper/db44c39e2583a58358f1364899a1e176300b33be)
  > This paper presents a self-contained ZFC-based separation framework that yields a contradiction under the assumption P = NP, thereby establishing P != NP.
- **Psi-Turing Machines: Bounded Introspection for Complexity Barriers and Oracle Separations** (2025) — Rafig Huseynzade [semantic_scholar](https://www.semanticscholar.org/paper/ec9849119f2e5e81499b9bb697dd3104831ab66a)
  > We introduce Psi-Turing Machines (Psi-TM): classical Turing machines equipped with a constant-depth introspection interface $ \iota $ and an explicit per-step information budget $ B(d,n)=c\,d\log_2 n 
- **Oracle Separations for RPH** (2025) — Thekla Hamm, Lucas Meijer, Tillmann Miltzow et al. [semantic_scholar](https://www.semanticscholar.org/paper/1582be87a95c8a4611c849db7905b491fa8ae42e)
- **Oracle separations for non-adaptive collapse-free quantum computing** (2025) — Henrique Hepp, M. V. G. Silva, L. Zatesko [semantic_scholar](https://www.semanticscholar.org/paper/49be0f30b46b293683a64ede15e595c338244f27)
  > The paper proves the existence of an oracle A for which P A = BQP A = SZK A = naCQP A ̸ = ( UP ∩ coUP ) A, and that NP A ̸⊆ naCQP A with probability 1 relative to a random oracle.
- **Multiquadratic Sum-of-Squares Lower Bounds Imply VNC$^1$ $\neq$ VNP** (2025) — Benjamin Rossman, Davidson Zhu [arxiv](http://arxiv.org/abs/2512.01227v1)
- **Model Counting for Dependency Quantified Boolean Formulas** (2025) — Long-Hin Fung, Che Cheng, J. Jiang et al. [semantic_scholar](https://www.semanticscholar.org/paper/df9001ad76f953099fb4ec1f90c37f663be1e655)
  > The model counting problem for 2-DQBF, denoted #2-DQBF, is #EXP-complete, paralleling Valiant's theorem for #2-SAT.
- **On the NP-Hardness Approximation Curve for Max-2Lin(2)** (2024) — Björn Martinsson [arxiv](http://arxiv.org/abs/2408.04832v2)
  > The paper presents a procedure for constructing increasingly better gadgets for Max-2Lin(2) inapproximability results, which is then used to construct an NP-hardness approximation curve $s(c)$ that im
- **Topics in Non-local Games: Synchronous Algebras, Algebraic Graph Identities, and Quantum NP-hardness Reductions** (2024) — Entong He [arxiv](http://arxiv.org/abs/2408.10114v5)
- **NP-hardness of testing equivalence to sparse polynomials and to constant-support polynomials** (2024) — Omkar Baraskar, Agrim Dewan, Chandan Saha et al. [arxiv](http://arxiv.org/abs/2410.12251v1)
  > The problem of testing equivalence to sparse polynomials (ETsparse) and to constant-support polynomials is NP-hard over any field, even when the input polynomial is given in sparse representation.
- **PSPACE-Hard 2D Super Mario Games: Thirteen Doors** (2024) — MIT Hardness Group, Hayashi Ani, Erik D. Demaine et al. [arxiv](http://arxiv.org/abs/2404.10380v1)
  > The paper proves PSPACE-hardness for fifteen 2D Super Mario Bros. games and NP-hardness for the remaining two 2D Mario games (Super Mario Land and Super Mario Run).
- **An even simpler hard variant of Not-All-Equal 3-SAT** (2024) — Andreas Darmann, Janosch Döcker, Britta Dorn [arxiv](http://arxiv.org/abs/2412.03395v2)
- **Polynomial Calculus for Quantified Boolean Logic: Lower Bounds Through Circuits and Degree.** (2024) — Olaf Beyersdorff, Tim Hoffmann, Kaspar Kasche et al. [dblp](https://dblp.org/rec/conf/mfcs/BeyersdorffHKS24)
- **Quantum Automating $\mathbf{TC}^0$-Frege Is LWE-Hard** (2024) — Noel Arteche, Gaia Carenini, Matthew Gray [arxiv](http://arxiv.org/abs/2402.10351v3)
  > Under the Learning with Errors (LWE) assumption, no quantum algorithm can weakly automate $\mathbf{TC}^0$-Frege.
- **Bounded-Depth Frege Lower Bounds for Random 3-CNFs via Deterministic Restrictions** (2024) — Svyatoslav Gryaznov, Navid Talebanfard [arxiv](http://arxiv.org/abs/2403.02275v3)
  > For every $k$, there exists $ε_k > 0$ such that any depth-$k$ Frege refutation of a random $n$-variable 3-CNF with $Θ(n)$ clauses requires $Ω(n^{1 + ε_k})$ steps with high probability.
- **Finding Bugs in Short Proofs: The Metamathematics of Resolution Lower Bounds** (2024) — Jiawei Li, Yuhao Li, Hanlin Ren [arxiv](http://arxiv.org/abs/2411.15515v2)
  > The paper introduces a new class $\mathrm{rwPHP}(\mathsf{PLS})$ in decision-tree $\mathsf{TFNP}$ to capture the complexity of refuter problems for resolution size lower bounds, showing that the theory
- **Jump Operators, Interactive Proofs and Proof Complexity Generators** (2024) — Erfan Khaniki [semantic_scholar](https://www.semanticscholar.org/paper/19b54ca26c4126b232f4c72196d5574f91b2976a)
  > The paper introduces a new candidate jump operator based on interactive proofs and proves that the widely believed assumption about the existence of computable jump operators in proof complexity is eq
- **Proof complexity of universal algebra in a CSP dichotomy proof** (2024) — Azza Gaysin [semantic_scholar](https://www.semanticscholar.org/paper/fd9570aee4095e748b92b62f278a7f3eb92abd5e)
  > This paper formalizes universal algebra theorems crucial for Zhuk's CSP dichotomy algorithm in bounded arithmetic $W^1_1$, demonstrating that $W^1_1$ proves the algorithm's soundness and implies short
- **Simple Stochastic Stopping Games: A Generator and Benchmark Library** (2024) — Avi Rudich, Isaac Rudich, Rachel Rue [arxiv](http://arxiv.org/abs/2402.02571v1)
  > The paper introduces a complete generating algorithm and a benchmark library for fully reduced instances of Simple Stochastic Stopping Games, along with an analysis of existing algorithms' performance
- **A simple lower bound for the complexity of estimating partition functions on a quantum computer** (2024) — Zherui Chen, Giacomo Nannicini [arxiv](http://arxiv.org/abs/2404.02414v2)
  > The paper provides a $\varOmega(1/\varepsilon)$ lower bound for the number of reflections needed by a quantum algorithm to estimate the partition function $\mathsf{Z}(\beta)$ with accuracy $\varepsilo
- **Oracle Separations for the Quantum-Classical Polynomial Hierarchy** (2024) — Avantika Agarwal, S. Ben-David [semantic_scholar](https://www.semanticscholar.org/paper/8325d10f17f1be00b153c9a12e16d662a2e5d6e3)
  > The quantum-classical polynomial hierarchy (QCPH) is infinite relative to a random oracle, and higher levels of the classical polynomial hierarchy (PH) are not contained in lower levels of QCPH relati
- **A Resolution-Based Interactive Proof System for UNSAT** (2024) — Philipp Czerner, Javier Esparza, Valentin Krasotin [semantic_scholar](https://www.semanticscholar.org/paper/0aa3a5c024083a6a33e1765fb1c577558d88668a)
  > The paper presents a theorem reducing the problem of finding competitive interactive protocols for UNSAT to finding an arithmetisation of formulas with specific commutativity properties, and applies t
- **Replicability in High Dimensional Statistics** (2024) — Max Hopkins, Russell Impagliazzo, Daniel Kane et al. [arxiv](http://arxiv.org/abs/2406.02628v1)
  > The paper establishes a computational and statistical equivalence between optimal replicable algorithms and high dimensional isoperimetric tilings, which yields matching sample complexity upper and lo
- **Pseudorandom Permutations from Random Reversible Circuits** (2024) — William He, Ryan O'Donnell [arxiv](http://arxiv.org/abs/2404.14648v4)
  > A random reversible circuit of depth n * O-tilde(k^2) using nearest-neighbor 3-bit gates yields almost k-wise independent permutations.
- **Structure in Communication Complexity and Constant-Cost Complexity Classes** (2024) — Hamed Hatami, Pooya Hatami [arxiv](http://arxiv.org/abs/2401.14623v1)
  > The paper discusses research directions concerning the relationship between communication complexity of a matrix and its analytic or algebraic parameters, emphasizing the challenge of establishing the
- **On the Counting Complexity of the Skolem Problem** (2024) — Gorav Jindal, Joël Ouaknine [semantic_scholar](https://www.semanticscholar.org/paper/0ab0432b343215f1307af6903c82fb4dd4439242)
  > The problem of counting the zeros of a given integer linear recurrence sequence (LRS) is #P-hard, and #P-complete for the instances generated in their reduction.
- **A new approach for a proof that P is NP** (2023) — Malay Dutta, Anjana K. Mahanta [arxiv](http://arxiv.org/abs/2302.09024v1)
  > The paper proposes a new technique for proving P=NP, involving a polynomial-time reduction of a novel NP-complete problem (Hamiltonian Time Path) to Linear Programming using multiple subroutine calls,
- **An Approach to Introduce High-School Students to the P-vs-NP Question.** (2023) — Jisoo Song, Seoyeon Oh, Soyeon Jeong et al. [dblp](https://dblp.org/rec/conf/issep/SongOJP23)
- **Verification of NP-hardness Reduction Functions for Exact Lattice Problems** (2023) — Katharina Kreuzer, Tobias Nipkow [arxiv](http://arxiv.org/abs/2306.08375v1)
  > The formal verification of NP-hardness reduction functions for the closest vector problem and shortest vector problem (infinity norm) was successfully completed using Isabelle, uncovering and correcti
- **Local Search and Its Application in CDCL/CDCL(T) solvers for SAT/SMT.** (2023) — Shaowei Cai 0001 [dblp](https://dblp.org/rec/conf/fmcad/Cai23)
- **Tight Correlation Bounds for Circuits Between AC0 and TC0** (2023) — Vinayak M. Kumar [arxiv](http://arxiv.org/abs/2304.02770v2)
  > The paper establishes a tight multi-switching lemma and a new depth reduction lemma for generalized AC0 circuits (GC0(k)), enabling many results previously obtained for AC0 circuits to be lifted to GC
- **Sharp Thresholds Imply Circuit Lower Bounds: from random 2-SAT to Planted Clique** (2023) — David Gamarnik, Elchanan Mossel, Ilias Zadik [arxiv](http://arxiv.org/abs/2311.04204v3)
  > Any Boolean function exhibiting a sharp enough threshold at arbitrary critical density cannot be computed by Boolean circuits of bounded depth and polynomial size, implying average-case circuit lower 
- **Depth-𝑑 Threshold Circuits vs. Depth-(𝑑+1) AND-OR Trees** (2023) — Pooya Hatami, William M. Hoza, Avishay Tal et al. [semantic_scholar](https://www.semanticscholar.org/paper/1d7ae20bb15abf2f6ce9db0376287ee35286fd97)
  > For any n ∈ ℕ and d = o(loglog(n)), there exists a Boolean function F computable by a uniform depth-(d+1) AC0 circuit with O(n) wires, but not by any depth-d TC0 circuit with n^(1+γ) wires, where γ = 
- **Sum-of-Squares Lower Bounds for the Minimum Circuit Size Problem** (2023) — Per Austrin, Kilian Risse [semantic_scholar](https://www.semanticscholar.org/paper/9437b504906801044da9f893079ffd1a8121fd32)
- **A PROOF COMPLEXITY CONJECTURE AND THE INCOMPLETENESS THEOREM** (2023) — Jan Krajícek [semantic_scholar](https://www.semanticscholar.org/paper/6b4f23076290e797a2c2461b64d5eb9b5d68afa8)
  > A p-time stretching function is used to prove incompleteness for sound first-order theories and to show that for propositional systems, at least one of three significant statements must be true: eithe
- **Stretching Demi-Bits and Nondeterministic-Secure Pseudorandomness** (2023) — Iddo Tzameret, Lulu Zhang [semantic_scholar](https://www.semanticscholar.org/paper/b6f2a745ed6bcfce60b59aa3cfa6ecde227ba92e)
- **On Hardness Assumptions Needed for "Extreme High-End'' PRGs and Fast Derandomization** (2023) — Ronen Shaltiel, Emanuele Viola [arxiv](http://arxiv.org/abs/2311.11663v1)
  > The paper shows that certain black-box approaches cannot construct extreme high-end PRGs from the extreme high-end hardness assumption, providing a partial negative answer to their feasibility.
- **On the works of Avi Wigderson** (2023) — Boaz Barak, Yael Kalai, Ran Raz et al. [arxiv](http://arxiv.org/abs/2307.09524v1)
  > The paper provides an overview of selected works by Avi Wigderson across cryptography, pseudorandomness, computational complexity lower bounds, and optimization over symmetric manifolds, highlighting 
- **The Complexity of Counting Planar Graph Homomorphisms of Domain Size 3** (2023) — Jin-Yi Cai, Ashwin Maran [semantic_scholar](https://www.semanticscholar.org/paper/a734dec6b0203ffe0de6d7c161e02d0340a55319)
  > We prove a complexity dichotomy theorem for counting planar graph homomorphisms of domain size 3, completely classifying the computational complexity of this problem for any 3x3 real valued symmetric 
- **Exploring P versus NP** (2022) — Jian-Gang Tang [arxiv](http://arxiv.org/abs/2209.15410v7)
  > The paper proposes a strategy to prove P != NP by reducing an EXP-complete problem to an NP problem in polynomial time, which would imply EXP=NP, and then using the 'well-known' P != NP to derive P !=
- **ON THE EXISTENCE OF STRONG PROOF COMPLEXITY GENERATORS** (2022) — J. Krajícek [semantic_scholar](https://www.semanticscholar.org/paper/ebc27aaa29f877ba0b18526915073b9838f45621)
  > The paper argues for a specific gadget generator as a strong candidate for a proof complexity generator, defines a new V-hardness property, and conditionally shows the main conjecture holds for all fe
- **Complexity and Ramsey Largeness of Sets of Oracles Separating Complexity Classes** (2022) — Alex Creiner, Stephen Jackson [semantic_scholar](https://www.semanticscholar.org/paper/da1ed15b52593616ceeff53a253e26288338aa52)
  > The paper demonstrates that sets of oracles separating complexity classes like NP from co-NP, PSPACE from PH, and NP from BQP are "large" in the Ellentuck topology, which makes a variation of the rand
- **Separations in Proof Complexity and TFNP** (2022) — Mika Göös, Alexandros Hollender, Siddhartha Jain et al. [semantic_scholar](https://www.semanticscholar.org/paper/cd1cb3c99b518fcc98a146bb84bd489f62c9cc8b)
  > This paper shows that Resolution cannot efficiently simulate Sherali-Adams proofs with unary coefficients, and Reversible Resolution cannot efficiently simulate Nullstellensatz proofs, leading to char
- **Monotone Classes Beyond VNP** (2022) — Prerona Chatterjee, Kshitij Gajjar, Anamay Tengse [arxiv](http://arxiv.org/abs/2202.13103v4)
  > The paper defines monotone VPSPACE (mVPSPACE) as the monotone analogue of Poizat's definition, demonstrating it is exponentially stronger than mVNP and possesses desirable closure properties, in contr
- **Low-depth arithmetic circuit lower bounds via shifted partials** (2022) — Prashanth Amireddy, Ankit Garg, Neeraj Kayal et al. [arxiv](http://arxiv.org/abs/2211.07691v1)
  > The paper proves super-polynomial lower bounds for low-depth arithmetic circuits, including for iterated matrix multiplication and Nisan-Wigderson design polynomials, and for a new subclass called uni
- **A Simple Proof of PreciseQMA = PSPACE** (2022) — Yulong Li [arxiv](http://arxiv.org/abs/2206.09230v1)
  > The paper provides an alternative proof of the equivalence PreciseQMA = PSPACE, where PreciseQMA is Quantum Merlin-Arthur with an inverse exponential completeness-soundness gap.
- **Microteaching: Semantics, Definition of a Computer, Running Times, Fractal Trees, Classes as Encapsulation, and P vs NP.** (2021) — Colleen M. Lewis, Kathi Fisler, Jenny Hinz et al. [dblp](https://dblp.org/rec/conf/sigcse/LewisFHMPPS21)
- **A note on VNP-completeness and border complexity** (2021) — Christian Ikenmeyer, Abhiroop Sanyal [arxiv](http://arxiv.org/abs/2102.07173v3)
  > The paper demonstrates that both the set of VNP-complete polynomials (VNPC) and its complement (VNP \ VNPC) lie dense in VNP under various reduction notions, including p-projections and border reducti
- **The PCP-like Theorem for Sub-linear Time Inapproximability** (2021) — Hengzhao Ma, Jianzhong Li [arxiv](http://arxiv.org/abs/2107.01520v3)
  > The paper proposes a PCP-like theorem for sub-linear time inapproximability, extending previous distributed PCP frameworks.
- **Quantum Pseudorandomness and Classical Complexity** (2021) — William Kretschmer [arxiv](http://arxiv.org/abs/2103.09320v5)
- **A class of examples demonstrating that P is different from NP in the "P vs NP" problem** (2020) — Vasil Penchev [arxiv](http://arxiv.org/abs/2005.01412v1)
  > The paper claims to prove P is different from NP by formulating a class of counterexamples based on quantum superposition and fundamentally random choices.
- **What one has to know when attacking P vs. NP.** (2020) — Juraj Hromkovic, Peter Rossmanith [dblp](https://dblp.org/rec/journals/jcss/HromkovicR20)
- **Classifying CELESTE as NP Complete** (2020) — Zeeshan Ahmed, Alapan Chaudhuri, Kunwar Shaanjeet Singh Grover et al. [arxiv](http://arxiv.org/abs/2012.07678v4)
  > Solving a generalized level of the video game "CELESTE" is NP-Complete.
- **Revisiting Cook-Levin theorem using NP-Completeness and Circuit-SAT** (2020) — E. E. Ogheneovo [semantic_scholar](https://www.semanticscholar.org/paper/d7e8c1f9ca4bb5af01529426a06dd282b2ffb46c)
  > A new proof for the NP-completeness of Boolean Satisfiability (SAT) is presented, using a combination of NP-completeness concepts and Circuit-SAT, through the reduction of polynomial time algorithms.
- **THE GUIDE TO NP-COMPLETENESS IS 40 YEARS OLD: AN HOMAGE TO DAVID S. JOHNSON** (2020) — L. Buriol, C. M. Figueiredo, Maurício Resende et al. [semantic_scholar](https://www.semanticscholar.org/paper/2bb64c4ff567e71e761c697b1df10b9e0c557d26)
  > This paper is an homage to David S. Johnson, summarizing his significant contributions to the theory of NP-completeness, approximation algorithms, and the experimental analysis of algorithms, celebrat
- **From NP-Completeness to DP-Completeness: A Membrane Computing Perspective.** (2020) — Luis Valencia-Cabrera, David Orellana-Martín, Miguel Ángel Martínez-del-Amor et al. [dblp](https://dblp.org/rec/journals/complexity/Valencia-Cabrera20)
- **Towards a Complexity-theoretic Understanding of Restarts in SAT solvers** (2020) — Chunxiao Li, Noah Fleming, Marc Vinyals et al. [arxiv](http://arxiv.org/abs/2003.02323v2)
  > This paper provides the first exponential separation results demonstrating that restarts can make CDCL SAT solvers exponentially more powerful for certain instance families, while also showing that re
- **Hardness of Random Optimization Problems for Boolean Circuits, Low-Degree Polynomials, and Langevin Dynamics** (2020) — David Gamarnik, Aukosh Jagannath, Alexander S. Wein [arxiv](http://arxiv.org/abs/2004.12063v2)
- **On the Existence of Algebraic Natural Proofs** (2020) — Prerona Chatterjee, Mrinal Kumar, C Ramya et al. [arxiv](http://arxiv.org/abs/2004.14147v4)
  > Over fields of characteristic zero, VNP does not have efficient equations if the Permanent is exponentially hard for algebraic circuits (even in the approximative sense), which establishes a barrier t
- **Circuit lower bounds for low-energy states of quantum code Hamiltonians** (2020) — Anurag Anshu, Chinmay Nirkhe [arxiv](http://arxiv.org/abs/2011.02044v5)
  > This work proves super-constant quantum circuit lower bounds for the complexity of all low-energy states (energy o(n)) of local Hamiltonians arising from nearly linear-rate or nearly linear-distance L
- **If VNP is hard, then so are equations for it** (2020) — Mrinal Kumar, C. Ramya, Ramprasad Saptharishi et al. [arxiv](http://arxiv.org/abs/2012.07056v1)
  > Assuming the Permanent polynomial requires algebraic circuits of exponential size, the class VNP does not have efficiently computable equations, meaning any non-zero polynomial vanishing on VNP's coef
- **Walking through Doors is Hard, even without Staircases: Universality and PSPACE-hardness of Planar Door Gadgets** (2020) — MIT Gadgets Group, Jeffrey Bosboom, Erik D. Demaine et al. [arxiv](http://arxiv.org/abs/2006.01256v2)
  > It is PSPACE-complete to decide whether an agent can move from one location to another through a planar system of simple door gadgets, which are shown to be universal gadgets capable of simulating any
- **Proof Compression and NP Versus PSPACE II: Addendum** (2020) — L. Gordeev, E. H. Haeusler [arxiv](http://arxiv.org/abs/2011.09262v2)
  > The paper claims to prove NP = coNP by applying proof compression techniques to 'naive' natural deduction refutations of NP-complete problems, specifically Hamiltonian cycles, without relying on Hudel
- **PCP Theorems, SETH and More: Towards Proving Sub-linear Time Inapproximability** (2020) — Hengzhao Ma, Jianzhong Li [arxiv](http://arxiv.org/abs/2011.02320v4)
  > The paper proposes a novel PCP-like theorem specifically designed for proving sub-linear time inapproximability results, adapting an MA-protocol for the Set Containment problem.
- **Counting Maximum Matchings in Planar Graphs Is Hard** (2020) — Istvan Miklos, Miklos Kresz [arxiv](http://arxiv.org/abs/2001.01493v2)
  > Counting maximum matchings in planar, bipartite graphs is #P-complete.
- **Unification of the Nature’s Complexities via a Matrix Permanent—Critical Phenomena, Fractals, Quantum Computing, ♯P-Complexity** (2020) — V. Kocharovsky, V. Kocharovsky, S. Tarasov [semantic_scholar](https://www.semanticscholar.org/paper/9b1ee1b7a89875b23ff740ee7ef21e34575edfbb)
  > The paper establishes analytic relations between the matrix permanent and various natural complexities, including critical phenomena, fractals, quantum computing, number theory, and #P-complete proble
- **Placing quantified variants of 3-SAT and Not-All-Equal 3-SAT in the polynomial hierarchy** (2019) — Janosch Döcker, Britta Dorn, Simone Linz et al. [arxiv](http://arxiv.org/abs/1908.05361v2)
  > The complexity of variants of 3-SAT and Not-All-Equal 3-SAT is well studied. However, in contrast, very little is known about the complexity of the problems' quantified counterparts. In the first part
- **On simplified NP-complete variants of Not-All-Equal 3-Sat and 3-Sat** (2019) — Andreas Darmann, Janosch Döcker [arxiv](http://arxiv.org/abs/1908.04198v2)
  > The paper demonstrates that Not-All-Equal 3-Sat and Monotone 3-Sat remain NP-complete under various strong structural restrictions, including specific exact variable appearance counts and linearity.
- **Parallels Between Phase Transitions and Circuit Complexity?** (2019) — Ankur Moitra, Elchanan Mossel, Colin Sandon [arxiv](http://arxiv.org/abs/1904.05483v2)
  > The paper establishes qualitative connections between phase transitions and circuit complexity in the broadcast tree model, showing that a TC0 circuit can compete with the Bayes optimal predictor abov
- **Beyond Natural Proofs: Hardness Magnification and Locality** (2019) — Lijie Chen, Shuichi Hirahara, Igor C. Oliveira et al. [arxiv](http://arxiv.org/abs/1911.08297v1)
  > The paper provides more examples of hardness magnification and investigates its potential for proving new lower bounds, focusing on its interaction with the natural proofs barrier and the adaptability
- **On CDCL-based proof systems with the ordered decision strategy** (2019) — Nathan Mull, Shuo Pang, Alexander Razborov [arxiv](http://arxiv.org/abs/1909.04135v1)
  > CDCL SAT-solvers with an ordered decision strategy are equivalent to ordered resolution under the DECISION learning scheme, and to general resolution under a different learning scheme that stops after
- **Weak lower bounds on resource-bounded compression imply strong separations of complexity classes** (2019) — D. McKay, Cody Murray, Richard Ryan Williams [semantic_scholar](https://www.semanticscholar.org/paper/08992622f19956a71a692d2e8cbb89891e47abe5)
  > Weak worst-case lower bounds on the search version of resource-bounded compression problems (like MCSP and time-bounded Kolmogorov complexity), even for highly restricted computational models, imply s
- **Strongly Exponential Separation Between Monotone VP and Monotone VNP** (2019) — Srikanth Srinivasan [arxiv](http://arxiv.org/abs/1903.01630v2)
  > The paper demonstrates a sequence of explicit multilinear polynomials with non-negative coefficients in monotone VNP that require monotone algebraic circuits of size $\exp(\Omega(n))$.
- **Search problems in algebraic complexity, GCT, and hardness of generator for invariant rings** (2019) — Ankit Garg, Christian Ikenmeyer, Visu Makam et al. [arxiv](http://arxiv.org/abs/1910.01251v2)
  > The paper disproves Mulmuley's conjecture that polynomial-sized succinct encodings always exist for generators of invariant rings of $\SL_n(\C)$-representations, under standard complexity assumptions.
- **Implementing geometric complexity theory: on the separation of orbit closures via symmetries** (2019) — Christian Ikenmeyer, Umangathan Kandasamy [semantic_scholar](https://www.semanticscholar.org/paper/dece735ce212ad2751e2fcf33cc7c3c7847daaca)
  > This paper implements the geometric complexity theory approach by Mulmuley and Sohoni, demonstrating a new multiplicity obstruction that separates the orbit closure of the power sum polynomial from th
- **Towards a quantum-inspired proof for IP = PSPACE** (2019) — Ayal Green, Guy Kindler, Yupan Liu [arxiv](http://arxiv.org/abs/1912.11611v3)
- **Non-Signaling Proofs with $O(\sqrt{\log n})$ Provers are in PSPACE** (2019) — Dhiraj Holden, Yael Kalai [arxiv](http://arxiv.org/abs/1910.02590v3)
- **Subspace arrangements, graph rigidity and derandomization through submodular optimization** (2019) — Orit E. Raz, Avi Wigderson [arxiv](http://arxiv.org/abs/1901.09423v1)
  > The paper presents a deterministic, strongly polynomial time algorithm for computing the matrix rank for a class of symbolic matrices, a problem previously known to be in NP intersect coNP and BPP.
- **More barriers for rank methods, via a "numeric to symbolic" transfer** (2019) — Ankit Garg, Visu Makam, Rafael Oliveira et al. [arxiv](http://arxiv.org/abs/1904.04299v1)
  > The paper proves new barrier results showing that even optimal rank lower bounds on k-tensors cannot yield non-trivial lower bounds on the rank of d-tensors for any constant d>k, thereby demonstrating
- **Algorithms and Complexity for Functions on General Domains** (2019) — Erich Novak [arxiv](http://arxiv.org/abs/1908.05943v2)
  > For approximation and integration of functions on general bounded Lipschitz domains, the asymptotic constant of optimal error bounds often depends only on the domain's volume (not its shape or boundar
- **Machine Learning-Based Restart Policy for CDCL SAT Solvers.** (2018) — Jia Hui Liang, Chanseok Oh, Minu Mathew et al. [dblp](https://dblp.org/rec/conf/sat/LiangOMTLG18)
- **Some Results on the Circuit Complexity of Bounded Width Circuits and Nondeterministic Circuits** (2018) — Hiroki Morizumi [arxiv](http://arxiv.org/abs/1811.01347v2)
- **Adaptive Lower Bound for Testing Monotonicity on the Line** (2018) — Aleksandrs Belovs [arxiv](http://arxiv.org/abs/1801.08709v2)
  > The paper proves a nearly tight $Ω(\frac{\log r}{\log \log r})$ lower bound for $ε$-testing monotonicity of a function $f\colon [n]\to[r]$ when $ε=1/2$, and completely characterizes the query complexi
- **Generalized matrix completion and algebraic natural proofs** (2018) — M. Bläser, Christian Ikenmeyer, Gorav Jindal et al. [semantic_scholar](https://www.semanticscholar.org/paper/e0d1132428e8af0841763c75184b9a84c82c99b7)
  > The paper establishes an algebraic natural proofs barrier for generalized matrix completion, conditional on coNP ⊆ ∃ BPP, but shows that Geometric Complexity Theory can overcome this barrier for the p
- **Quantum generalizations of the polynomial hierarchy with applications to QMA(2)** (2018) — Sevag Gharibian, M. Santha, Jamie Sikora et al. [semantic_scholar](https://www.semanticscholar.org/paper/bff6a95c98861ff049ee6d4bc491d563c8fe9816)
  > The paper places the third level of the quantum polynomial hierarchy with quantum proofs (QΣ3) into NEXP using the ellipsoid method and derives two implications for QMA(2) based on the relationship be
- **The query complexity of graph isomorphism: bypassing distribution testing lower bounds** (2018) — Krzysztof Onak, Xiaorui Sun [semantic_scholar](https://www.semanticscholar.org/paper/22898527c8ea18867ecfa21b80890a4b0fee0b70)
  > The paper presents an algorithm for testing graph isomorphism in dense graphs with a query complexity of n^(1+o(1)), which is optimal up to a subpolynomial factor and improves upon the previous best b
- **Fine-grained Complexity Meets IP = PSPACE** (2018) — Lijie Chen, Shafi Goldwasser, Kaifeng Lyu et al. [arxiv](http://arxiv.org/abs/1805.02351v3)
  > The paper establishes reductions from exact to approximate solutions for problems in P, identifying a BP-Pair-Class where exact and approximate solutions are equivalent under near-linear time reductio
- **On the Approximation Method and the P versus NP Problem** (2017) — Norbert Blum [arxiv](http://arxiv.org/abs/1708.03486v3)
  > The paper provides evidence that the approximation method alone is insufficient to prove super-linear lower bounds for the non-monotone complexity of Boolean functions, while also arguing that natural
- **Planar 3-SAT with a Clause/Variable Cycle** (2017) — Alexander Pilz [arxiv](http://arxiv.org/abs/1710.07476v6)
  > The problem of deciding satisfiability of a 3-SAT formula remains NP-complete even when its planar incidence graph can be augmented by a given Hamiltonian cycle passing through all variables and then 
- **一种基于搜索路径识别的CDCL命题逻辑求解器延迟重启算法 (Path Identification Based Delaying Restart Algorithm for CDCL SAT Solver).** (2017) — Qingshan Chen, Yang Xu 0001, Guanfeng Wu et al. [dblp](https://dblp.org/rec/journals/jsjkx/Chen0WH18)
- **A Tight Lower Bound for Counting Hamiltonian Cycles via Matrix Rank** (2017) — Radu Curticapean, Nathan Lindzey, Jesper Nederlof [arxiv](http://arxiv.org/abs/1709.02311v2)
- **Towards an algebraic natural proofs barrier via polynomial identity testing** (2017) — Joshua A. Grochow, Mrinal Kumar, Michael Saks et al. [arxiv](http://arxiv.org/abs/1701.01717v1)
  > A class of algebraic proof techniques, encompassing nearly all known algebraic circuit lower bounds, cannot prove lower bounds against VP if and only if succinct hitting sets for VP exist, establishin
- **Succinct Hitting Sets and Barriers to Proving Algebraic Circuits Lower Bounds** (2017) — Michael A. Forbes, Amir Shpilka, Ben Lee Volk [arxiv](http://arxiv.org/abs/1701.05328v2)
  > The existence of an algebraic natural proofs barrier is shown to be equivalent to the existence of succinct derandomization of the polynomial identity testing problem, and the paper provides the first
- **Distributed PCP Theorems for Hardness of Approximation in P** (2017) — Amir Abboud, Aviad Rubinstein, Ryan Williams [arxiv](http://arxiv.org/abs/1706.06407v2)
  > The paper introduces a new distributed model of probabilistically checkable proofs (PCPs) and uses it to obtain the first PCP-like reductions from the Strong Exponential Time Hypothesis (SETH) to appr
- **Quantified Derandomization of Linear Threshold Circuits** (2017) — Roei Tell [arxiv](http://arxiv.org/abs/1709.07635v2)
  > The paper presents the first quantified derandomization algorithm for $TC^0$ circuits of depth $d>2$ (and linear threshold circuits) with super-linear wires, which runs in almost-polynomial-time and d
- **Autoreducibility of NP-Complete Sets** (2016) — John M. Hitchcock, Hadi Shafei [arxiv](http://arxiv.org/abs/1601.05494v1)
- **On the Hardness of SAT with Community Structure** (2016) — Nathan Mull, Daniel J. Fremont, Sanjit A. Seshia [arxiv](http://arxiv.org/abs/1602.08620v4)
  > The paper establishes hardness results showing that community structure is not sufficient to explain the practical success of CDCL SAT solvers, as instances with good community structure can still be 
- **Solving MaxSAT by Successive Calls to a SAT Solver** (2016) — Mohamed El Halaby [arxiv](http://arxiv.org/abs/1603.03814v1)
  > The paper conducts an experimental investigation to compare the practical performance of recent SAT-based and branch and bound algorithms for MaxSAT on standard benchmarks.
- **Trade-offs Between Time and Memory in a Tighter Model of CDCL SAT Solvers.** (2016) — Jan Elffers, Jan Johannsen, Massimo Lauria et al. [dblp](https://dblp.org/rec/conf/sat/ElffersJLMNV16)
- **Functional lower bounds for arithmetic circuits and connections to boolean circuit complexity** (2016) — Michael A. Forbes, Mrinal Kumar, Ramprasad Saptharishi [arxiv](http://arxiv.org/abs/1605.04207v1)
  > This paper proves exponential lower bounds for homogeneous depth-3 arithmetic circuits and for homogeneous depth-4 arithmetic circuits with bounded individual degree, for polynomials in VNP, using a n
- **Proof Complexity Lower Bounds from Algebraic Circuit Complexity** (2016) — Michael A. Forbes, Amir Shpilka, Iddo Tzameret et al. [arxiv](http://arxiv.org/abs/1606.05050v1)
  > The paper develops two general methods to convert certain algebraic circuit lower bounds into proof complexity lower bounds for subsystems of the Ideal Proof System (IPS), and uses these methods to ob
- **Polymorphisms and Circuit Complexity** (2016) — Gustav Nordh [arxiv](http://arxiv.org/abs/1609.04274v2)
  > The circuit complexity of a Boolean function is characterized by the partial polymorphisms of its truth table, and its non-deterministic circuit complexity is characterized by the polymorphisms of its
- **Complexity-Theoretic Foundations of Quantum Supremacy Experiments** (2016) — Scott Aaronson, Lijie Chen [arxiv](http://arxiv.org/abs/1612.05903v2)
  > The paper lays theoretical foundations for quantum supremacy experiments, showing that a non-sampling hardness assumption implies the impossibility of efficient classical algorithms passing statistica
- **Geometric complexity theory and matrix powering** (2016) — Fulvio Gesmundo, Christian Ikenmeyer, Greta Panova [arxiv](http://arxiv.org/abs/1611.00827v2)
  > In a new homogeneous formulation of Geometric Complexity Theory (GCT) that removes padding, there are no orbit occurrence obstructions capable of proving even superlinear lower bounds on the complexit
- **Boundaries of VP and VNP** (2016) — Joshua A. Grochow, Ketan D. Mulmuley, Youming Qiao [arxiv](http://arxiv.org/abs/1605.02815v1)
- **Statistical Query Lower Bounds for Robust Estimation of High-dimensional Gaussians and Gaussian Mixtures** (2016) — Ilias Diakonikolas, Daniel M. Kane, Alistair Stewart [arxiv](http://arxiv.org/abs/1611.03473v2)
  > The paper establishes the first Statistical Query (SQ) lower bounds for robust estimation of high-dimensional Gaussians and Gaussian mixtures, demonstrating a super-polynomial gap between information-
- **Targeted Pseudorandom Generators, Simulation Advice Generators, and Derandomizing Logspace** (2016) — William M. Hoza, Chris Umans [arxiv](http://arxiv.org/abs/1610.01199v4)
  > Under the assumption that for every derandomization result for logspace algorithms there is a strong enough pseudorandom generator, $\mathbf{BPL} \subseteq \bigcap_{\alpha> 0} \mathbf{DSPACE}(\log^{1 
- **NP-Hardness and Inapproximability of Sparse PCA** (2015) — Malik Magdon-Ismail [arxiv](http://arxiv.org/abs/1502.05675v2)
  > Sparse PCA is NP-hard, and unless P=NP, it does not admit an FPTAS; under weaker complexity assumptions, it also excludes polynomial constant-factor approximation algorithms.
- **On Asymptotic Gate Complexity and Depth of Reversible Circuits With Additional Memory** (2015) — Dmitry V. Zakablukov [arxiv](http://arxiv.org/abs/1505.02372v3)
- **Permanent v. determinant: an exponential lower bound assumingsymmetry and a potential path towards Valiant's conjecture** (2015) — Joseph M. Landsberg, Nicolas Ressayre [arxiv](http://arxiv.org/abs/1508.05788v2)
  > The paper demonstrates that Grenet's determinantal representation for the permanent is optimal among determinantal representations that respect left multiplication by permutation and diagonal matrices
- **TrackMania is NP-complete** (2014) — Franck Dernoncourt [arxiv](http://arxiv.org/abs/1411.5765v1)
  > Completing an untimed, unbounded track in TrackMania Nations Forever is NP-complete.
- **NP-hardness of hypercube 2-segmentation** (2014) — Uriel Feige [arxiv](http://arxiv.org/abs/1411.0821v1)
  > The paper provides a publicly available proof of NP-hardness for the hypercube 2-segmentation problem.
- **Lower Bounds for Tropical Circuits and Dynamic Programs** (2014) — Stasys Jukna [arxiv](http://arxiv.org/abs/1406.3065v2)
  > The paper presents lower bounds arguments for tropical circuits, which in turn apply to dynamic programming algorithms.
- **Multiplicative Complexity of Vector Valued Boolean Functions** (2014) — Magnus Gausdal Find, Joan Boyar [arxiv](http://arxiv.org/abs/1407.6169v3)
  > Functions with $n$ inputs and $n$ outputs achieving the highest nonlinearity must have at least $2.32n$ AND gates in $ΣΠΣ$ circuits, and while nonlinearity alone cannot yield stronger lower bounds, al
- **Forrelation: A Problem that Optimally Separates Quantum from Classical Computing** (2014) — Scott Aaronson, Andris Ambainis [arxiv](http://arxiv.org/abs/1411.5729v1)
  > The paper introduces the Forrelation problem, demonstrating an optimal separation between quantum and classical query complexities (1 quantum query vs. ~sqrt(N)/log(N) randomized queries), and proves 
- **Parameterized Complexity of CTL: A Generalization of Courcelle's Theorem** (2014) — Martin Lück, Arne Meier, Irina Schindler [arxiv](http://arxiv.org/abs/1410.4044v3)
  > The paper presents an almost complete classification of the parameterized complexity of all operator fragments of the satisfiability problem in computation tree logic (CTL), showing a dichotomy betwee
- **On the structure of the class NP** (2013) — Anatoly D. Plotnikov [arxiv](http://arxiv.org/abs/1304.1307v1)
  > The paper introduces a new class UF, strictly included in NP, and claims to prove that P is not equal to NP, suggesting that the problem 'P vs UF' should be considered instead of 'P vs NP'.
- **An exact algorithm for 1-in-3 SAT** (2013) — Édouard Bonnet, Vangelis Th. Paschos [arxiv](http://arxiv.org/abs/1307.5776v2)
  > An exact algorithm is presented that solves 1-in-3 SAT in time $O^*(1.260^n)$.
- **Computational Lower Bounds for Sparse PCA** (2013) — Quentin Berthet, Philippe Rigollet [arxiv](http://arxiv.org/abs/1304.0828v2)
  > The paper proves a statistical price for computational efficiency in sparse PCA, showing that the performance of their semidefinite programming test cannot be strictly improved by any computationally 
- **Superpolynomial lower bounds for general homogeneous depth 4 arithmetic circuits** (2013) — Mrinal Kumar, Shubhangi Saraf [arxiv](http://arxiv.org/abs/1312.5978v1)
- **A reduction of proof complexity to computational complexity for $AC^0[p]$ Frege systems** (2013) — Jan Krajicek [arxiv](http://arxiv.org/abs/1311.2501v4)
  > This paper presents a general reduction that transforms lengths-of-proofs lower bounds for AC^0[p] Frege systems into computational complexity lower bounds for search tasks involving search trees bran
- **Unifying Known Lower Bounds via Geometric Complexity Theory** (2013) — Joshua A. Grochow [semantic_scholar](https://www.semanticscholar.org/paper/1fd28639199818f073daa3ab5bfe6efe8a1590f8)
  > This paper demonstrates that most known algebraic circuit lower bounds and their interrelations naturally fit into the representation-theoretic framework of Geometric Complexity Theory (GCT), showing 
- **Determinant versus Permanent: salvation via generalization? The algebraic complexity of the Fermionant and the Immanant** (2013) — Nicolas de Rugy-Altherre [arxiv](http://arxiv.org/abs/1309.2156v1)
  > The fermionant is VNP-complete for most cases and #P-complete for specific cases, while the immanant of any family of Young diagrams with bounded width and at least n boxes at the right of the first c
- **Arithmetic Circuit Lower Bounds via MaxRank** (2013) — Mrinal Kumar, Gaurav Maheshwari, Jayalal Sarma M. N [arxiv](http://arxiv.org/abs/1302.3308v1)
  > The paper proves that any homogeneous depth-3 circuit for computing the product of $d$ matrices of dimension $n 	imes n$ requires $Ω(n^{d-1}/2^d)$ size, improving previous lower bounds by Nisan and Wi
- **Computation Environments, An Interactive Semantics for Turing Machines (which P is not equal to NP considering it)** (2012) — Rasoul Ramezanian [arxiv](http://arxiv.org/abs/1205.5994v1)
  > The equality of complexity classes P and NP in a persistently evolutionary computation environment (E_e) conflicts with the free will of the computist.
- **NP-Completeness of deciding the feasibility of Linear Equations over binary-variables with coefficients and constants that are 0, 1, or -1** (2012) — Deepak Ponvel Chermakani [arxiv](http://arxiv.org/abs/1210.4120v2)
  > Deciding the feasibility of a system of linear equations with binary variables and coefficients/constants restricted to {0, 1, -1} is strongly NP-Complete.
- **Classic Nintendo Games are (Computationally) Hard** (2012) — Greg Aloupis, Erik D. Demaine, Alan Guo et al. [arxiv](http://arxiv.org/abs/1203.1895v3)
  > The paper proves NP-hardness for generalized versions of five major Nintendo game franchises (Mario, Donkey Kong, Legend of Zelda, Metroid, Pokemon) and PSPACE-completeness for Donkey Kong Country and
- **Packing Trominoes is NP-Complete, #P-Complete and ASP-Complete.** (2012) — Takashi Horiyama, Takehiro Ito, Keita Nakatsuka et al. [dblp](https://dblp.org/rec/conf/cccg/HoriyamaINSU12)
- **Generalizing and Derandomizing Gurvits's Approximation Algorithm for the Permanent** (2012) — Scott Aaronson, Travis Hance [arxiv](http://arxiv.org/abs/1212.0025v2)
  > The paper generalizes Gurvits's permanent approximation algorithm to yield better approximations for matrices with repeated rows or columns, and derandomizes the algorithm (and its generalization) for
- **Explicit lower bounds via geometric complexity theory** (2012) — Peter Bürgisser, Christian Ikenmeyer [semantic_scholar](https://www.semanticscholar.org/paper/85905aff9ab53f2e104892179d70871e235faf89)
  > A lower bound of R Mm) ≥ 3/2 m2-2 is proven for the border rank of m x m matrix multiplication.
- **Geometric Complexity Theory V: Equivalence between Blackbox Derandomization of Polynomial Identity Testing and Derandomization of Noether&apos;s Normalization Lemma.** (2012) — Ketan Mulmuley [dblp](https://dblp.org/rec/conf/focs/Mulmuley12)
- **Kernelization Lower Bounds By Cross-Composition** (2012) — Hans L. Bodlaender, Bart M. P. Jansen, Stefan Kratsch [arxiv](http://arxiv.org/abs/1206.5941v1)
- **Better Pseudorandom Generators from Milder Pseudorandom Restrictions** (2012) — Parikshit Gopalan, Raghu Meka, Omer Reingold et al. [arxiv](http://arxiv.org/abs/1210.0049v1)
  > This paper presents an iterative approach using mild pseudorandom restrictions to construct pseudorandom generators for combinatorial rectangles and read-once CNFs, and a hitting set generator for wid
- **Lee-Yang theorems and the complexity of computing averages** (2012) — Alistair Sinclair, Piyush Srivastava [arxiv](http://arxiv.org/abs/1211.2376v2)
  > The average quantities related to spin systems, such as mean magnetization, susceptibility, and average dimer count, are #P-hard to compute.
- **On the relationship between classes P and NP** (2011) — Anatoly D. Plotnikov [arxiv](http://arxiv.org/abs/1109.5531v1)
  > The paper claims that the difficulties in solving the P versus NP problem are methodological, stemming from the sensitivity of algorithms to problem formulation, particularly for some problems within 
- **Inclusion of Unambiguous RE#s is NP-Hard** (2011) — Pekka Kilpeläinen [arxiv](http://arxiv.org/abs/1111.0422v1)
  > Testing inclusion between languages represented by unambiguous regular expressions with numerical occurrence indicators (RE#s) is NP-hard.
- **Short Proofs for the Determinant Identities** (2011) — Pavel Hrubes, Iddo Tzameret [arxiv](http://arxiv.org/abs/1112.6265v2)
  > The paper establishes that arithmetic circuit proofs (P_c(F)) can be balanced to achieve polynomial size and reduced depth, leading to a quasipolynomial simulation of P_c(F) by P_f(F) for polynomial-d
- **Quantum Copy-Protection and Quantum Money** (2011) — Scott Aaronson [arxiv](http://arxiv.org/abs/1110.5353v1)
  > There exist quantum oracles relative to which publicly-verifiable quantum money is possible, and any family of functions that cannot be efficiently learned from its input-output behavior can be quantu
- **Advice Coins for Classical and Quantum Computation** (2011) — Scott Aaronson, Andrew Drucker [arxiv](http://arxiv.org/abs/1101.5355v1)
  > The classes BPPSPACE/coin and BQPSPACE/coin, representing classical and quantum polynomial-space computation with advice coins, both coincide with PSPACE/poly.
- **A zero-one SUBEXP-dimension law for BPP** (2011) — Philippe Moser [arxiv](http://arxiv.org/abs/1101.4848v1)
  > BPP either has SUBEXP-dimension zero (implying randomness is easy) or BPP=EXP (implying randomness is intractable), establishing a zero-one law for BPP based on SUBEXP-dimension.
- **Applications of Monotone Rank to Complexity Theory** (2011) — Yang D. Li [arxiv](http://arxiv.org/abs/1102.2932v2)
  > The paper demonstrates that monotone rank provides unconditional bounds and solutions to open problems across algebraic complexity, quantum computing, and communication complexity, including a super-e
- **A strong direct product theorem for quantum query complexity** (2011) — Troy Lee, Jérémie Roland [arxiv](http://arxiv.org/abs/1104.4468v3)
  > Quantum query complexity satisfies a strong direct product theorem, showing that computing multiple copies of a function or their parity requires nearly proportional quantum queries, otherwise success
- **Bounds on Threshold of Regular Random $k$-SAT** (2010) — Vishwambhar Rathi, Erik Aurell, Lars Rasmussen et al. [arxiv](http://arxiv.org/abs/1002.1290v3)
  > The paper derives upper and lower bounds on the satisfiability threshold and NAE-satisfiability threshold for regular random $k$-SAT, showing that these bounds match those for the uniform model and an
- **On Universal Complexity Measures** (2010) — John Scoville [arxiv](http://arxiv.org/abs/1005.2254v9)
  > The paper proposes a universal complexity measure for finite strings based on universal representations of their underlying symmetries, classifying binary strings via their automorphism groups and gen
- **A Full Characterization of Quantum Advice** (2010) — Scott Aaronson, Andrew Drucker [arxiv](http://arxiv.org/abs/1004.0377v2)
  > Quantum advice (BQP/qpoly) is exactly characterized as equivalent in power to untrusted quantum advice combined with trusted classical advice, implying BQP/qpoly is contained in QMA/poly.
- **A note about a partial no-go theorem for quantum PCP** (2010) — Itai Arad [arxiv](http://arxiv.org/abs/1012.3319v2)
  > The paper derives an upper bound on the maximal promise gap for the quantum PCP conjecture, showing it shrinks as the system's non-commuteness decreases.
- **A Dichotomy Theorem for the Approximate Counting of Complex-Weighted Bounded-Degree Boolean CSPs** (2010) — Tomoyuki Yamakami [arxiv](http://arxiv.org/abs/1008.2688v3)
  > A dichotomy theorem is presented that classifies the computational complexity of approximately counting complex-weighted Boolean CSPs with bounded degree (greater than two) and unary constraints into 
- **On P vs. NP, Geometric Complexity Theory, Explicit Proofs and the Complexity Barrier** (2009) — Ketan D. Mulmuley [arxiv](http://arxiv.org/abs/0908.1932v2)
  > This article provides a complexity-theoretic overview of Geometric Complexity Theory (GCT) as an approach to the P vs. NP problem, making it accessible without prior background in algebraic geometry o
- **About the impossibility to prove P=NP and the pseudo-randomness in NP** (2009) — M. Rémon [arxiv](http://arxiv.org/abs/0904.0698v3)
  > The paper claims that the P!=NP assertion is impossible to prove within the a-temporal framework of Mathematics.
- **An axiomatic approach to algebrization** (2009) — R. Impagliazzo, Valentine Kabanets, A. Kolokolova [semantic_scholar](https://www.semanticscholar.org/paper/29125ea3299dd583bc9f019bb9db3ab610e3674a)
  > The paper proposes an axiomatic approach to algebrization, extending the AIV92 theory with a new axiom called "Arithmetic Checkability," which formalizes algebrizing techniques by stating that NP lang
- **Algebrization: A New Barrier in Complexity Theory.** (2009) — Scott Aaronson, Avi Wigderson [dblp](https://dblp.org/rec/journals/toct/AaronsonW09)
- **A Complex Analogue of Toda’s Theorem** (2009) — S. Basu [semantic_scholar](https://www.semanticscholar.org/paper/7847d703c662c7cb801e590a5964797c184beda4)
  > This paper establishes a complex analogue of Toda’s theorem, demonstrating that the (compact) polynomial hierarchy over complex numbers is contained in a class analogous to P#P, enabled by the efficie
- **On P vs. NP, Geometric Complexity Theory, and the Riemann Hypothesis** (2009) — Ketan D. Mulmuley [arxiv](http://arxiv.org/abs/0908.1936v2)
  > The paper provides a mathematical overview and research plan for Geometric Complexity Theory (GCT) as an approach to the P vs. NP problem, based on a series of lectures.
- **Two-message quantum interactive proofs are in PSPACE** (2009) — Rahul Jain, Sarvagya Upadhyay, John Watrous [arxiv](http://arxiv.org/abs/0905.1300v1)
  > The class of problems solvable by two-message quantum interactive proof systems, QIP(2), is a subset of PSPACE.
- **Pseudorandom Generators Against Advised Context-Free Languages** (2009) — Tomoyuki Yamakami [arxiv](http://arxiv.org/abs/0902.2774v4)
  > The paper explicitly constructs an almost one-to-one pseudorandom generator (PRG) that stretches $n$-bit seeds to $n+1$ bits, fools advised context-free languages (CFL/n), is computed in logarithmic s
- **A complex analogue of Toda's Theorem** (2009) — Saugata Basu [arxiv](http://arxiv.org/abs/0912.2652v7)
  > The paper extends techniques from previous work to the complex projective case, obtaining a complex analogue of Toda's theorem, which shows that the (compact) polynomial hierarchy over complex numbers
- **Independence of P vs. NP in regards to oracle relativizations** (2008) — Jerrald Meek [arxiv](http://arxiv.org/abs/0805.2170v6)
  > The solution to the P vs. NP problem is independent of oracle relativizations.
- **Almost-natural proofs** (2008) — Timothy Y. Chow [arxiv](http://arxiv.org/abs/0805.1385v3)
  > If the largeness condition for natural proofs is slightly weakened, then the Razborov-Rudich barrier breaks down, and such 'almost-natural' properties provably exist and can separate P/poly from NP un
- **Polynomial Hierarchy, Betti Numbers, and a Real Analogue of Toda’s Theorem** (2008) — S. Basu, T. Zell [semantic_scholar](https://www.semanticscholar.org/paper/aa140de3185d13841aa5f0a939ecff9690ffdc16)
  > The paper formulates and proves a real analogue of Toda’s theorem, showing that the real polynomial hierarchy is contained in a real version of P#P, and as a consequence, provides a polynomial time re
- **Reduced Kronecker coefficients and counter-examples to Mulmuley's strong saturation conjecture SH** (2008) — Emmanuel Briand, Rosa Orellana, Mercedes Rosas [arxiv](http://arxiv.org/abs/0810.3163v3)
  > The paper provides counter-examples to Mulmuley's strong saturation conjecture (strong SH) for Kronecker coefficients and proves the #P-hardness of computing Kronecker coefficients.
- **ASP, The Art and Science of Practice: Appeal to NP-Completeness Considered Harmful: Does the Fact That a Problem Is NP-Complete Tell Us Anything?** (2007) — Constantine N. Goulimis [dblp](https://dblp.org/rec/journals/interfaces/Goulimis07)
- **Geometric Complexity Theory V: On deciding nonvanishing of a generalized Littlewood-Richardson coefficient** (2007) — Ketan D. Mulmuley Hariharan Narayanan [arxiv](http://arxiv.org/abs/0704.0213v2)
  > The paper, originally titled 'Geometric Complexity Theory V: On deciding nonvanishing of a generalized Littlewood-Richardson coefficient,' was withdrawn because its content was merged with an earlier 
- **Geometric Complexity Theory: Introduction** (2007) — Ketan D. Mulmuley, Milind Sohoni [arxiv](http://arxiv.org/abs/0709.0746v1)
  > This paper provides an introductory overview of Geometric Complexity Theory (GCT) and its foundational concepts, including invariant theory, for graduate students without prior background in algebraic
- **On P vs. NP, Geometric Complexity Theory, and the Flip I: a high level view** (2007) — Ketan D. Mulmuley [arxiv](http://arxiv.org/abs/0709.0748v1)
  > This article provides a high-level exposition of the basic plan of Geometric Complexity Theory (GCT) for P vs. NP, based on the principle called the flip.
- **Geometric Complexity Theory VI: the flip via saturated and positive integer programming in representation theory and algebraic geometry** (2007) — Ketan Mulmuley [dblp](https://dblp.org/rec/journals/corr/abs-0704-0229)
- **Interpolation in Valiant's theory** (2007) — Pascal Koiran, Sylvain Perifel [arxiv](http://arxiv.org/abs/0710.0360v1)
  > The paper investigates the relationship between boolean and algebraic complexity by analyzing whether polynomials evaluable efficiently by boolean algorithms have small arithmetic circuits, showing it
- **On the expressive power of planar perfect matching and permanents of bounded treewidth matrices** (2007) — Laurent Lyaudet, Pascal Koiran, Uffe Flarup [arxiv](http://arxiv.org/abs/0705.3751v1)
  > The permanent and hamiltonian polynomials for matrices of bounded treewidth are shown to be equivalent to arithmetic formulas, and arithmetic weakly skew circuits are shown to be equivalent to the sum
- **Mastermind is NP-Complete** (2005) — Jeff Stuckman, Guo-Qiang Zhang [arxiv](http://arxiv.org/abs/cs/0512049v1)
  > The Mastermind Satisfiability Problem (MSP) is NP-complete.
- **Geometric Complexity III: on deciding positivity of Littlewood-Richardson coefficients** (2005) — Ketan D. Mulmuley, Milind Sohoni [arxiv](http://arxiv.org/abs/cs/0501076v1)
  > The problem of deciding positivity of Littlewood-Richardson coefficients for GLn(C) is shown to belong to P, with a strongly polynomial algorithm.
- **Logarithmic Lower Bounds in the Cell-Probe Model** (2005) — Mihai Patrascu, Erik D. Demaine [arxiv](http://arxiv.org/abs/cs/0502041v2)
  > The paper develops a new technique to prove amortized randomized Omega(lg n) lower bounds per operation for dynamic data structures in the cell-probe model, applicable to problems like partial sums an
- **$P \ne NP$, propositional proof complexity, and resolution lower bounds for the weak pigeonhole principle** (2003) — Ran Raz [arxiv](http://arxiv.org/abs/cs/0304041v1)
  > Exponential lower bounds of $Ω(2^{n^ε})$ were established for the length of any Resolution proof for the weak pigeonhole principle with $n$ holes, implying that certain propositional formulations of $
- **A New Multilayered PCP and the Hardness of Hypergraph Vertex Cover** (2003) — Irit Dinur, Venkatesan Guruswami, Subhash Khot et al. [arxiv](http://arxiv.org/abs/cs/0304026v1)
- **Hardness as randomness: a survey of universal derandomization** (2003) — Russell Impagliazzo [arxiv](http://arxiv.org/abs/cs/0304040v1)
  > Proving that probabilistic algorithms have non-trivial deterministic simulations is basically equivalent to proving circuit lower bounds, either in the algebraic or Boolean models.
- **Counting complexity classes for numeric computations II: algebraic and semialgebraic sets** (2003) — Peter Buergisser, Felipe Cucker [arxiv](http://arxiv.org/abs/cs/0312007v1)
  > The paper defines counting complexity classes #P_R and #P_C in the Blum-Shub-Smale model and shows that computing topological invariants of (semi)algebraic sets are complete problems for these classes
- **The SAT Phase Transition** (2000) — Ke Xu, Wei Li [arxiv](http://arxiv.org/abs/cs/0005024v2)
  > For random k-SAT model, it is proved that as the ratio of clauses to variables (r) increases, the structure of solutions undergoes a sudden change, like a satisfiability phase transition, when r reach
- **A Lower Bound on the Average-Case Complexity of Shellsort** (1999) — Tao Jiang, Ming Li, Paul Vitanyi [arxiv](http://arxiv.org/abs/cs/9906008v2)
  > The average number of data-movements (and comparisons) made by a $p$-pass Shellsort for any incremental sequence is $Ω(pn^{1 + 1/p})$ for every $p$.
- **What&apos;s Up with Downward Collapse: Using the Easy-Hard Technique to Link Boolean and Polynomial Hierarchy Collapses** (1999) — Edith Hemaspaandra, Lane A. Hemaspaandra, Harald Hempel [dblp](https://dblp.org/rec/journals/corr/cs-CC-9910002)
- **PSPACE has 2-round quantum interactive proof systems** (1999) — John Watrous [arxiv](http://arxiv.org/abs/cs/9901015v1)
  > It is proved that every language in PSPACE has a quantum interactive proof system that requires only two rounds of communication between the prover and verifier, while having exponentially small (one-
- **Dense Quantum Coding and a Lower Bound for 1-way Quantum Automata** (1998) — Andris Ambainis, Ashwin Nayak, Amnon Ta-Shma et al. [arxiv](http://arxiv.org/abs/quant-ph/9804043v2)
  > The paper shows that non-trivial quantum encodings exist that have no classical counterparts, but quantum encodings cannot be much more succinct than classical ones, providing a lower bound that is th
- **Natural Proofs.** (1997) — Alexander A. Razborov, Steven Rudich [dblp](https://dblp.org/rec/journals/jcss/RazborovR97)
- **Natural Proofs** (1994) — Alexander A. Razborov, Steven Rudich [dblp](https://dblp.org/rec/journals/eccc/ECCC-TR94-010)
- **Erratum: The Polynomial Time Hierarchy Collapses if the Boolean Hierarchy Collapses.** (1991) — Jim Kadin [dblp](https://dblp.org/rec/journals/siamcomp/Kadin91)
- **The Polynomial Time Hierarchy Collapses if the Boolean Hierarchy Collapses.** (1988) — Jim Kadin [dblp](https://dblp.org/rec/journals/siamcomp/Kadin88)
