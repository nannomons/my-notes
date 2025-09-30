# Answer 2c
[[Pasted image 20250923024226.png]]
![[stt200a activity 2 - 2c]]
## 2a
$\neg(r \wedge \neg s) \implies p$ 

$r \wedge \neg s$ ; Dogs can fly (**FALSE**) AND there exists an even prime number (**TRUE**). = ***FALSE***
$r \wedge \neg s = false \wedge true = false$

$\neg(r \wedge \neg s) = \neg r \vee s$ ; Dogs cannot fly (**TRUE**) OR there does no even prime number (**FALSE**). = ***TRUE** simply because the negation of the previous statement (which is FALSE) is true*.
$\neg(r \wedge \neg s) = \neg r \vee s = true \vee false = true$ 

$\neg(r \wedge s) \implies p$ ; 0 = 1 (**FALSE**) if dogs cannot fly (**TRUE**) OR there does no even prime number (**FALSE**). 
$\neg(r \wedge s) \implies p = true \vee false \implies false$
$\neg(r \wedge s) \implies p = true \implies  false$ 
$\neg(r \wedge s) \implies p = false$


## 2c
### Given
p is $0=1$
s is There is no even prime number
r is Dogs can fly
t is all composite numbers are divisible by 2

Determine whether the statement is true or false: $\neg[p \implies (s \implies (r \implies t))]$.

### Solution
$r \implies t = false \implies false = true$
$s \implies (r\implies t) = s \implies true = false \implies true = true$
$p \implies (s \implies (r \implies t)) = p \implies true = false \implies true = true$
$\neg[p \implies (s \implies (r \implies t))] = \neg true = false$

# Answer 5c 
[[Pasted image 20250923024331.png]]
![[stt200a activity 2 - 5c]] 

### Yuh
Prove the ff. statements using the [[Contrapositive]]

5c.) An integer is odd if its square is not divisible by 4. 

q if p 
q is an integer is odd
p is its square is not divisible by 4

if p, q
If an integer's square is not divisible by 4, it is odd.

$\neg q \implies \neg p$ 
If an integer is not odd (i.e., even), then its square is divisible by 4.

Let $n \in \mathbb{Z}_{E}$. By definition, $n = 2k$ for some $k \in \mathbb{Z}$. Also, an integer $a$ is said to divide an integer $b$, denoted by $a|b$, if and only if $b=al$ for some integer $l$. 

$n = 2k$ 
$n^2 = (2k)^2$ 
$n^2=(2k)(2k)$ 
$n^2=2(2k)k$ ; [[Associativity]] for Multiplication
$n^2=(2)(2)(k)(k)$ ; [[Commutativity]] for Multiplication
$n^2=4(k^2)$ 

Since $k^2 \in \mathbb{Z}$ by closure, we can write $n^2=4l$ where $l=k^2 \in \mathbb{Z}$. 

By definition of divisibility, this means $4|n^2$. 

### Conclusion
We have shown that if $n$ is even, then $n^2$ is divisible by 4.

By contrapositive logic, this implies that if $n^2$ is not divisible by 4, then $n$ is odd.