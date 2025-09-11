### Definition of function
```racket
(define (funciton-name parameters) (procedures))
```
- An evaluation step is a substitution step in racket 

### Predicates
```racket
(define (helper-funcitons? parameter) (statements))
```

### Identifiers
- Can contain letters, numbers `-, _, ., ?, =` and some other characters
- Cannot contain space, brackets of any kind, or quotation marks
- Must contain at least one non-number

### Substitution Rules
- **Leftmost/inner subexpression**(i.e. first closing bracket)
- Boolean Operators:
	![[Screenshot 2025-09-11 at 11.03.36 AM.png]]
- User-defined function:
	![[Screenshot 2025-09-11 at 11.03.12 AM.png]]
- Constant definition substitute one at a time when they are met

### Inexact Numbers
The range of an exact number is around $\pm 2.23e-308 \text{ to } \pm 1.80e308$
When we want to indicate that a function could produce or consume any type of number, we write `Num`.
The `number?` predicate tests if something is a `Num`

Build-in Math Functions

$$
\begin{array}{|c|c|}
\hline function & functionality \\
\hline \text{abs} & \text{absolute value of a Num} \\
\hline \text{sqrt} & \text{square root of a Num} \\
\hline \text{log} & \text{ln of a Num} \\
\hline \text{exp} & \text{e raised to a Num} \\
\hline
\end{array}
$$