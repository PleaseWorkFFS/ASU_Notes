# Motivation 
Recall, the derivative at $s = a$ for some function $f$, is given by
$\begin{multline*} f'(a) = \lim_{h\to 0} \dfrac{f(a+h)-f(a)}{h} \end{multline*}$
In this setting, $a$ is representing a fixed number. For example, if $k(u) = 3u$, then 
$\begin{multline*} k'(-0.25) = \lim_{h\to 0} \dfrac{k(-0.25+h)-k(-0.25)}{h} = \lim_{h\to 0} \dfrac{3(-0.25+h)-(3(-0.25))}{h} = \lim_{h\to 0}\dfrac{-3(0.25)+3h+3(0.25)}{h} = \lim_{h\to 0}\dfrac{3h}{h} = 3 \end{multline*}$

# The Derivative as a Function
What if we let the value of $a$ vary ?
That is, treat. $a$ as a variable input for a function that outputs the derivative value at $a$. 
We call
$\begin{multline*} f'(a) = \lim_{x\to a}\dfrac{f(x)-f(a)}{x-a} \end{multline*}$
the derivative of $f$
So the equation above looks exactly the same as the equation for the derivative of $f at x = a$ 
The Difference is, $x$ is varying whereas $a$ is a fixed value. 
We can also think of $f'(x)$ as the function that takes in an $x$ value and outputs the slope of the line tangent to $y = f(x) at (x, f(x))$.

The domain of $f'$ are the values of $x$ such that 
$\begin{multline*} f'(a) = \lim_{x\to a}\dfrac{f(x)-f(a)}{x-a} \end{multline*}$
exists.
The domain of $f'$ may be smaller than the domain of $f$.

# Other notions for derivative 
The following are other ways to write the derivative of some function $y = f(x)$
-	$y'$
-	$\dfrac{dy}{dx}$
-	$\dfrac{d}{dx}f(x)$

# Differentiability 
$f$ is differentiable at $x = a$ if $f'(a)$ exists.
$f$ is differentiable on an open interval of the form 
- $(a, b)$
- $(a, \infty)$
- $(-\infty, a)$
- $(-\infty, \infty)$
If it is differentiable at every $x$-value interval.

>Example (1) :
>Where is $f(x) = |x|$ differentiable ?
>
>**Solution :**
>If $x \geq 0$, then $f(x = |x| = x)$
>$\begin{multline*} \lim_{h\to 0}\dfrac{|x+h|-|x|}{h} = \lim_{h\to 0} \dfrac{x+h-x}{h} = \lim_{h\to 0}\dfrac{h}{h} = 1 \end{multline*}$
>If $x \leq 0$, then $f(x) = |x| = -x$
>$\begin{multline*} \lim_{h\to 0}\dfrac{|x+h|-|x|}{h} = \lim_{h\to 0}\dfrac{-(x+h)-(-x)}{h} = \lim_{h\to 0}\dfrac{-h}{h} = -1 \end{multline*}$
>$\begin{multline*} \lim_{h\to 0^{-}}\dfrac{|0+h|-|0|}{h} = \lim_{h\to 0^{-}}\dfrac{|h|}{h} = \lim_{h\to 0^{-}}\dfrac{-h}{h} = -1 \end{multline*}$
>$\begin{multline*} \lim_{h\to 0^{-}}\dfrac{|0+h|-|0|}{h} = \lim_{h\to 0^{+}}\dfrac{|h|}{h} = \lim_{h\to 0^{+}}\dfrac{h}{h} = 1 \end{multline*}$
>$\begin{multline*} f'(0) = \lim_{h\to 0}\dfrac{|h|}{h} = DNE \end{multline*}$
>Hence, $f$ is differentiable on $(-\infty, 0) \cup (0, \infty)$
>The derivative of $f(x) = |x|$ is given by
>$f'(x) = \begin{cases} -1 &\ x < 0\\ 1 &\ x > 0 \end{cases}$

# Differentiability and Continuity 
It turns out, if $f$ is differentiable at $x = a$, then $f$ is continuous at $x = a$.
Well, if $f$ differentiable at $a$, 
$\begin{multline*} f'(a) = \lim_{x\to a}\dfrac{f(x)-f(a)}{x-a}\end{multline*}$
exists.
for $x \neq a$, we can write
$\begin{multline*} f(x)-f(a) = \dfrac{f(x)-f(a)}{x-a}(x-a) \end{multline*}$
so that,
$\begin{multline*} \lim_{x\to a}f(x)-f(a) = \lim_{x\to a}\dfrac{f(x)-f(a)}{x-a}(x-a) \end{multline*}$
but then,
$\begin{multline*} \lim_{x\to a}f(x)-\lim_{x\to a}f(a)=(\lim_{x\to a}\dfrac{f(x)-f(a)}{x-a})(\lim_{x\to a}x-a) \end{multline*}$
so that 
$\begin{multline*} \Big[ \lim{x\to a}f(x) \Big]-\Big[ f(a) \Big]=f'(a) \cdot 0=0 \end{multline*}$
and finally, 
$\begin{multline*} \lim_{x\to a}f(x)=f(a) \end{multline*}$
and $f$ is continuous at $x=a$

Note, the reverse is not necessarily true, if $f$ is continuous at $a$, $f$ is not necessarily differentiable at $a$

How can a function $f$ not be differentiable at some value $x=a$?
-> If $f$ is not continuous at $x=a$
-> If there are any "corners" or "kinks" in the graph of $f$ at $x=a$
-> If $f$ has a vertical tangent at $x=a$

# Higher Derivatives 
- $f"(x) :$ the second derivative of $f$, or the first derivative of $f'$
- $f'''(x) :$ the third derivative of $f$, or the first derivative of $f"$
- $f^{(4)}(x) :$ the fourth derivative of $f$, or the first derivative of $f'''$
- $f^{(n)}(x) :$ the $n^{th}$ derivative of $f$

# Higher Derivatives 
We can also use our physical and geometric interpretations for higher derivatives.
For example, $f"(x)$ can be thought of as the instantaneous rate of change of $f'(x)$ at the value $x$ or the slope of the line tangent to $y=f'(x)$ at the value $x$.
Let $s(t)$ represent an objects' position after time $t$.
We calculated the velocity $v(t)$ of the object as $v(t) = s'(t)$
The acceleration of the object $a(t)$ is the forst derivative of the velocity function, and the second derivative of the speed function.
Thus, $a(t) = v'(t) = s"(t)$

******