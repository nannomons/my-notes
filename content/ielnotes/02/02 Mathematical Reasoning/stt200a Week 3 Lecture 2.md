---
title: Quantifiers and Methods of Proof
publish: true
tags:
Subject:
  - Mathematical Reasoning
Course:
  - STT200A
Type: Lecture Notes
Difficulty:
Date: 2025-09-19
---
# Defn. [[Propositional Function]]
A *declarative sentence* whose truth value depends on the value of *one or more variables* is called a **propositional function**.

## Notes
1. A propositional function $P(x)$ has a well-defined truth value for each value of $x$ in $D$ or the **domain of discourse**. 
2. The set of all values $x \in D$ that make $P(x)$ true is called the **truth set**.
3. In a propositional function $P(x)$, $x$ is called a **free variable**.
4. In a quantified statement, $x$ is called a **bound variable**.
5. The **scope** of the quantifier is the part of a logical expression to which a quantifier is applied. 

# Defn. 
Let $D$ be the **domain of discourse**.

## Defn. Universal Quantification
The **universal quantification** of $P(x)$ is the statement $\forall x \in D, P(x)$.
- For all
- For every
- For each 
- All of
- Given any
- For arbitrary

## Defn. Existential Quantification
The **existential quantification** of $P(x)$ is the statement $\exists x \in D, P(x)$.
- For some
- There is
- For at least some
- There is at least one
- There exists

## Defn. Uniqueness Quantification
The **uniqueness quantification** of $P(x)$ is the statement $\exists!x \in D, P(x)$. 
- There exists a unique
- There is a unique
- For a unique

## Notes
- If the **domain is empty**, then $\forall x,P(x)$ is **true** for any propositional function $P(x)$ because there are no elements $x \in D$ for which $P(x)$ is false (aka *vacuously true* or *true by default*). 
- If the **domain is empty**, then $\exists x, P(x)$ is **false** whenever $P(x)$ whenever $P(x)$ is a propositional function because there can be no element $x \in D$ for which $P(x)$ is true. 

- When all elements in the domain can be listed, say, $x_{1},\dots,x_{n}$, then $\forall x, P(x)$ is the same as the [[Conjunction]]. 
- When all elements in the domain can be listed, say, $x_{1},\dots,x_{n}$, then $\exists x, P(x)$ is the same as the [[Disjunction]].

- $\exists_{2}$ is used for **two unique elements**, $\exists_{3}$ for three, $\exists_{4}$ for four, and so on.
- The **quantifiers have higher precedence** than all logical operators from propositional calculus, for example, $\forall x,P(x) \wedge Q(x)$ is not the same as $\forall x,(P(x) \wedge Q(x))$. 

- The **universal conditional statement** $\forall x,(P(x) \implies Q(x))$ also has a universally quantified converse, inverse, or contrapositive. 

- $\forall x \in D, P(x) \equiv \forall x, (x \in D \implies P(x))$ 
- $\exists x \in D, P(x) \equiv, (x \in D \wedge P(x))$ 

# Thm. [[De Morgan]]'s Law for Quantifiers 
- $\neg(\forall x. P(x)) \equiv \exists x,, \neg P(x)$ ; Read as *"Not all"* or *"Some are not"*
- $\neg(\exists x, P(x))\equiv \forall x,\neg P(x)$ ; Read as *"There does not exist"* or *"It is not the case that"* 

# Defn. Nested Quantifiers
Let $D_{1}$ and $D_{2}$ be the domains of discourse where $x \in D_{1} \cap y \in D_{2}$.


