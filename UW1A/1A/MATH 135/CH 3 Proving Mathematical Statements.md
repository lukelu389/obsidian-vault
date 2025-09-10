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
### To Disprove Universally Quantified Statement
1) Find an element $x \in S$ for which the open sentence is false. 
Example:
	Proof that $\forall x \in \mathbb{R}, x^2=5$
	Proof:
		Let $x=0$
		Thus $x^2 = 0$, which is not 5.
		Therefore $\exists x \in \mathbb{R}, x^2 \neq 5$, namely $x=0$.
		So it is false $\forall x \in \mathbb{R}, x^2=5$