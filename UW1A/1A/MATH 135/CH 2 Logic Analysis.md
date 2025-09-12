
### Truth Tables and Negation
$A$ is a statement with assigned truth value and can be manipulated as treated as logical expression using logical operators(e.g. $\neg, \vee, \wedge, \implies$). 

$$
\begin{array}{|c|c|c|}
\hline 
A & \neg A & \neg(\neg A) \\
\hline
T & F & T \\
\hline
F & T & F \\
\hline 
\end{array}
$$
### Compound Statement 
is a statement composed of several individual statement, each of which is called component statement
	$\vee$ is "or", is disjunction
	$\wedge$ means "and", is a conjunction
	$$\begin{array}{|c|c|c|}
\hline 
A & B & A \vee B & A \wedge B \\
\hline
T & T & T & T  \\
\hline
T & F & T & F  \\
\hline 
F & T & T & F  \\
\hline
F & F & F & F  \\
\hline
\end{array}
$$ 

### Logical Laws

1) De Morgan's Law (DML)
	For statement variables $A \text{ and } B$
	1) $\neg(A \wedge B) \equiv \neg (A) \vee \neg (B)$
	2) $\neg(A \vee B) \equiv \neg (A) \wedge \neg (B)$

2) Commutative, Associative, and Distributive Laws
     ![[Screenshot 2025-09-08 at 11.02.30 AM.png]]


Examples:
1) Show using a truth table that $\neg (A \wedge B) \equiv \neg(A) \vee \neg(B)$(the proof of DML)
$$\begin{array}{|c|c|c|c|c|c|c|}
\hline A & B & \neg A & \neg B & A \wedge B & \neg(A \wedge B) & \neg(A) \vee \neg (B)\\
\hline T & T & F & F & T & F & F \\
\hline T & F & F & T & F & T & T \\
\hline F & T & T & F & F & T & T \\
\hline F & F & T & T & F & T & T \\
\hline
\end{array}$$
	since the columns for $\neg(A \wedge B)$ and $\neg(A) \vee \neg(B)$ are identical in the truth table, we may conclude that they are logically equivalent, 
	i.e. $\neg (A \wedge B) \equiv \neg(A) \vee \neg(B)$
	Similarly, $\neg (A \vee B) \equiv \neg(A) \wedge \neg(B)$ can also be proven through truth table
2) Prove that 
	$A \wedge (B \vee C) \equiv (A\wedge B)\vee(A \wedge C)$
	$$\begin{array}{|c|c|c|c|c|c|c|c|}
\hline A & B & C & B \vee C & A \wedge(B \vee C) & A \wedge B & A \wedge C & (A \wedge B) \vee (A \wedge C) \\
\hline T & T & T & T & T & T & T & T \\
\hline T & T & F & T & T & T & F & T \\
\hline T & F & T & T & T & F & T & T \\
\hline T & F & F & F & F & F & F & F \\
\hline F & T & T & T & F & F & F & F \\
\hline F & T & F & F & F & F & F & F \\
\hline F & F & T & T & F & F & F & F \\
\hline F & F & F & F & F & F & F & F \\
\hline
\end{array}$$

### Implications
$\implies$ is an implication meaning:
	B if A
	B when A
	B whenever A
	A is a sufficient condition of B

*Commutative, Associative, and Distributive properties still apply on implications*

$(A \implies B) \equiv (\neg A \vee B)$
$$\begin{array}{|c|c|c|c|c|}
\hline A & B & A \implies B & \neg A & (\neg A\vee B) \\
\hline T & T & T & F & T\\
\hline T & F & F & F & F\\
\hline F & T & T & T & T\\
\hline F & F & T & T & T\\
\hline
\end{array}$$
so $\neg A \implies B \equiv \neg(\neg A \vee B) \equiv A \wedge \neg(B)$

Practice:
	$((A \vee B)\implies C) \equiv (A \implies C)\wedge (B\implies C)$
$$\begin{array}{|c|c|c|c|c|c|c|}
\hline A & B & C & A \vee B & (A \vee B)\implies C & A \implies C & B \implies C & (A \implies C) \wedge (B \implies C)B\\
\hline T & T & T & T & T & T & T & T \\
\hline T & T & F & T & F & F & T & F \\
\hline T & F & T & T & T & T & T & T \\
\hline T & F & F & T & F & F & F & F \\
\hline F & T & T & T & T & T & T & T \\
\hline F & T & F & T & F & T & F & F \\
\hline F & F & T & F & T & T & T & T \\
\hline F & F & F & F & T & T & T & T \\
\hline
\end{array}
$$

