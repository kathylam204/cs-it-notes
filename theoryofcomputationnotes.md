# Theory of Computation

## Logic and Proofs
Propositions
Proposition: A statement that is either true or false.
Example: "0 = 1" (false), "peanut butter is a source of protein" (true).
Proposition with Free Variable: Its truth value depends on the variable's value.
Example: "x - 1 is prime" (true for x = 8, false for x = 10).

## Logical Connectives
Conjunction (∧): x∧y means "x and y".
Disjunction (⋁): x∨y means "x or y".
Negation (¬): ¬x means "not x".
Conditional (→): x→y means "if x then y".
Biconditional (↔): x↔y means "x if and only if y".

## Truth Tables
Negation: The truth value of ¬p is the opposite of p.
Conditional: If p is true, p→q takes the value of q. If p is false, p→q is true regardless of q.

## Special Propositions
Tautology: Always true. Example: p∨¬p.
Contradiction: Always false. Example: p∧¬p.
Logical Equivalence: P↔Q means P and Q have the same truth value.
Logical Implication: P⇒Q means P→Q is a tautology.

## Logical Identities
### Commutative Laws:
p∨q↔q∨p
p∧q↔q∧p
### Associative Laws:
p∨(q∨r)↔(p∨q)∨r
p∧(q∧r)↔(p∧q)∧r
### Distributive Laws:
p∨(q∧r)↔(p∨q)∧(p∨r)
p∧(q∨r)↔(p∧q)∨(p∧r)
### De Morgan's Laws:
¬(p∨q)↔¬p∧¬q
¬(p∧q)↔¬p∨¬q
### Conditionals and Biconditionals:
(p→q)↔(¬p∨q)
(p→q)↔(¬q→¬p)
(p↔q)↔((p→q)∧(q→p))

## Quantifiers
Universal Quantifier (∀): "For every" or "for all".
Example: ∀x(x−1 is prime)
Existential Quantifier (∃): "There exists" or "for some".
Example: ∃x(x−1 is prime)

## Proof Techniques
Direct Proof: Uses definitions and previously established statements.
Example: Prove ab is odd if a and b are odd.
Indirect Proof (Contrapositive): Proves ¬Q→¬P.
Example: Prove ij=n→i≤ n∨j≤n .
Proof by Contradiction: Assumes the negation of the statement and derives a contradiction.
Example: Prove 2 is irrational.
Proof by Cases: Enumerates and proves all possible cases.
Example: Prove a proposition P→Q using truth tables.

## Sets
Definitions
Set: A collection of distinct elements.
Examples: A={1,2,4,8}, B={0,3,6,9,…}.
Element Membership: x∈A means x is an element of A.
Subset: A⊆B means every element of A is in B.
Empty Set: ∅ contains no elements.

## Operations
Union: A∪B={x∣x∈A∨x∈B}
Intersection: A∩B={x∣x∈A∧x∈B}
Difference: A−B={x∣x∈A∧xB}
Complement: A ′ =U−A, where U is the universal set.

## Properties
Commutative: A∪B=B∪A, A∩B=B∩A
Associative: A∪(B∪C)=(A∪B)∪C, A∩(B∩C)=(A∩B)∩C
Distributive: A∪(B∩C)=(A∪B)∩(A∪C), A∩(B∪C)=(A∩B)∪(A∩C)

## Special Sets
Power Set: The set of all subsets of A, denoted 2^A.
Cartesian Product: A×B={(a,b)∣a∈A,b∈B}

## Functions and Equivalence Relations
Functions
Function f:A→B: Assigns each element of A to one element of B.
Range: {f(x)∣x∈A}
Bijection: A function that is both one-to-one and onto.
Inverse Function: f −1 if f is a bijection.

## Equivalence Relations
Reflexive: xRx for all x∈A.
Symmetric: xRy→yRx for all x,y∈A.
Transitive: xRy∧yRz→xRz for all x,y,z∈A.

## Equivalence Classes
Equivalence Class: The set of all elements related to x.
Partition: A set of pairwise disjoint sets whose union is A.

## Languages
Alphabet and Strings
Alphabet: A finite set of symbols, Σ={a,b,c}.
String: A finite sequence of symbols from Σ.
Null String: ϵ, the string of length 0.
Language: A set of strings over an alphabet Σ.

## Operations
Concatenation: xy is the concatenation of strings x and y.
Union: L1∪L2
Intersection: L1∩L2
Difference: L1−L2
Complement: Σ∗−L
Kleene Star: L∗ is the set of all strings obtained by concatenating zero or more strings in L.

## Recursive Definitions
Recursive Definition: Defines a set with a basis statement and a recursive part.
Example: N defined by 0∈N and n∈N→n+1∈N.

## Structural Induction
Structural Induction: Proves properties of recursively defined sets.

## Indistinguishability and DFA Minimization
State Numbering: Use a grid of size n-1 where n is the number of nodes. E.g., for 10 nodes, use a 9x9 grid.
Labeling: Start with 0 at the bottom and 1 on the side. Ensure correct grid formation.
Marking: Nodes cannot be marked if both are accepting. One must be in and one out. Permanent blanks are not marked.

## Control Flow Testing
Inputs: Source code.
Path Selection Criteria: Statement, branch.
Control Flow Graph (CFG): Visual representation of a program's paths.
CFG Generation: Modified compilers produce CFGs.
Path Selection: Ensure paths justify selection criteria (entry/exit).
Path Types:
Executable Path: Can be executed with input.
Infeasible Path: Cannot be executed.
Decision Points:
Decision point (triangle)
Sequential computation (rectangle)
Merge point (circle)
Coverage Criteria:
All paths.
Complete statement coverage.
Complete branch coverage.
Predicate coverage.

## Regular Expressions and Kleene’s Theorem
Regular Languages: Can be described using union, concatenation, and Kleene star operations.
Examples:
Strings ending in aa: {a,b}* aa
Strings containing ab or bba: {a,b}* {ab, bba} {a,b}*
Language {a,b}* {aa, aab}* {b}
Definition:
For alphabet Σ, the set R of regular languages over Σ includes the empty set and languages formed by union, concatenation, and Kleene star operations.

## NFAs and Null Closures
Null Closure:
For NFA M = (Q, Σ, q0, A, δ), the null closure of a set S is recursively defined as S ⊆ (S) where (q, ε) ⊆ Λ(S) for every q ∈ S.
Extended Transition Function:
For every q ∈ Q, *(q, ε) = {q}
For every q ∈ Q, every y ∈ Σ*, and every a ∈ Σ, *(q, y) = (∪ {(p, ε) | p ∈ *(q, y)})
Acceptance: A string x ∈ Σ* is accepted if *(q0, x) ∩ A ≠ ∅.

## NFA Nondeterminism
Types of Nondeterminism:
Different arcs for the same input symbol.
ε-transitions.
Elimination:
Introduce new transitions to eliminate ε-transitions, potentially increasing other forms of nondeterminism.

## Context-Free Grammars (CFGs)
Purpose: Describe languages more complex than regular languages, including many programming languages.
CFG Definition: A 4-tuple G = (V, Σ, S, P):
V and Σ are finite, disjoint sets.
S ∈ V is the start variable.
P is a set of production rules A → α where A ∈ V and α ∈ (V ∪ Σ)*.
Language Generated: L(G) = {x ∈ Σ* | S ⇒* x}.
Properties:
Closure Properties: If L1 and L2 are CFLs, then L1 ∪ L2, L1L2, and L1* are also CFLs.
Grammar Combination: Combine CFGs for union, concatenation, and Kleene star.
Derivations: Use derivation trees to show grammar rules and structures.
