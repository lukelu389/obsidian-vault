
**Truth Tables and Negation**
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
**Compound Statement** is a statement composed of several individual statement, each of which is called component statement
	$\vee$ is "or", is disjunction
	$\wedge$ means "and", is a conjunction
	$\implies$ means "implies", is an implication
	$$\begin{array}{|c|c|c|}
\hline 
A & B & A \vee B & A \wedge B & A \implies B \\
\hline
T & T & T & T & ?  \\
\hline
T & F & T & F & ? \\
\hline 
F & T & T & F & ? \\
\hline
F & F & F & F & ?  \\
\hline
\end{array}
$$

**Logical Laws**

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

**Implications**
$\implies$ is an implication meaning:
	B if A
	B when A
	B whenever A
	A is a sufficient condition of B

Commutative, Associative, and Distributive properties still apply on implications

$A \implies B \equiv \neg(A) \vee B$

$$\begin{array}{|c|c|c|}
\hline A & B & A \implies B \\
\hline T & T & T \\
\hline T & F & F \\
\hline F & T & T  \\
\hline F & F & T \\
\hline
\end{array}$$

