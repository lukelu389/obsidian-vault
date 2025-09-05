**Real and Transcendental Functions** 

1. Real-Valued Functions
	Let $X$ and $Y$ be sets. A function $f$ is a mapping that assigns to each $x\in X$ exactly one $y=f(x) \in Y$. We use the notation:
	$$f:X\to Y,    x\mapsto f(x) $$
	![[Screenshot 2025-09-03 at 3.26.00 PM.png]]
	1.1 
		Let $f:X\to Y$ be a function. We call the set of numbers for which the function $f$ is well defined the **domain** of $f$.
		$$D(f) = \{x:f(x) \text{ is well defined\} }$$
		The **range** of a function $f:X\to Y$ is the set
		$$R(f) = \{f(x): x \in X\} $$
		Parity of Function:
			A function $f$ is called **even** if $f(-x)=f(x)   \text{ }  \forall  x\in D$ 
			A function $g$ is called **old** if $g(-x) = -g(x) \text{ } \forall x\in D$ 
	1.2  
		Examples of transcendental functions and its domain and range
		 $$
\begin{array}{|c|c|c|}
\hline
\textbf{Function} & \textbf{Domain} & \textbf{Range} \\
\hline
y = x & \mathbb{R} & \mathbb{R} \\
\hline
y = x^2 & \mathbb{R} & [0,\infty) \\
\hline
y = \sqrt{x} & [0,\infty) & [0,\infty) \\
\hline
y = \tfrac{1}{x} & \mathbb{R}\setminus\{0\} & \mathbb{R}\setminus\{0\} \\
\hline
e^x & \mathbb{R} & (0,\infty) \\
\hline
\ln(x) & (0,\infty) & \mathbb{R} \\
\hline
\sin(x) & \mathbb{R} & [-1,1] \\
\hline
\cos(x) & \mathbb{R} & [-1,1] \\
\hline
\tan(x) & \mathbb{R}\setminus\{\tfrac{\pi}{2}+k\pi: k\in\mathbb{Z}\} & \mathbb{R} \\
\hline
\arcsin(x) & [-1,1] & \left[-\tfrac{\pi}{2}, \tfrac{\pi}{2}\right] \\
\hline
\arccos(x) & [-1,1] & [0,\pi] \\
\hline
\arctan(x) & \mathbb{R} & \left(-\tfrac{\pi}{2}, \tfrac{\pi}{2}\right) \\
\hline
\end{array}
$$
	1.3.1
		Composite functions
		Let $f:X\to Y$ and $g:Y\to Z$
		The composition of $f$ and $g$, denoted $g \circ f$ 
		$g \circ f: X\to Z$, $(g \circ f)(x) = g(f(x))$ 
	1.3.2
		Inverse functions
		Let $f:X\to Y$ be a function with domain $X$ and range $Y$. Then $f$ is invertible if $\exists f^-1: Y\to X$ so that 
		$$f^-1(f(x)) = x  \;  \forall x \in X \text{ and } f^-1(f(x)) = x\;  \forall x\in Y $$
	Examples:
		$f(x) = \frac{x}{x^2-x} = \frac{x}{(x-1)(x)}; x\neq 0, 1$ 
		Therefore the domain should be $x\in \mathbb{R} \setminus \{0, 1\}$, alternatively $x \in (\infty, 0) \cup (0, 1)\cup (1, \infty)$ 
		