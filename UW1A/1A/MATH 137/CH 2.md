**Triangle Inequality**
$|x-y|\leq|x-z|+|z-y|$
	It suggests the straight distance between two points is a direct line
	Proof: (number line)
		Without loss of generality, suppose $x \leq y$
			swap $x$ and $y$, $|x-y|\leq|x-z|+|z-y|$ <=> $|y-x|\leq|x-z|+|y-z|$ <=> $|x-y|\leq |x-z|+|z-y|$   
		Case 1($z\leq x\leq y$):
			$|x-y|\leq|z-y\leq|x-z|+|z-y|$ 
		Case 2($x\leq z\leq y$):
			$|x-y|=|x-z|+|z-y|$ so $|x-y|\leq|x-z|+|z-y|$
		Case 3($x\leq y\leq z$):
			$|x-y|\leq|x-z|+|z-y|$
**Triangle Inequality 2**
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
3) $|0<|x-a|\leq\delta$ implies $x \in (a-\delta, a) \cup (a, a+\delta)$

Practice questions:
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
	$\frac{x+2}{2-x} > 5\iff x+2>10-5x \iff \frac{x>4}{3}$
	Case 3($x>2$):
	$\frac{x+2}{x-2}> 5 \iff x+2>5x-10\iff 3>x$
	Solution interval Case 2 + Case 3
