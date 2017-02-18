$$$\require{cancel}$$$

# 18.03
###Pset 4
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/assignments/MIT18_03S10_ps4.pdf)

#####Part 1.
######2F6b)
$$
\begin{align}
y''' + y'' -y' + 2y &= 2 cos (x)\\\
p(D) &= r^3 + r^2-r + 2\\\
p(D)y(x) &= Re\left\\{2 e^{ix}\right\\}\\\
y(x) &= {2e^{ix}\over p(i)}\\\
p(i) &= i^3 + i^2-i+2\\\
&= -i-1-i+2\\\
&= -2i+1\\\
y(x) &= Re\left\\{{2e^{ix} \over -2i+1}\right\\}\\\
&= Re\left\\{{2\left(cos(x) + isin(x)\right)\over -2i+1}\right\\}\\\
&= Re\left\\{{2\left(cos(x) + isin(x)\right)\over -2i+1} \cdot {-2i-1\over -2i-1}\right\\}\\\
&= \bbox[5px, border:2px solid black]{{-2cos(x)+4sin(x)\over-5}}
\end{align}
$$

######2F6c)
$$
\begin{align}
y'' - 2y' + 4y &= e^{x}cos(x) \\\
p(D) &= r^2-2r+4 \\\
p(D)_{y(x)} &= Re\left\\{e^{x}e^{ix}\right\\}\\\
y(x) &= {e^{(i+1)x} \over (i+1)^2-2(i+1)+4}\\\
y(x) &= {e^{(i+1)x} \over -1+2i+1-2i-2+4}\\\
y(x) &= \bbox[5px, border:2px solid black]{{e^{(i+1)x} \over 2}}\\\
\end{align}
$$

######2F6d)
Notice that in this case the $$$p(\alpha) = 0$$$, and so
the rule $$${e^{\alpha x}\over p(\alpha)}$$$ is invalid for this equation.

The formula in the case of a double root is:
$$
\begin{align}
x_p &= {x^2e^{\alpha x}\over p''(\alpha)}\\\
\end{align}
$$

We can see that this is the case for $$$p(D) = (D-\alpha)(D-\alpha)$$$ through the following calculation:

$$
\begin{align}
p(D)e^{\alpha x}f(x) &= e^{\alpha x}p(D+\alpha)f(x)\\\
D\left(e^{\alpha x}f(x)\right) &= e^{\alpha x}Df(x) + \alpha e^{\alpha x}f(x) \\\
&= e^{\alpha x}(D+\alpha)f(x)\\\
\end{align}
$$
Applying the last equation repeatedly allows the first conversion (aka 'exponential shift rule') to hold.

To see that the double root formula holds (at least for second-order differential equations):
$$
\begin{align}
&p(D) = (D-\alpha)(D-\alpha)\\\
&p'(D) = 2(D-\alpha)\\\
&p''(D) = 2\\\
\end{align}
$$
$$
\begin{align}
p(D){x^2e^{\alpha x}\over p''(\alpha)} &= e^{\alpha x}\\\
&= {e^{\alpha x}p(D+\alpha)x^2\over p''(\alpha)}\\\
&= {e^{\alpha x}D^2x^2\over 2}\\\
&= {e^{\alpha x}2\over 2}\\\
&= e^{\alpha x}
\end{align}
$$

Applying the formula to the particular problem in this case:
$$
\begin{align}
y'' - 6y' + 9y &= e^{3x}\\\
y(x)_p &= \bbox[5px, border:2px solid black]{{x^2e^{3x}\over 2}}
\end{align}
$$

######14)
$$
\begin{align}
{d^3x\over dt^3}-x &= e^{2t}\\\
p(D) &= r^3-1\\\
x_p &= e^{2t}\over p(2)\\\
x_p &= \bbox[5px, border:2px solid black]{e^{2t}\over 7}
\end{align}
$$

######2C-8)