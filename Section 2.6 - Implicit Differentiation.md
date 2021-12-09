# Motivation
We know how to differentiate functions of the form $f(x) = x\sin(x)$ and $y=\sqrt{x^{3}+1}$
But what about an equation of the form $x^{2}+y^{2}=25$ or $x^{3}+y^{3}=6xy$ ?

# Implicit Differentiation
To deal with differentiating the equations previously described, we will use a technique called **Implicit Differentiation**.

Taking the example mentioned previously, differentiate $x^{2}+y^{2}=25$

We begin with taking derivative w.r.t. $x$ on both sides of the equation
$\dfrac{d}{dx}(x^{2}+^{2}) = \dfrac{d}{dx}(25)$
Since the derivative of constant functions is always $0, \dfrac{d}{dx}(25) = 0$

$\dfrac{d}{dx}(x^{2}+y^{2}) = \dfrac{d}{dx}{x^2}+\dfrac{d}{dx}(y^{2})$
Like we have seen before, $\frac{d}{dx}(x^{2}) = 2x$ by Power Rule ( [[Section 2.3 - Basic Differentiation Formulae#The Power Rule]] ). Since we treat $y$ as a function of $x$, we will need to use The Chain Rule ( [[Section 2.5 - The Chain Rule#The Chain Rule]] ) to differentiate $y^{2}$, i.e. $\dfrac{d}{dx}(y^{2}) = 2y \dfrac{dy}{dx}$
and we obtain $2x + 2y\dfrac{dy}{dx} = 0$
To obtain $\dfrac{dy}{dx}$, we solve the equation algebraically 
$2x + 2y\dfrac{dy}{dx} = 0 \to 2y\dfrac{dy}{dx}=-2x \to \dfrac{dy}{dx}=\dfrac{-2x}{2y}=-\dfrac{x}{y}$
So, $\dfrac{dy}{dx}=-\dfrac{x}{y}$

*******