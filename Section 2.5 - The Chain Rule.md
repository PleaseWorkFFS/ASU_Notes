# Motivation
Consider the function $y = \sqrt{x^{2}+1}$
Do we have any differentiation rules available to determine $\dfrac{dy}{dx}$ ?
Well, the definition of the derivative tells us :
$\begin{multline*} \dfrac{dy}{dx} = lim_{h\to 0} \dfrac{\sqrt{(x+h)^{2}+1}- \sqrt{x^{2}-1}}{h} \end{multline*}$
$\begin{multline*} \Rightarrow \lim_{h\to 0} \dfrac{\sqrt{(x+h)^{2}+1}- \sqrt{x^{2}+1}}{h} \cdot \dfrac{\sqrt{(x+h)^{2}+1} - \sqrt{x^{2}+1}}{\sqrt{(x+h)^{2}+1}- \sqrt{x^{2}+1}} \end{multline*}$
$\begin{multline*} \Rightarrow \lim_{h\to 0}\dfrac{(h+x)^{2}+1-(x^{2}+1)}{h(\sqrt{(x+h)^{2}+1}+\sqrt{x^{2}+1})} \end{multline*}$
$\begin{multline*} \Rightarrow \lim_{h\to 0}\frac{x^{2}+2xh+h^{2}+1-x^{2}-1}{h(\sqrt{(x+h)^{2}+1}+\sqrt{x^{2}+1})} \end{multline*}$
$\begin{multline*} \Rightarrow \lim_{h\to 0}\dfrac{2x+h}{\sqrt{(x+h)^{2}+1}+\sqrt{x^{2}+1}} \end{multline*}$
$\begin{multline*} \Rightarrow \dfrac{2x}{2\sqrt{x^{2}+1}} \end{multline*}$
So, that for $y = \sqrt{x^{2}+1}$, $\begin{multline*} \dfrac{dy}{dx} = \dfrac{2x}{2\sqrt{x^{2}+1}} \end{multline*}$

THERE HAS TO BE A BETTER METHOD !!!

# Function Composition 
The function $h(x) = \sqrt{x^{2}+1}$ is an example of a composition of functions.
First, we apply the function $f(x) = x^{2} + 1$ to the input, $x$, then we apply the function $g(y) = \sqrt{y}$ to $y = \sqrt{x^{2}+1}$.
Using the function notation we can write, $h(x) = g \circ f (x) = g(f(x))$
We can also write $z = \sqrt{x^{2}+1}, y = x^{2}+1$
so that $z=\sqrt{y}$
With $x=\sqrt{y}, y=x^{2}+1$, we can write 
$\dfrac{dz}{dy} = \dfrac{1}{2\sqrt{y}}, \dfrac{dy}{dx} = 2x$
Using composition we can write,
$z=\sqrt{x^{2}+1}$
Notice, 
$\dfrac{dz}{dx} = \dfrac{dz}{dy} \dfrac{dy}{dx}$
The equation above is not exactly multiplying fractions, but we can somewhat think of the operation int that way.
We see, 
$\dfrac{dz}{dx} = \dfrac{dz}{dy} \dfrac{dy}{dx} = \dfrac{1}{2\sqrt{y}} \dfrac{2x}{1}$
And we obtain, $\dfrac{dz}{dx} = \dfrac{2x}{2\sqrt{x^{2}+1}}$ as before.

# The Chain Rule 
Let $f$ and $g$ be differentiable functions, and define
$F(x) = f \circ g (x)$
Then $F$ is differentiable and 
$F'(x) = f'(g(x))\cdot g'(x)$
The equation above is known as the **Chain Rule**
A good reminder :
"Derivative of composite function is derivative of outer function time derivative of inner function."

******