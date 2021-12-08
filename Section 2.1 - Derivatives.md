# Motivation
When talking about the derivative of a function, $f$, we want to make precise the notion of an instantaneous rate of change.
We have already seen, for linear of the form $f(x) = mx + b$, the rate of change is simple the slope, $m = \dfrac{\Delta y}{\Delta x}$
For more general functions, we want to use simpler things like slopes and straight lines to define the derivative.
Keeping in mind we want to represent a functions' instantaneous rate of change at some value $x = a$, and also using the idea of slope, it makes sense that a derivative should be realized as the slope of the line tangent to the curve $y =f(x)$ at the point $(a, f(a))$.

![[line tangent to y=f(x).png|200]]
Recall, using point-slope form, we can find the equation of any line if we know the slope of the line and a point it passes through.
If the slope of our line is $m$, and $(x_{1}, y_{1})$ is a point on our line, then the equation of the line is given by $y - y_{1} = m(x - x_{1})$ or $y = m(x - x_{1}) + y_{1}$
For equations for lines tangent to a functions' curve at some value $x+a$, we already know a point on the tangent line, namely where it is tangent to the curve $(a, f(a))$.
We must figure out the situation for the slope now.

>Example (1) :
>Consider the function $f(x) = x^{2}$
>What is the equation for the line tangent to $y=x^{2}$ at the point $(1, 1)$
>
>**Solution :**
>To find the slope of this line, we need to calculate
>$\begin{multline*} \lim_{x\to 1}\dfrac{f(x)-f(1)}{x=1} = \lim_{x\to 1}\dfrac{x^{2}-1}{x-1} = \lim_{x\to 1}\dfrac{(x+1)(x-1)}{x-1} = \lim_{x\to 1} x+1 = 2 \end{multline*}$
>We see the slope of the tangent is $m = 2$, thus the equation for the tangent line is 
>$L = 2(x - 1)+1$

# Slopes of Tangents 
The tangent line to the curve $y = f(x)$, at the point $(a, f(a))$, is the line through the point $(a, f(a))$ with slope $\begin{multline*} m = \lim_{x\to a} \dfrac{f(x)-f(a)}{x-a} \end{multline*}$
provided this limit exists.
Performing the transformation, $h = x - a$ (so that $x = a + h$), we can equivalently write the slope of the tangent line as $\begin{multline*} m = \lim_{h\to 0}\dfrac{f(a+h)-f(a)}{h} \end{multline*}$
provided this limit exists. 

>Example (2) :
>Find the equation of the tangent line to the hyperbola $f(x) = \dfrac{3}{x}$ at the point $(3, 1)$.
>
>**Solution :**
>We have the point $(3, 1)$, we just need the slope:
>$\begin{multline*} m = \lim_{h\to 0}\dfrac{f(3+h)-f(3)}{h} = \lim_{h\to 0}\dfrac{(\dfrac{3}{3+h})-1}{h} = \lim_{h\to 0} \dfrac{(\dfrac{3}{3+h}-1)}{h}\cdot \dfrac{\dfrac{3+h}{3+h}}{1}\end{multline*}$ 
>$\begin{multline*}= \lim_{h\to 0}\dfrac{\dfrac{3-(3+h)}{3+h}}{h} = \lim_{h\to 0}\dfrac{\dfrac{-h}{3+h}}{h} = \lim_{h\to 0}\dfrac{-h}{3+h}\cdot \dfrac{1}{h} = \lim_{h\to 0}\dfrac{-1}{3+h} = \dfrac{-1}{3} \end{multline*}$
>We obtain the equation for the tangent line :
>$y = -(\dfrac{1}{3})x + 2$

# The Velocity Problem 
Suppose an object moves along the path according to the equation of motion $s = f(t)$
$s = f(t)$ is the position function for our object. If $t$ represents time, and $t$ changes from $t = a to t = a + h$, we have 
$\Delta s = f(a+h)-f(a)$ is the change in position
$\Delta t = (a+h)-a = h$ is the change in time 
The average velocity, or average rate of change for $f(t)$, is given by 
$\bar{m} = \dfrac{\Delta s}{\Delta t} = \dfrac{f(a+h)-f(a)}{h}$

Looking familiar ?

If an objects' position is modeled by $s = f(t)$, where $t$ is a unit of time (sec, min, etc.), the velocity of the object, or instantaneous velocity, at $t = a$ is given by 
$\begin{multline*} v(a) = \lim_{h\to 0}\dfrac{f(a+h)=f(a)}{h} \end{multline*}$

# Bringin' it all together 
We have seen the same limit of difference quotients arise when calculating slopes of lines tangent to curves and instantaneous velocities.
The same limit arises whenever we calculate an instantaneous rate of change. 
#### Definition ( The Derivative )
The _derivative_ of a function $f$, at a number $x = a$, denoted $f'(a)$, is given by :
$\begin{multline*} f'(a) = \lim_{h\to 0}\dfrac{f(a+h)-f(a)}{h} \end{multline*}$
provided this limit exists. If the limit does not exist, we say $f$ is differentiable at $x = a$. We may also use 
$\begin{multline*} f'(a) = \lim_{x\to a}\dfrac{f(x)-f(a)}{x-a} \end{multline*}$

# Average Rate of Change 
Suppose $y=f(x)$ is a function.
Given two instances of $x$, $x_{1,} and x_{2}$ and corresponding $y$ values, $y_{1} and y_{2}$, we write the "change in $x$" and "chanhe in $y$" as
$\Delta x = x_{2} - x_{1}$, $\Delta y = y_{2} - y_{1}$

The average rate of change of $f$ over the interval $[a, b]$ is given by 
$\dfrac{\Delta y}{\Delta x} = \dfrac{f(b)-f(a)}{b-a}$
We see that we can obtain the instantaneous rate of change at $x=a$ by taking a limit of average rates of change, that is 
$\begin{multline*} f'(a) = \lim_{x\to a}\dfrac{f(x)-f(a)}{x-a} \end{multline*}$