### Converse
$B \implies A$ is called the **converse** of $A \implies B$

### Contrapositive
$(\neg B) \implies \neg(A)$ is called the **contrapositive** of $A \implies B$

$$\begin{array}{|c|c|c|c|c|c|}
\hline A & B & A \implies B & B \implies A & \neg A & \neg B & (\neg B) \implies (\neg A) \\
\hline T & T & T & T & F & F & T \\
\hline T & F & F & T & F & T & F \\
\hline F & T & T & F & T & F & T \\
\hline F & F & T & T & T & T & T \\
\hline
\end{array}$$
Examples:
1) If $x>y$, then $x\geq y$
2) Converse: If $x\geq y$, then $x>y$
3) Contrapositive: If $x < y$, then $x\leq y$


### If and Only If
$\iff$ means "if and only if"

$$\begin{array}{|c|c|c|c|c|c|}
\hline A & B & A \implies B & B \implies A & A \iff B & (A \implies B) \wedge (B \implies A) \\
\hline T & T & T & T & T & T \\
\hline T & F & F & T & F & F \\
\hline F & T & T & F & F & F \\
\hline F & F & T & T & T & T \\
\hline
\end{array}
$$
What is $\neg(A \iff B)$ ?
$\equiv \neg ((A \implies B) \wedge (B \implies A))$
$\equiv \neg(A \implies B) \vee \neg(B \implies A)$ 
$\equiv \neg(\neg(A) \vee B) \wedge \neg(A \vee \neg(B))$
$\equiv (A\wedge \neg(B)) \wedge (\neg(A) \wedge B))$
$\equiv \neg A \implies B \wedge \neg B \implies A$

  

Q1) 
a)
Knowing that  $[(\neg H)\iff((\neg E)\wedge G)] \wedge [E \wedge \neg(H\wedge G)] \equiv True$
Construction of truth table
$$\tiny\begin{array}{|c|c|c|} 
\hline H & E & G & \neg H & \neg E & \neg E \wedge G & \neg H \iff ((\neg E)\wedge G) & H\wedge G & \neg (H \wedge G) & E \wedge \neg(H \wedge G) & [(\neg H)\iff((\neg E)\wedge G)] \wedge [E \wedge \neg(H\wedge G)] \\
\hline T & T & T & F & F & F & T & T & F & F & F \\
\hline T & T & F & F & F & F & T & F & T & T & T \\
\hline T & F & T & F & T & T & F & T & F & F & F \\
\hline T & F & F & F & T & F & T & F & T & F & F \\
\hline F & T & T & T & F & F & F & F & T & T & F \\
\hline F & T & F & T & F & F & F & F & T & T & F \\
\hline F & F & T & T & T & T & T & F & T & F & F \\
\hline F & F & F & T & T & F & F & F & T & F & F  \\
\hline
\end{array}
$$
b)
$[((\neg S)\vee K)\implies(W \wedge S)] \equiv [(W \vee(\neg K))\wedge S]$

$$
\begin{array}{|c|c|c|}
\hline S & K & W & \neg S & \neg K & \neg S \vee K & W \wedge S & (\neg S\vee K) \implies (W \wedge S) & W \vee (\neg K) & (W \vee \neg K) \wedge S \\
\hline T & T & T & F & F & F & T & T & T & T \\
\hline T & T & F & F & F & T & F & F & F & F  \\
\hline T & F & T & F & T & F & T & T & T & T \\
\hline T & F & F & F & T & F & F & T & T & T \\
\hline F & T & T & T & F & T & F & F & T & F  \\
\hline F & T & F & T & F & T & F & F & F & F  \\
\hline F & F & T & T & T & T & F & F & T & F \\
\hline F & F & F & T & T & T & F & F & T & F \\
\hline
\end{array}

$$
Since each element of the column of $(\neg S \vee K) \implies (W \wedge S)$ holds the exact same truth value as the column $[(W\vee(\neg K)) \wedge S]$. We conclude that these two logical expressions are logically equivalent, that is $[((\neg S)\vee K)\implies(W \wedge S)] \equiv [(W \vee(\neg K))\wedge S]$

