
**Set Notation**
$\mathbb{N}$ is the set of natural number, 0 is excluded. 
$\mathbb{Z}$ is the set of integers.    
$\mathbb{Q}$ is the set of all numbers of form $\frac{a}{b}$ where $a \in \mathbb{Z}$ and $b \in \mathbb(Z) \setminus \{0\}$.   
$\mathbb{R}$ is the set of all real numbers.    

Parity: if an integer is even or odd.  

**Statements**  
A statement is a sentence that has a definite state of being either true of false.  
	Examples not statement:   
		questions 
		order  
		no definite true of false answers  
			This statement is false  
			Let $x$ be ...    
			$x > 3$   
			$x = x$   
**Negation**   
Suppose that $A$ is a statement. Then the **negation** of $A$, is denoted by $\neg A$, is the statement asserting the opposite truth value to . That is, $\neg A$ is false when $A$ is true, and $\neg A$ is true when $A$ is false.   

Logically equivalent : $\neg (\neg A) \equiv A$   

**Quantifiers**  
- Universal  
	- $\forall$ means "for all" is the universal quantifier.  
- Existential  
	- $\exists$ means "there exist(s)" is the existential quantifier.  

Example:
	$\exists x \in \mathbb{R}, x>3$ means "There exists a real number $x$ s.t. $x > 3$" ), an existentially quantified statement. 

Terminology:  
	Variable (e.g. $x$) 
	A domain is any set (e.g. $\mathbb{R}$, etc.)  
	An open sentence denoted, $P(x)$, involving the variable that is either true of false whenever a value of variable chosen from the domain is specified (e.g. $x>3$ from the previous lines).  

FYI 
![[Screenshot 2025-09-05 at 11.02.48 AM.png]]
Examples:  
Consider the phrase "$x+1 > x$ "; this is not a statement, as we cannot tell if it is true of false until we know what $x$ is.(e.g. a real number? a horse?). 
However, the phrase. "$\forall x \in \mathbb{R}, x+1>x$" is a statement; it is true.  

**Nested Quantifier**  
Consider the universally quantified statement on $x$:"$\forall x \in \mathbb{R}, \exists y \in \mathbb{R}, x>y$ ", which is true. It says every real number $x$ has a smaller number $y$ s.t. $x>y$.   

Caution that "$\exists y \in \mathbb{R}, \forall x \in \mathbb{R}, x>y$" is a completely a new universally quantified statement on $y$, which is false. It says $y$ is the smallest than any real number, even smaller than itself!   

**Two Nested Quantifiers**  
If we have the same domain and same quantifier for both variables, we can abbreviate the notation:
$$\forall x,y\in \mathbb{R}, P(x, y)$$
$$\exists x,y \in \mathbb{R},P(x, y)$$
Negation:   
![[Screenshot 2025-09-05 at 11.18.59 AM.png]]

Assignment 1 
Q1
a)S
b)N
c)N
d)S

Q2
a)F
b)T
c)T
d)F

Q3 
a) Solution:
	We know that $\neg(\forall x\in X, P(x)) \equiv \exists x \in X \neg(P(x))$,
	we have $\neg(\forall a \in \mathbb{Z}, (a-5)^2\geq_{0}) \equiv \exists a \in \mathbb{Z}, (a-5)^2 < 0$$
	Thus, the answer is: $\exists a \in \mathbb{Z}, (a-5)^2 < 0$
b)Solution:
	Similarly, $\neg(\exists x \in X, \forall y \in Y, Q(x, y)) \equiv \forall x \in X, \exists y \in Y, \neg(Q(x, y))$
	we have $\neg(\exists \theta\in \mathbb{R}, \forall \alpha \in \mathbb{R}, \sin(\theta)=\cos(\alpha)) \equiv \forall \mathbb{\theta} \in \mathbb{R}, \exists \mathbb{\alpha} \in \mathbb{R}, \sin(\mathbb{\theta}) \neq \cos\mathbb(\alpha)$
	Thus, the answer is: 
	$\forall \mathbb{\theta} \in \mathbb{R}, \exists \mathbb{\alpha} \in \mathbb{R}, \sin(\mathbb{\theta}) \neq \cos\mathbb(\alpha)$ 

Q4
a) $f(x) = \sin(x); f(x) \in [-1,1]$
b) $\forall r \in \mathbb{R}, \exists a, b \in \mathbb{R}$ s.t. $r = a*b$

Q5
a)Statement is False
b)Statement is True
c)Statement is True
d)Open sentence depending on $w$
e)Statement is True

Q6) 
a)$\forall x, y \in S, P(x, y)$ with domain $\mathbb{Q}_{>0}$, $P_{4}=xy \in S$
b)$\forall x \in S, \exists y \in S, P(x, y)$ with domain $\mathcal{T}=\{-1, 0, 1\}$, $P_{3}: \sin\left( \frac{\pi y}{2} \right) = |x|$
c)$\exists x \in S, \forall y \in S, P(x, y)$ with domain $\mathbb{R}$,  $P_{2}=y^2\geq x$ 
d)$\exists x, y \in S$ with domain $\mathcal{U}=\{3, \frac{1}{3}\}$, $P_{1}(x, y):x=27^y$

7)
a) True

b) Seeking help is a tip that resonates with me. Whenever encountering a problem, I will always try to solve it alone, which typically goes awfully wrong. When I was in CEGEP, I frequently seek help for tough questions. Professors and classmates are very open towards the discussion and give inspiration tips to help me find the solution. This reminds me that there is a whole community that is surrounding me with resources and kindness, and it is never too late to reach out to others than fighting alone. 