|                                                               | TRUE                                                       | FALSE                                                       |
| ------------------------------------------------------------- | ---------------------------------------------------------- | ----------------------------------------------------------- |
| $\forall x,\exists y,P(x, y)$                                 | For every $x$, there is a $y$ for which $P(x, y)$ is true. | There is an $x$ such that $P(x, y)$ is false for every $y$. |
| $\exists x. \forall x, P(x,y)$                                | There is an $x$ for which $P(x,y)$ is true for all $y$.    | For every $x$, there is a $y$ for which $P(x,y)$ is false.  |
| $\forall x, \forall y, P(x,y)$ $\forall y,\forall x, P(x,y)$  | $P(x,y)$ is true for every pair $(x,y)$.                   | There is a pair $(x, y)$ for which $P(x,y)$ is false.       |
| $\exists x, \exists y, P(x,y)$ $\exists y, \exists x, P(x,y)$ | There is a pair $(x,y)$ for which $P(x,y)$ is true.        | $P(x,y)$ is false for every pair $(x,y)$.                   |
## Notes
- Everything within the scope of a quantifier can be thought of as a propositional function. 
- Negate the statement with nested quantifiers by successively applying [[De Morgan]]'s Law. For example, $\neg(\forall x,\exists x,P(x,y))\equiv \neg \forall x,\exists y,P(x,y) \equiv \exists x,\neg \exists y,P(x,y) \equiv \exists x,\forall y,P(x,y)$ 

# Methods of Proof
**Proving a conditional statement $p \implies q$**.

1. **Trivial Proofs**: By showing that $q$ is true, it follows that $p \implies q$ must be true. That is, if $q$ is true then it doesn't matter if $p$ is true or not, $p \implies q$ is true.
2. **Vacuous Proof** *(Proof by Default)*: By proving that $p$ is false, it follows that $p \implies q$ must be true. That is, if $p$ is false, it doesn't matter if $q$ is true or not, $p \implies q$ is true because there is no situation where it may be proven true or false.  
3. **Direct Proof**: By proving that $p$ leads to $q$ through logical and [[Axiomatic]] steps, it follows that $p \implies q$. 
	1. Identify and list all hypotheses and the results related to the hypotheses.
	2. Develop a complete set of logical arguments from the hypotheses to the conclusion.
	3. Rewrite into a clear and concise proof with each step of the step clearly justified.
	4. Proofread the proof.
4. **Proof by Contraposition (*[[Contrapositive]]*)**: 
	1. State the **contrapositive** $\neg q \implies \neg p$. Now, $\neg q$ is the hypothesis and $\neg p$ is the conclusion. 
	2. Identify and list all hypotheses and results related to the hypothesis. 
	3. Develop a complete set of logical arguments from the hypothesis to the conclusion. 
	4. Rewrite into a clear and concise proof with each step of the proof clearly justified.
	5. Proofread the proof.
5. **Proof by Contradiction (*reductio ad impossible* or *reductio ad absurdum*)** 
	1. Assume the **negation** of $p \implies q$ which is $p \wedge \neg q$. Start with *"Suppose not. That is..."*
	2. Identify and list all results related to $p$ and $\neg q$.
	3. Develop a logical sequence of arguments that leads to a contradiction.
	4. Rewrite into a clear and concise proof with each step of the proof clearly justified.
	5. Proofread the proof. 

## Disproof
- To disprove $p$ is to prove $\neg p$. 
## Note on Ending Proofs
- It is common to write "Proof." or "Pf." to indicate the beginning of a proof, and a black square (⬛) or "$Q.E.D.$" to indicate the end. 
- Q.E.D. stands for "*quod erat demonstratum*" which means "what which was to be demonstrated" or "what was to be shown".

## Aside. Some notes on mathematical writing
- Never start a sentence with a symbol
- Explain the *meaning* of every symbol/variable you introduce
- Use consistent symbols. Use **"frozen symbols"** such as:
	- $m,n$ for $\mathbb{Z}$
	- $x,y$ for $\mathbb{R}$ 
	- $A,B$ for sets
- Use "We" or no pronouns
- Avoid "clearly" "obviously" "of course" or "certainly"
- The word "any" can be vague. Use **"for each" "for every" or "for all"** 
- Write **"Since..., it follows that..."** and not "Since..., then..."
- Introduce some *variety*: **"Therefore" "thus" "hence" "consequently" "so" or "this implies that"**