# Motivation
Recall, certain functions like polynomials and some trigonometric functions satisfy
$\begin{multline*} \lim_{x\to a}f(x) \end{multline*}$
For example, 
$\begin{multline*} \lim_{x\to \pi} \cos(x) = \cos(x) = -1 \end{multline*}$
$\begin{multline*} \lim_{t\to 3.77}[t^{2}+3] = (3.7)^{2}+3 = 16.69 \end{multline*}$
$\begin{multline*} \lim_{q\to \frac{-1}{4}}\dfrac{4-q^{3}+2q}{1-q} = \dfrac{4-(\dfrac{-1}{4})^{3}+2(\dfrac{-1}{4})}{1-(\dfrac{-1}{4})} = 2.8125 \end{multline*}$
They key idea is that the functions above are continuous at the input values of interest.

# Continuity
A function, $f$, is continuous at a number, $x = a$, if :
$\begin{multline*} \lim_{x\to a} f(x) = f(a) \end{multline*}$
Notice, we need three things to occur, 
1. $f$ must be defined at $x = a, i.e.$ we can plug $a$ into $f$.
2. $\lim_{x\to a} f(x)$ must exist
3. $\lim_{x\to a} f(x) = f(a)$
If any of these three conditions isnt' satisfied, we say $f$ is discontinuous at $a$.

# Types of Discontinuities
We will deal with three types of discontinuities:
#### Removable Discontinuity
A discontinuity of a function, $f$, is removable if at $a$ there exists a function, $g$, that is continuous at $a$ and satisfies $g(x) = f(x), x\neq a$.
Example, 
$f(x) = \dfrac{x^{2}-4}{x-2}$ discontinuous at $x=2$, but away from $x=2$, $f(x) = x+2$
#### Infinite Discontinuity
A discontinuity of a function, $f$, is infinite discontinuity at $a$ if either
$\begin{multline*} \lim_{x\to a^{-}}f(x) and \lim_{x\to a^{+}}f(x) \end{multline*}$
are unbounded, that is approach $\pm \infty$
#### Jump Discontinuity 
A discontinuity of a function, $f$, is a jump discontinuity at $a$ if both
$\begin{multline*} \lim_{x\to a^{-}}f(x) and \lim_{x\to a^{+}}f(x) \end{multline*}$
exist, but are not real

# Infinite Discontinuity
$\begin{multline*} f(x) = \tan(x) = \dfrac{\sin(x)}{\cos(x)} \end{multline*}$

# Continuity and Limits 
If $f$ is continuous at $b$, and $g$ is a function satisfying 
$\begin{multline*} \lim_{x\to a}g(x) = b \end{multline*}$
then, 
$\begin{multline*} \lim_{x\to a}f(g(x)) = f(b) \end{multline*}$
in other words, 
$\begin{multline*} \lim_{x\to a} f(g(x)) = f(\lim_{x\to a}g(x)) \end{multline*}$
We see that for continuous functions, like $f$ above, we can commute, or exchange the order of taking a limit and plugging into $f$.
If $g$ is continuous at $a$, and $f$ is continuous at $g(a)$, then $f \circ g$ is continuous at $a$.
$f \circ g = f(g(x))$

# Left and Right Continuity 
A function, $f$, is continuous from the left at $a$ if:
$\begin{multline*} \lim_{x\to a^{-}} f(x) = f(a) \end{multline*}$
A function, $f$, is continuous from the right at $a$ if:
$\begin{multline*} \lim_{x\to a^{+}} f(x) = f(a) \end{multline*}$
A function, $f$, is continuous on an interval if $f$ is continuous at every point inside the interval.
If the interval has endpoints, we use the corresponding type of either left or right continuity.

# Intermediate Value Theorem 
Suppose $f$ is continuous on a closed interval, $[a,b]$. Let $N$ be any number between $f(a) and f(b)$, where $f(a) \neq f(b)$, there exists a number, $c$, in the open interval, $(a, b)$, such that $f(c) = N$

# Continuity and Algebra 
If $f and g$ are continuous at $a$, what can we say about :
-> $f+g ?$
-> $f-g ?$
-> $f\cdot g ?$
-> $\dfrac{f}{g} (if g(a)\neq 0)$
-> $cf$, for constant number
These are all continuous as well 
~EXTRA CREDIT~

*******