Q2)
a) $a+b\leq 5$
b) $(a\leq 2) \vee (b\leq 3)$
c) The logical expression $J(a, b)$ says that $a+b\leq 5 \implies (a\leq 2) \vee (b \leq 3)$
The converse will then be $K(a, b)$, which is $(a\leq 2) \vee (b \leq 3) \implies a+b\leq 5$
$\forall a, b \in R, K(a, b)$ is False
d)The contrapositive of $J(a, b)$ is $L(a, b) \equiv (a > 2) \wedge (b> 3) \implies a+b>5$
$\forall a, b \in R, L(a, b)$ is True
e)$\exists a, b \in R, (a+b\leq 5) \wedge [(a>2)\wedge(b>3)]$ 
$\neg J(a, b)\equiv$ True
f)False

Q3)
a) 
True
Let $x$ be the smallest of arbitrary four consecutive integers, those consecutive integers can be expressed as $x, x+1, x+2, x+3$. 
We compute their average: $\frac{x + (x+1)+(x+2)+(x+3)}{4} = \frac{4x+6}{4}$
Factor $\frac{4x+6}{4}  = \frac{4\left( x+\frac{3}{2} \right)}{4} = x+ \frac{3}{2}$
Since $x$ is an integer and $\frac{3}{2}$ is a rational number, their sum remains a rational number.
Thus the average of four consecutive integer is always a non-integer.
b)
False
Let $x$ be the smallest of arbitrary five consecutive integers, those consecutive integers can be expressed as $x, x+1, x+2, x+3, x+4$
We compute their average: $\frac{x+(x+1)+(x+2)+(x+3)+(x+4)}{5} = \frac{5x+10}{5} = x+2$
Since $x$ is an integer and 2 is also an integer, $x+2$ is always an integer. That is, the average of any five consecutive integers is always an integer.

Q4) 
$\forall x \in \mathbb{R}, 3|x+8|-5|2x-4|\leq 30$
$3|x+8|-5|2x-4|\leq 30 \iff 3|x+8|-10|x-2|\leq 30 \iff 3|x+8|-10|x-2|-30\leq 0$
Let's perform case analysis:

Case 1($x<-8$):
The function becomes  $-3x-24+10x-20-30 \leq 0 \iff 7x-74 \leq 0 \iff 7x \leq 74 \iff x \leq \frac{74}{7}$ 

Case 2($-8\leq x\leq 2$):
The function becomes
$3x+24+10x-20-30\leq 0 \iff 13x-26 \leq 0 \iff x \leq 2$

Case 3($x>2$):
$3x+24-10x+20-30 \leq 0 \iff -7x-14 \leq 0 \iff x \geq 2$

Now, we have $3|x+8|-5|2x-4|\leq 30 \iff x \in (-\frac{\infty,74}{4}] \cup (-\infty, 2] \cup [2, \infty)$ 
Since the set $(-\frac{\infty,74}{4}] \cup (-\infty, 2] \cup [2, \infty)$ is $\mathbb{R}$, 
Thus we have shown that $\forall x \in \mathbb{R}, 3|x+8|-5|2x-4|\leq 30$

Q5)
$\forall a, b, c \in \mathbb{R}, a^2+14b^2+4c^2-6ab-7bc\geq b(4b-3c)$
Let $a, b, c$ be arbitrary numbers
Since $a, b, c$ are all real numbers, $(a-3b)$ and $(b-2c)$ are all real numbers.
$(a-3b)^2$ and $(b-2c)^2$ are also real numbers, $(a-3b)^2+(b-2c)^2\geq 0$
$(a-3b)^2+(b-2c)^2\geq 0 \iff a^2+9b^2+b^2+4c^2-6ab-4bc\geq 0 \iff a^2+10b^2+4c^2-6ab-4bc \geq 0 \iff a^2+14b^2+4c^2 - 6ab - 7 bc -4b^2+3bc \geq 0 \iff a^2+14b^2+4c^2-6ab-7bc-b(4b-3c) \geq 0 \iff a^2+14b^2+4c^2-6ab-7bc\geq b(4b-3c)$ 
Thus we have proved that $\forall a, b, c \in \mathbb{R}, a^2+14b^2+4c^2-6ab-7bc\geq b(4b-3c)$ 

Q6)
a) $\forall \theta \in \mathbb{R}, [P(\theta) \wedge Q(\theta) \wedge T(\theta) \iff U(\theta)]$
b)$\neg[\forall \theta \in \mathbb{R}, S(\theta)\iff V(\theta)]$
c)
d)

