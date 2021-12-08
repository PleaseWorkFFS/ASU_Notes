# Motivation 
Why are limits important ?
Calculus has two halves : Defferentiation and Integration 

**Differentiation :** Quantitatively describing how a function's values change 
**Integration :** Using information about how values of a function change to obtain information about the function itself 

>Example (1) :
>If $\Big[s(t) = 3t+5]$ models the position of a particle in feet from a starting position, what is the velocity of the particle ?

>Example (2) :
>If at time, $t=0$, a particle is 5 feet from its' starting position and moves with a velocity of $3 ft/s$, what is the expression for the particles' position, $s(t)$ ?

But what if the functions of interest are not linear or the rates of change are not constant ?
It turns out, we can deal with general situations using the techniques for linear functions.

# Limits 
In order to make the previous procedures precise, we will need the definition of a limit.

## Definition 
Suppose the function, $f$, is defined when $x$ is "near"(Near means $f$ has outputs on an interval containing $a$ except maybe $a$ itself) a number, $a$.
We say, 
$\begin{equation} \lim_{x\to a} f(x)=L \end{equation}$
"The limit of $f(x)$ approaches $a$ equals $L$", if we can make the values of $f(x)$ as close to the value of $L$ as we desire by taking values of $x$ close to, but not equal to $a$.
The question we want to ask is : "What do the output values, $f(x)$, approach as we simultaneously plug in values that are getting closer to $a$ ?"

## Numerical Limits 
Consider the function $t(y)=\dfrac{y^{2}-4}{y-2}$
We wish we could calculate $\big[\lim_{y\to 2} t(y)\big]$ without using a graph .

When using a functions' graph to calculate a limit, we trace along the functions' curve approaching the input value of interest. Here, our input value of interest is $y=2$.

Tracing along the curve of $t(y)$ corresponds to plugging in a set of values of $t$ that increase to the value $y=2$, and a set of values that decreases to $y=2$.

For values of $y$ increasing to $y=2$, lets' take $y=1.9, 1.99, 1.999$
For values of $y$ decreasing to $y=2$, lets' take $y=2.01, 2.001, 2.0001$
After plugging these values in we see, 
$t(1.9)=3.9$ | $t(1.99)=3.9900$ | $t(1.999)=3.9990$
$t(2.01)=4.010$ | $t(2.001)=4.0010$ | $t(2.0001)=4.00010$

$\lim_{y\to 2} t(y)=4$

# One-Sided Limits 
Notice in every limit example, we have investigated input values that both increase to our input of interest, and decease to our input of interest. We write $\Big[\lim_{x\to a^{-}}f(x)=L\Big]$ and say "the limit of $f(x)$ as $x$ approaches from the left is equal to $L$", if we can make the output values, $f(x)$, sufficiently close to $L$ by taking values sufficiently close to $a$ that are less than $a$. 
When we approach $a$ from left, we plug input values that increase to $a$.

We write $\Big[\lim_{x\to a^{+}}f(x)=L\Big]$ and say "the limit of $f(x)$ as $x$ approaches from the right is equal to $L$", if we can make the output values, $f(x)$, sufficiently close to $L$ by taking values sufficiently close to $a$ that are greater than $a$. 
When we approach $a$ from the right, we plug in input values that decrease to $a$.

From our procedures, graphical and numerical, we see :
$\Big[\lim_{x\to a} f(x) = L\Big]$
if and only if, 
$\Big[\lim_{x\to a^{-}}f(x) = L = \lim_{x\to a^{+}}f(x)\Big]$

If it is the case such that :
$\Big[\lim_{x\to a^{-}}f(x) = L_{1} \neq L_{2} = \lim_{x\to a^{+}}f(x)\Big]$
Then we say, "the limit of $f(x)$ as $x$ approaches $a$ _does not exist_". In this situation, we write :
$\Big[ \lim_{x\to a} f(x) = DNE \Big]$
 
 In practice, calculating the one-sided limits and showing equality of these limits is how one obtains a limiting value.
 
 >Example (3) :
 >$f_{n} \begin{cases} p^{2} &-\infty < p \leq 2 \\ p + 2 &2 < p \leq 3 \\ \sin(p) &3 < p \leq \infty \end{cases}$
	 >Calculate the following values if they exist, otherwise, write "DNE" :
	 >$\lim_{p\to 2^{-}} h(p)$, $\lim_{ p\to 2^{+} } h(p)$, $\lim_{p\to 2} h(p)$, $h(2)$
	 >$\lim_{p\to 3^{-}} h(p)$, $\lim_{p\to 3^{+}} h(p)$, $\lim_{p\to 3} h(p)$, $h(3)$

^bed6c2

>Example (4) :
>Let $n(\theta) = \dfrac{1}{\theta^{2}}$
>Calculate -> $\lim_{\theta\to 0} n(\theta)$
> 
>**Solution :** 
>Here, we see that as $\theta$ increases to $0$, $n(\theta)$ gets larger and larger. We write, 
>$\Big[ \lim_{\theta\to 0^{-}} n(\theta) = \infty \Big]$
>to depict this phenomenon. The left handed limit does not exist because the output values do not approach a finite number, but we can still describe the behavior. Similarly we can write, 
>$\Big[ \lim_{\theta\to 0^{+}} n(\theta) = \infty \Big]$
>using the same idea.
>Although on both sides of $\theta = 0$, the output of $n$ gets larger and larger, the limit as $\theta$ approaches $0$ does not exist since we dont' approach a finite number. 
>However, we can still describe the behavior of as $\theta$ approaches $0$ by :
>$\Big[ \lim_{\theta\to 0} n(\theta) = \infty \Big]$

^16138b

# A couple of ways to say the same thing ...
"The limit of $f(x)$ as $x$ approaches $a$ equals $L$" -> $\lim_{x\to a} f(x) = L$

"As $x$ approaches $a$, $f(x)$ approaches $L$" -> $x \to a$, $f(x) \to L$

We can use the same words and symbols in the one-sided limit situations as well : 
"As $x$ approaches $a$ from the left, $f(x)$ approaches $L$" -> $\lim_{x\to a^{-}} f(x) = L$

******