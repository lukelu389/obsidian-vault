### Definitions
1) **Proposition** is a true statement has to be proved to be true
2) **Theorem** is a significant proposition
3) **Lemma** is a subsidiary proposition
4) **Corollary** is a proposition that follows almost immediately from a theorem

### Proving Universally Quantified Statements
1) Choose a representative mathematical object $x \in S$ (e.g. Let the object be an arbitrary in S)
2) Show the open sentence must be true for representative $x$, using known facts about the elements of $S$
Example:
	Proof that $\forall x, y \in \mathbb{R}$, $x^4+x^2y+y^2\geq 5x^2y-3y^2$ 
	Discovery:
		if $x^4+x^2y+y^2\geq 5x^2y-3y^2 \implies x^4+x^2y+y^2 - 5x^2y + 3y^2 \geq 0$ 
		then $(x^2-y)^2 \geq 0$ 
		However this is not a proof, it assumes the statement to be true already
	**Actual Proof:**
		Let $x \text{ and } y$ be arbitrary real numbers.
		Since $x, y \in \mathbb{R}$, then $(x^2-2y)$ is a real number.
		Which means that $(x^2-2y)^2 \geq 0$, as all real numbers squared will be non-negative.
		Thus, $x^4-4x^2y+4y^2 \geq 0$.
		Then, $x^4 + x^2y - 5x^2y + y^2 + 3y^2 \geq 0$.
		So, $x^4+x^2y+y^2\geq 5x^2y-3y^2$ .
		Therefore, we have proved that $\forall x, y \in \mathbb{R}$, $x^4+x^2y+y^2\geq 5x^2y-3y^2$
#### Disprove Universally Quantified Statement
Find an element $x \in S$ for which the open sentence is false; that is proving an existentially quantified statement.
Example:
	Proof that $\forall x \in \mathbb{R}, x^2=5$
	Proof:
		Let $x=0$
		Thus $x^2 = 0$, which is not 5.
		Therefore $\exists x \in \mathbb{R}, x^2 \neq 5$, namely $x=0$.
		So it is false $\forall x \in \mathbb{R}, x^2=5$

### Prove Existentially Quantified Statement
Find an element $x \in S$ for which the open sentence is true.

Example 1:
	Prove that $\exists \in \mathbb{Z}$ s.t. $\frac{m-7}{2m+4}=5$
	Discovery:
	$m-7 = 5(2m+4) \iff m-7 = 10m+10 \iff -27 = 9m \iff m=-3$
	**Actual Proof**:
		Let $m = -3$, clearly $-3 \in \mathbb{Z}$
		and $\frac{m-7}{2m+4} = \frac{-3-7}{2(-3)+4} = \frac{-10}{-6+4}=\frac{-10}{-2} = 5$
		Therefore, we have shown that $m \in \mathbb{Z}, \frac{m-7}{2m+4}=5$
Example 2:
	Prove that there exists a perfect square $k$ s.t. $k^2-\frac{31}{2}k = 8$
	Proof:
	Let $k = 16$, clearly, $k=16 = 4^2$
	Also, $k^2-\frac{31}{2}k = 16^2-\frac{31}{2}(16) = 16 \left(  16-\frac{31}{2} \right) = \frac{16}{2}*1 = 8$
	Therefore, we have shown that there exists a perfect square $k$ s.t. $k^2-\frac{31}{2}k = 8$

#### Disprove Existentially Quantified Statement
Example:
Disprove that $\exists x \in \mathbb{R}, \cos(2x)+\sin(2x)=3$
we need to prove $\forall x \in \mathbb{R}, \cos(2x)+\sin(2x)\neq 3$
Let $x \in \mathbb{R}$
Notice that $-1 \leq \cos 2x \leq 1$ and $-1 \leq \sin 2x \leq 1$
So we can add the inequalities to get: $-2 \leq \cos 2x +\sin 2x \leq 2$
Clearly, $\cos(2x)+\sin(2x) \neq 3$, since $3 \notin [-2,2]$
$\therefore \forall x \in \mathbb{R}, \cos(2x)+\sin(2x) \neq 3$ 
i.e. $\neg(\exists x \in \mathbb{R}, \cos(2x)+\sin(2x)=3)$  



### Prove/Disprove Nested Quantified Statement
Example:
Consider the two statements:
1) $\forall x \in \mathbb{R}, \exists y \in \mathbb{R}, x^3-y^3=1$
2) $\exists x \in \mathbb{R}, \forall y \in \mathbb{R}, x^3-y^3=1$

Prove or Disprove:
1) This is true
	Let $x \in \mathbb{R}$, let $y= (x^3-1)^\frac{1}{3}$
	$x^3-y^3 = x^3-((x^3-1)^\frac{1}{3})^3$
	$= x^3 - (x^3-1)$
	$= x^3-x^3+1$
	$= 1$
	$\therefore \forall x \in \mathbb{R}, \exists y \in \mathbb{R}, x^3-y^3=1$
2) This is false
	We will prove the negation, that is $\forall x \in \mathbb{R}, \exists y \in \mathbb{R}, x^3-y^3 = 1$
	Let $x \in \mathbb{R}$, let $y=x$
	Then $x^3-y^3 = x^3-x^3=0 \neq 1$ 
	We have shown that $\forall x \in \mathbb{R}, \exists y \in \mathbb{R}, x^3-y^3 = 1$  
	$\therefore \exists x \in \mathbb{R}, \forall y \in \mathbb{R}, x^3-y^3=1$