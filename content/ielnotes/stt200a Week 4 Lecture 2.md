---
title: Universal Set and Subsets
publish: true
tags:
Subject:
  - Mathematical Reasoning
Course:
  - STT200A
YearTerm: Y1T1
Type: Lecture Notes
Difficulty:
Date: 2025-09-26
---
# Defn. Set 
- A **set** is a well-defined collection of objects.
- These objects are called **elements** or **members** of the set.
- The collection of all objects of interest is called the **universal set** or **universe**.

## Note.
- **Notations:** Uppercase letters for *sets*, e.g. $A,B,C$ ; $u$ or $\Omega$ for *universals*.
- $x \in A$ is read as **"$x$ in $A$"** or **"$x$ is an element of $A$"**
- $A = 3k | \mathbb{Z}$ is read as **"$A$ is the set of numbers of form $3k$ such that $k$ is an integer."**

## Examples
- **Finite set**: $\{ 1,2,3 \}$, $\{ 2,4,6,8,\dots,1000\}$
- **Countably Infinite set**: $\mathbb{Z}$, $\mathbb{Q}$, $2,4,6,8,\dots$
- **Uncountable set**: $(0,1)$, $(-\infty,1]$, $[100,\infty)$

| Roster Method/Listing Method                              | Set-Builder Notation/Rule Method                                                    |
| --------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| $\mathbb{Z}_{E} = \{\dots,-2,0,2,4,\dots\}$               | $\mathbb{Z}_{0} = \{ n:n=2k$ for some $k \in \mathbb{Z}\}$                          |
| $\mathbb{Z}^-=\{\dots,-4,-3,-2,-1\}$                      | $[1,\infty)=/{x \in \mathbb{R}:x \geq \frac{1}{}}$                                  |
| Set of primes less than 3 = $\{ 2 \}$                     | $\mathbb{Q}^+ = \{ x \in \mathbb{R} : x = \frac{p}{q}$ where $p,q \in \mathbb{Z}\}$ |
| $\mathbb{N}=\{1,2,3,4,5,\dots\}$                          | $\mathbb{C} = \{a+bi:a,b \in \mathbb{R} \wedge i=\sqrt{ -1 }\}$                     |
| Set of multiples of 5 = $\{ \dots,-10,-5,0,5,10,\dots \}$ | Set of multiples of 3 = $\{ n:3\|n$ for some $n\in z$                               |

# Defn. Cardinality
- The **cardinality** or **size** of a finite set is the number of elements it has.
- **Notations**: $|A|$ or $n(A)$

# Defn. Empty and Singleton Sets
- The **empty set** is the set that has *no elements*. Written as $\emptyset$.
- A **singleton set** is the set that has *only one element*. 

## Note
- $\emptyset$ is a *finite set* with $|\emptyset|=0$
- $\emptyset$ is not the same as $\{ \emptyset \}$. $|\{ \emptyset=1 \}|$. 

# Defn. Subset
Let $A$ and $B$ be sets.
- $A$ is a **subset** of $B$ if every element of $A$ also belongs to $B$. $A \subseteq B \iff \forall x, (x \in A \implies x \in B)$ or $B \supseteq A$.
- $A$ is a **proper subset** of $B$ if every element of $A$ also belongs to $B$. $A \subset B \iff \forall x, (x \in A \implies x \in B)\wedge \exists x, (x \in B \wedge n \notin A$) 
- $A$ and $B$ are **equal** if they contain exactly the same elements. 
	- $A = B \iff A \subseteq B \wedge B \subseteq A$ 
	- $A = B \iff \forall x, (x \in A \ x \in B) \wedge \forall x, (x \in B = x \in A)$
	- $A = B \iff \forall x, (x \in A \iff x \in B)$

## Examples
- $\mathbb{Q} \subseteq \mathbb{R}$
- $\{ 1,2\} \subseteq (0,1)$
- $\mathbb{Z}_{E} \subset \mathbb{Z}$
- $\mathbb{Z} \subset \mathbb{R}$
- $\mathbb{Z}^+ =\mathbb{N}$
- $\mathbb{Z}_{E}=\{x \in \mathbb{Z}:2|x\}$
- $\{ 1 \} \not\subseteq [10,\infty)$
- $\mathbb{Q} \subset \mathbb{Q}^C$
- $\{ a \} \not\subset \{ a \}$
- $\{ x,y,z \} \not\subset \{ x,y,z \}$

# Thm. 
1. $\emptyset \subseteq A$ for any set $A$.
2. $A \subseteq A$ for any set $A$.
3. If $A \subseteq B$  and $B \subseteq C$ then $A \subseteq C$ for any sets $A,B,C$.

# Cor. 
There is only one set with no elements ($\emptyset$).