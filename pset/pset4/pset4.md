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

To get the general solution, notice that:
$$
\begin{align}
{d^3x\over dt^3}-x &= 0\\\
r^3-1 &= 0\\\
(r+i)(r-i)(r-1) &= 0\\\
\end{align}
$$

And therefore we can write that the general solution is:
$$
\bbox[5px, border:2px solid black]{C_1e^{-it} + C_2e^{it} + C_3e^{t} + {e^{2t}\over 7}}
$$

######2C-8c)
$$
\begin{align}
y'' + y' + y &= 2xe^{x}\\\
p(D) &= D^2 + D + 1\\\
p(D)y &= 2xe^{x}\\\
y_p &= f(x)e^{x}\\\
p(D)f(x)e^{x} &= e^{x}p(D+1)f(x)\\\
e^{x}p(D+1)f(x) &= 2xe^{x}\\\
p(D+1)f(x) &= 2x\\\
p(D+1) &= (D+1)^2 + (D+1) + 1\\\
p(D+1) &= D^2 + 2D + 1 + (D+1) + 1\\\
p(D+1) &= D^2 + 3D + 3\\\
f(x) &= Ax + B\\\
f'(x) &= A\\\
f''(x) &= 0\\\
p(D+1)f(x) &= 2x\\\
D^2f(x) + 3Df(x) + 3f(x) &= 2x\\\
0 + 3A + (3Ax+3B) &= 2x\\\
3Ax + 3A + 3B &= 2x\\\
3A + 3B &= 0\\\
3A &= 2\\\
A &= {2\over 3}\\\
B &= -{2\over 3}\\\
y_p &= \bbox[5px, border:2px solid black]{e^{x}\left({2\over 3}x - {2\over 3}\right)}
\end{align}
$$

For the general solution, we need to find the associated equation:
$$
\begin{align}
y''+ y' + y &= 0\\\
r^2 + r + 1 &= 0 \\\
\left(r-{-1+i\sqrt3\over2}\right)\left(r-{-1-i\sqrt3\over2}\right) &= 0 \\\
\end{align}
$$
$$\bbox[5px, border:2px solid black]{y(x) = C_1e^{1-i\sqrt3\over2} + C_2e^{1+i\sqrt3\over2} + e^{x}\left({2\over3}x-{2\over3}\right)}$$

######2C-8d)
Step 1: Find a particular solution $$$y_p$$$:
$$
\begin{align}
y'' - y &= x^2\\\
p(D) &= D^2-1\\\
p(D)u(x) &= x^2\\\
u(x) &= Ax^2+Bx+C\\\
u'(x) &= 2Ax+B\\\
u''(x) &= 2A\\\
p(D)u(x) &= x^2\\\
D^2u(x)-u(x) &= x^2\\\
2A-Ax^2+Bx+C &= x^2\\\
A &= -1\\\
B &= 0\\\
C &= -2\\\
u(x) &= -x^2-2\\\
\end{align}
$$

Step 2: Find a complementary solution $$$y_c$$$:
$$
\begin{align}
y'' - y &= 0\\\
r^2-1 &= 0\\\
(r+1)(r-1) &= 0\\\
y(x) &= C_1e^{-x} + C_2e^{x}\\\
\end{align}
$$

$$\therefore \bbox[5px, border:2px solid black]{y(x) = -x^2-2+C_1e^{-x}+C_2e^{x}}$$

Step 3: Include the initial conditions:
$$
\begin{align}
y(0) &= 0\\\
y'(0) &= -1\\\
y(x) &= -x^2-2+C_1e^{-x}+C_2e^{x}\\\
y(0) &= -(0)^2-2+C_1e^{0}+C_2e^{0}\\\
0 &= -2 + C_1 + C_2\\\
y'(x) &= -2x - C_1e^{-x}+C_2e^{x}\\\
y'(0) &= -2(0) - C_1e^{0}+C_2e^{0}\\\
-1 &= -C_1 + C_2\\\
C_1-1 &= C_2\\\
0 &= -2 + C_1 + C_1-1\\\
3 &= 2C_1\\\
C_1 &= {3\over 2}\\\
C_2 &= {1\over 2}\\\
\end{align}
$$
$$\therefore \bbox[5px, border:2px solid black]{y(x) = -x^2-2 + {3\over 2}e^{-x} + {1\over 2}e^{x}}$$

