# Derivatives of Simple Functions 
Recall the definition of the derivative 
$\begin{multline*} f'(x)=\lim_{x]to a}\dfrac{f(x+h)-f(x)}{h} \end{multline*}$
What if $f(x) = c$, where $c$ is a constant real number ?
$\begin{multline*} f'(x)=\lim_{x\to a}\dfrac{c-c}{h} = 0 \end{multline*}$
Hence, constant functions $f(x)=c$ always satisfy $f"(x)=0$ for all $x$

What about $f(x)=x$?
$\begin{multline*} f'(x) = \lim_{h\to 0}\dfrac{(x+h)-x}{h} = \lim_{h\to 0}\dfrac{1}{1} = 1 \end{multline*}$
Hence, the derivative of $f(x)=x$ is $f'(x)=1$ for all $x$.

# The Power Rule 
Let $n$ be a real number with $n \neq 0$.
**Power Rule :** $\dfrac{d}{dx}(x^{n})=nx^{x-1}$
That is, to take the derivative of $x^{n}$, take the exponent, $n$, and bring it out in front of $x$ as a multiplier, and subtract one from the exponent.

# Making new derivatives out of old 
Let $C$ be a constant, real number, and find $f$ a differentiable function.
$\begin{multline*} \dfrac{d}{dx}(C\cdot f(x))=c\dfrac{d}{dx}(f(x)) \end{multline*}$

If $f$ and $g$ are differentiable functions, then 
$\begin{multline*} \dfrac{d}{dx}(f(x)+g(x)) = \dfrac{d}{dx}(f(x)) + \dfrac{d}{dx}(g(x)) \end{multline*}$
$\begin{multline*} \dfrac{d}{dx}(f(x)+g(x)) = \lim_{h\to 0}\dfrac{f(x+h)+g(x+h)-[f(x)+g(x)]}{h} \end{multline*}$
$\begin{multline*} \Rightarrow \lim_{h\to 0}\dfrac{f(x+h)-f(x)+g(x+h)-g(x)}{h} \end{multline*}$
$\begin{multline*} \Rightarrow \lim_{h\to 0}\dfrac{f(x+h)-f(x)}{h} + \lim_{h\to 0}\dfrac{g(x+h)-g(x)}{h} \end{multline*}$
$\begin{multline*} \Rightarrow \dfrac{d}{dx}(f(x)) +\dfrac{d}{dx}(g(x)) \end{multline*}$
*Works for Finite Sums, i.e. $\dfrac{d}{dx}(f(x)+g(h)+h(x))$*

#### Sin(x) and Cos(x)
1. $\dfrac{d}{dx}\Big( \sin(x) \Big) = \cos(x)$
2. $\dfrac{d}{dx}\Big( \cos(x) \Big) = -\sin(x)$

$\begin{multline*} \lim_{h\to 0}\dfrac{\sin(x+h)-\sin(x)}{h} = \lim_{h\to 0}\dfrac{\sin(x)\cos(h) +\sin(h)\cos(x) -\sin(x)}{h} \end{multline*}$
$\begin{multline*} \Rightarrow \lim_{h\to 0} \sin(x)\dfrac{\cos(h) -1}{h} + \lim_{h\to 0}\cos(x)\dfrac{\sin(h)}{h} \end{multline*}$
$\begin{multline*} \Rightarrow \sin(x) \lim_{h\to 0}\dfrac{\cos(h)-1}{h} + \cos(x) \lim_{h\to 0}\dfrac{\sin(h)}{h} \end{multline*}$
$\begin{multline*} \Rightarrow \sin(x)\cdot 0 + \cos(x)\cdot 1 = \cos(x) \end{multline*}$

*****