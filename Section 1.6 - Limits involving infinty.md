Recall from [[Section 1.3 - Limits#^16138b]], the example
$\begin{multline*} \lim_{x\to 0} \dfrac{1}{x^{2}} \end{multline*}$
This limit did not exist, but we used the notation
$\begin{multline*} \lim_{x\to 0} \dfrac{1}{x^{2}} = \infty \end{multline*}$
to depict that as $x$ approaches $0$ from either side, the output values $f(x)$ become arbitrarily large.

# Infinite Limits
The equation
$\begin{multline*} \lim_{x\to a}f(x) = \infty \end{multline*}$
means the the values of $f(x)$ increase without bound as we take $x$ sufficiently to $a$, but never equal.
We equivalently say "as $x$ approaches $a$, $f(x)$ increases without bounds, or as $x \to a, f(x) \to \infty$"
Similarly,
$\begin{multline*} \lim_{x\to a}f(x) = -\infty \end{multline*}$
means the the values of $f(x)$ decrease without bound as we take $x$ sufficiently to $a$, but never equal.
We equivalently say "as $x$ approaches $a$, $f(x)$ decrease without bounds, or as $x \to a, f(x) \to -\infty$"

# Vertical Asymptotes
The line, $x = a$, is a vertical asymptote of the curve, $y = f(x)$, if any one of the following are true :
-	$\begin{multline*} \lim_{x\to a^{-}} f(x) = \pm \infty \end{multline*}$
-	$\begin{multline*} \lim_{x\to a^{+}} f(x) = \pm \infty \end{multline*}$

# Horizontal Asymptotes 
Consider the function $f(x) = \dfrac{x^{2}+1}{x^{2}-1}$
What do the output values approach if we increase $x$ without bound ? What if we decrease $x$ without bound ?

Let $f$ be a function defined on the interval $(a, \infty)$ for some number $a$
$\begin{multline*} \lim_{x\to \infty} f(x) = L \end{multline*}$
means we can make the values $f(x)$ as close as we like to the value $L$ by taking $x$ sufficiently large. 
We say "as $x$ increases without bound, $f(x)$ approaches $L$"
Or, as $x\to \infty, f(x) \to L$
Similarly, 
Let $f$ be a function defined on the interval $(a, -\infty)$ for some number $a$
$\begin{multline*} \lim_{x\to -\infty} f(x) = L \end{multline*}$
means we can make the values $f(x)$ as close as we like to the value $L$ by taking $x$ sufficiently negative. 
We say "as $x$ decreases without bound, $f(x)$ approaches $L$"
Or, as $x\to -\infty, f(x) \to L$

>$\begin{multline*} \lim_{x\to \pm \infty} f(x) = \pm \infty \end{multline*}$
>Values of $f(x)$ increase/decrease without bounds as the value of $x$ increases/decreases without bound

******