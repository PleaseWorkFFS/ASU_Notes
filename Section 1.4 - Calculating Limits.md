# Algebraic Limit Laws
Suppose, $\lim_{x\to a} f(x) = L_{1}$, $\lim_{x\to a} g(x) = L_{2}$
that is, the limits of $f(x)$ and $g(x)$ as $x \to a$ both exist and have the values $L_{1}$ and $L_{2}$ respectively. Then,
1. $\begin{multline*}\lim_{x\to a} [f(x) + g(x)] = \lim_{x\to a} f(x) + \lim_{x\to a} g(x) = L_{1} + L_{2} \end{multline*}$ 
2. $\begin{multline*}\lim_{x\to a} [f(x) - g(x)] = \lim_{x\to a} f(x) - \lim_{x\to a} g(x) = L_{1} - L_{2} \end{multline*}$ 
3. $\begin{multline*}\lim_{x\to a} [f(x) \cdot g(x)] = \lim_{x\to a} f(x) \cdot \lim_{x\to a} g(x) = L_{1} \cdot L_{2} \end{multline*}$ 
4. $\begin{multline*}\lim_{x\to a} \dfrac{f(x)}{g(x)} = \dfrac{\lim_{x\to a} f(x)} {\lim_{x\to a} g(x)} = \dfrac{L_{1}}{L_{2}} \end{multline*}$, if $\lim_{x\to a} g(x) = L_{2} \neq 0$
Also, if $C$ is a constant, real number, then $\lim_{x\to a} C \cdot f(x) = C \cdot \lim_{x\to a} f(x)$ 

We also have, 
-> $\lim_{x\to a} C = C$, for $C$, a constant 
-> $\lim_{x\to a} x = a$, for the function $f(x) \to x$
-> $\lim_{x\to a} x^{n} = a^{n}$, for $n$, any integer
-> $\lim_{x\to a} \sqrt[n]{x} = \sqrt[n]{a}$, if $n$ even, assume $a \geq 0$
More generally, 
$\Big[ \lim_{x\to a} \sqrt[n]{f(x)} = \sqrt[n]{\lim_{x\to a} f(x)} \Big]$

>Example (1) :
>Calculate 
>1. $\lim_{x\to 5} [2x^{2}-3x+4]$
>2. $\lim_{x\to -2} \dfrac{x^3+2x^2-1}{5-3x}$

# When can we plug in x=a ?
The previous examples led us to believe there are some situations when $\begin{multline*} \lim_{x\to a} f(x) = f(a)\end{multline*}$
It turns out, if $f$ is $a$ :
-> polynomial function $i.e. f(x) = -2x^{3}-4x^{7}+9.33$
-> rational function with $a$ in the domain of $f$, $i.e. f(x) = \dfrac{x^{3}+3x^{2}-1}{5-3x}$, and plugging in $a$ doesnt' cause us to divide by $0$
-> trigonometric function, $i.e. \sin(x), \cos(x)$, etc. and $a$ is in the somain of $f$
then, 
$\lim_{x\to a} f(x) = f(a)$

>Example (2) :
>Calculate -> $\lim_{x\to \pi} x\cos(x)$
>
>**Solution :**
>we have, $\begin{multline*} \lim_{x\to \pi} x\cos(x)   \Rightarrow (\lim_{x\to \pi} x)\cdot (\lim_{x\to \pi}\cos(x)) = (\pi)\cdot (\cos(\pi)) \Rightarrow \pi \cdot (-1) = -\pi \end{multline*}$
>Hence, $\begin{multline*}\lim_{x\to \pi} x\cos(x) = -\pi\end{multline*}$

>Example (3) :
>Calculate -> $\begin{multline*} \lim_{x\to 2} \dfrac{x^{2}-4}{x-2}\end{multline*}$
>
>**Solution :**
>Note, we can write
>$\begin{multline*}\dfrac{x^{2}-4}{x-2} = \dfrac{(x+2)(x-2)}{x-2} \end{multline*}$
>If we look at values $x \neq 2$, then we can cancel the $(x-2)$ factors and write :
>$\begin{multline*}\dfrac{x^{2}-4}{x-2} = \dfrac{(x+2)(x-2)}{x-2} = x + 2 \end{multline*}$
>Remember, with limits we dont' care about the outputs when $x = a$, just $x$ near $a$.

>Example (4) :
>Calculate the following limits :
>1. $\begin{multline*} \lim_{h\to 0} \dfrac{(3+h)^{2}-9}{h} \end{multline*}$
>2. $\begin{multline*} \lim_{t\to 0} \dfrac{\sqrt{t^{2}+9}-3}{t^{2}} \end{multline*}$

# Limit Comparisons
If $f(x) \leq g(x)$ when $x$ is "near" $a$, except possibly at $a$, and both
$\begin{multline*}\lim_{x\to a}f(x) , \lim_{x\to a}g(x) \end{multline*}$
exist, then
$\begin{multline*}\lim_{x\to a}f(x) \leq \lim_{x\to a}g(x) \end{multline*}$

# Squeeze Theorem
If $f(x) \leq g(x) \leq h(x)$ near $a$, except possibly at $a$, and
$\begin{multline*} \lim_{x\to a}f(x) = L =\lim_{x\to a} h(x) \end{multline*}$
then,
$\begin{multline*} \lim_{x\to a}g(x) = L \end{multline*}$

*******