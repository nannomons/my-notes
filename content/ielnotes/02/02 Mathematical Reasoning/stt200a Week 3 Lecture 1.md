---
title: introduction to Logic
publish: true
tags:
Subject:
  - Mathematical Reasoning
Course:
  - STT200A
Type: Lecture Notes
Difficulty: 100
Date: 2025-09-16
---
# Defn. Statements or Propositions
- A **statement or proposition** is a declarative sentence that is either *definitely true* or *definitely false*. 
	- The **truth value** of a proposition is either true (**T**) or false (**F**), but not both. 
	- *Letters*, such as $p, q, r$ are used to *represent propositions*. 
	- **Propositional calculus** is the area of logic that deals with propositions.

E.g. *Statement:* Seth Cordeta is from BS Stats. *Truth Value:* T. 

# Defn. Compound Statements
- A **compound statement** is composed of one or more propositions and at least one *logical connective*.  
- A **truth table** is used to display the truth values of every possible combination of truth values of the statements that form a compound proposition.

# Defn. Logical Operators
- **Negation of p**: $\neg p$, or *~$p$*, read as *not p* or *it is not the case that p*
- **[[Conjunction]] of p**: $p \wedge q$, combine proposition w/ "and", *true only if both are true*
- **Inclusive [[Disjunction]] of p and q**: $p \vee q$, *true if p or q or both is true* 
- **Exclusive [[Disjunction]] of p and q**: $p \oplus q$ or $p\bar{\vee} q$, *true if only p or q is true* 

![[Pasted image 20250916144739.png]]
# Defn. Conditional Statement
- Let $p$ and $q$ be [[Proposition]]s. The **conditional statement** (also called an *implication*) $p \implies q$ is the proposition 
	- where $p$ is called the **hypothesis or antecedent or premise**, and
	- $q$ is called the **conclusion or consequence**.

## Other ways to express $p \implies q$
1. if p, q
2. q if p
3. q whenever p
4. q when p
5. p is sufficient for q*
6. a sufficient condition for p is q*
7. q is necessary for p**
8. a necessary condition for q is p**
9. p implies q
10. q follows from p
11. q unless $\neg p$ 
12. q if not $\neg p$
13. q only if p

- *Note: 5 and 6 are both using the term **sufficient**, meaning if q is proven to be true, then p could automatically be proven true.*
- *Note: 7 and 8 are both using the term **necessary**, meaning if p happened, then q has happened or will happen as well.
## Other forms of Conditional Statements 
- The **converse** of $p \implies q$ is $q \implies p$
- The **inverse** of $p \implies q$ is $\neg p \implies q$
- The **[[Contrapositive]]** of $p \implies q$ is $\neg q \implies \neg p$  
- The **negation** of $p \implies q$ is $p \wedge q$, which is $\neg(p \implies q)$

![[Pasted image 20250916145655.png]]
# Defn. Biconditional Statements

- Let $p$ and $q$ be [[Proposition]]s. The **biconditional** (also called a *bi-implication*) $p \iff q$ is the proposition "*p if and only if q*"
	- which is true if both p and q *have the same truth values*.

## Other ways to express $p \iff q$
1. p is necessary and sufficient for q
2. if p then q, and conversely
3. p iff q, *iff is read as if and only if*

# Defn. Compound Proposition

- A **compound proposition** is a 
	- **tautology** ($p \equiv q$) — if it is *true for all possible combinations of truth values* of the component statements
	- **contradiction** or **absurdity** — if it is *false for all possible combinations of truth values* of the component statements
	- **contingency** — if it is neither a tautology or contradiction 

## Defn. Logical equivalents
- The compound propositions p and q are called logically equivalent if $p \iff q$ is a **tautology**.

# Thm. Logical Identities (Rules of Replacement)
- Given propositions $pqr$, tautology $t$, and contradiction $c$, the following logical equivalencies hold:
1. **Commutative Laws**: $p \wedge \equiv q \wedge p$, **OR** $p \vee q \equiv q \vee p$
2. **Associative Laws**: $(p \wedge q) \wedge r \equiv p\wedge(q \wedge r)$, **OR** $(p \vee q) \vee r\equiv p\vee (q \vee r)$ 
3. **Distributive Laws**: $p \wedge(q \vee r)\equiv(p\wedge q)\vee(p \wedge r)$, **OR** $p \vee (q \wedge r)\equiv(q \vee p) \wedge(p \vee r)$ [[HW MATH REASONING]] 
4. **Identity Laws**: $p \wedge t \equiv p$, **OR** $p \vee c \equiv p$ 
5. **Negation Laws** or *Rule of Excluded Middle*: $p \vee \neg p \equiv t$, **OR** $p \wedge \neg p \equiv c$
6. **Double Negative Laws**: $\neg(\neg p) \equiv p$
7. **Idempotent Laws**: $p \wedge p \equiv p$, **OR** $p \vee p \equiv p$
8. **Universal Bound Laws** or *Domination Laws*: $p \vee t \equiv t$ **OR** $p \wedge c \equiv t$
9. **[[De Morgan]]'s Laws**: $\neg(p\wedge q) \equiv \neg p \vee \neg q$, **OR** $\neg (p \vee q) \equiv \neg p \wedge \neg q$ [[HW MATH REASONING]]
10. **Absorption Laws**: $p \vee (p \wedge q) \equiv p$ **OR** $p \wedge  (p \vee q) \equiv p$
11. **Negations of t and c**: $\neg t \equiv c$, **OR** $\neg c \equiv t$
12. **[[Material Implication]]**: $p \implies q \equiv \neg p \vee q$ [[HW MATH REASONING]] 
13. **Material Equivalence**: $p \iff q \equiv (p \implies q) \wedge (q \implies p)$
14. **Contrapositive** or *Transposition*: $p \implies q \equiv \neg q \implies \neg p$ 