### Triangle Inequality

$$|x-y|\leq|x-z|+|z-y|$$
![[Screenshot 2025-09-10 at 11.29.49 AM.png]]
	It suggests the straight distance between two points is a direct line
	Without loss of generality, suppose $x \leq y$
			swap $x$ and $y$, $|x-y|\leq|x-z|+|z-y| \iff |y-x|\leq|x-z|+|y-z| \iff  |x-y|\leq |x-z|+|z-y|$   
	Proof: (number line)
		Case 1($z\leq x\leq y$):
			$|x-y|\leq|z-y\leq|x-z|+|z-y|$ 
		Case 2($x\leq z\leq y$):
			$|x-y|=|x-z|+|z-y|$ so $|x-y|\leq|x-z|+|z-y|$
		Case 3($x\leq y\leq z$):
			$|x-y|\leq|x-z|+|z-y|$
### Triangle Inequality 2
$\forall a, b \in \mathbb{R}, |a+b|\leq|a|+|b|$
Proof:
	By Triangle Inequality, $|x-y|\leq|x-z|+|z-y|, \forall x, y, z \in \mathbb{R}$
	in particular, $x= a, y = -b, z =0$
	becomes $|a+b|\leq|a-0|+|0-(-b)| = |a|+|b|$
	
Is it true that $|a - b|\leq|a|-|b|, \forall a, b \in \mathbb{R}$ ?
	No, let $a = 10, b = -9 \implies |10-(-9)|\nleq|10|-|-9|$ 

Examples of inequalities:
1) $|x-a|<\delta$ implies $x \in (a-\delta, a+\delta)$
2) $|x-a|\leq \delta$ implies $x \in [a-\delta, a+\delta]$
3) $0<|x-a|\leq\delta$ implies $x \in (a-\delta, a) \cup (a, a+\delta)$

### Practice questions:
1) Solve $|-2x+6|<5 \implies 2|x-3|<5 \implies |x-3|< 5/2$ 
	Solution interval is $(3-\frac{5}{2}, 3+\frac{5}{2})$
2) Solve $2<|x+7|\leq {3} \implies 2<|x-(-7)\leq_{3}$
	 Solution interval is $[-10, -9)\cup(-5, -4]$
3) Solve $\frac{|x+2|}{|x-2|}>5$
	$$|x+2| = \begin{cases}
x+2, & \text{if } x \geq -2\\
-x+2, & \text{if } x < -2
\end{cases}$$$$|x-2| = \begin{cases}
x-2, & \text{if } x\geq2\\
-x-2, & \text{if } x<2
\end{cases}$$
	Case 1($x<-2$):
	$\frac{-x-2}{2-x} > 5 \iff -x-2>10-5x \iff x > 3 \iff$ impossible
	Case 2($-2\leq x<2$):
	$\frac{x+2}{2-x} > 5\iff x+2>10-5x \iff \frac{x>4}{3} \implies x\in (\frac{4}{3}, 2)$ 
	Case 3($x>2$):
	$\frac{x+2}{x-2}> 5 \iff x+2>5x-10\iff 3>x \implies x\in (2, 3)$
	Solution:  
	$x \in (\frac{4}{3}, 2) \cup (2, 3)$


### Infinite Sequence
An infinite sequence is a list of numbers in a definite order
$$a_{1}, a_{2}, a_{3}, a_{4}, \dots, a_{n}, \dots$$
where $a_{i} \in \mathbb{R} for i \in \mathbb{N}$. We use notation $\{a_{n}\}^{\infty}_{n=0}$

Let $\{a_{n}\}$ be a sequence of real numbers and $n_1< n_2< \dots$ be increasing sequence of natural numbers$$a_{n_{1}}, a_{n_{2}}, a_{n_{3}}\dots$$ denoted $\{a_{n_{k}}\}$ is called a subsequence of $\{a_{n}\}$.

The subsequence $a_{k}, a_{k+1}, a_{k+2},\dots$ of $\{a_{n}\}$  is called the **tail** of $\{a_{n}\}$ with **cutoff** $k$


Examples:
What is happening to the sequence $\{1/n\}$ and $\{(-1)^n\}$ as $n$ gets larger and larger?
1) Arbitrary close to 0
2) Never arbitrarily close to any single number
#### Convergence of Infinite Sequence

Let $\{a_{n}\}$ be a sequence and $L \in \mathbb{R}$. We say that $L$ is the **limit** of $\{a_{n}\}$ if $\forall \epsilon > 0, \exists \mathbb{N}$ s.t. if $n>N$, then
$$
|a_{n}-L|<\epsilon
$$
If such an $L$ exists, we say $\{a_{n}\}$ **converges to** $L$ and write
$$\lim_{n \to -\infty} a_{n} = L \text{ or } a_{n} \to L$$If no such $L$ exists, then we say $\{a_{n}\}$ **diverges**.

Example:
We want to show that $\lim_{n \to \infty} \frac{1}{\sqrt[3]{n}} = 0$. For now, we suppose $\epsilon = \frac{1}{1000}$
That is, $|\frac{1}{\sqrt[3]{n}} - 0| < \frac{1}{1000} \implies |\frac{1}{\sqrt[3]{n}}| < \frac{1}{1000} \iff  \frac{1}{\sqrt[3]{n}} < \frac{1}{1000}, \text{since } n>0 \iff \sqrt[3]{n} > 1000 \iff n > 1000000000$





