$$$\require{cancel}$$$

# 18.03
###Pset 5
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/assignments/MIT18_03S10_ps5.pdf)

#####Part I
######a) 2.5 8)
$$
\begin{align}
y'' - 4y &= cosh(2x)\\\
&= {e^{2x} + e^{-2x}\over 2}\\\
y'' - 4y &= {1\over2}e^{2x}\\\
p(D) &= D^2 - 4\\\
p'(D) &= 2D\\\
y\_{p1} &= {1\over2}{te^{2x}\over p'(2)}\\\
y\_{p1} &= {1\over2}{te^{2x}\over 4}\\\
y'' - 4y &= {1\over2}e^{-2x}\\\
y\_{p2} &= {1\over2}{te^{-2x}\over p'(-2)}\\\
y\_{p2} &= {1\over2}{te^{-2x}\over 4}\\\
y\_{p} &= {1\over2}{t\left(e^{2x} + e^{-2x}\right)\over 4}\\\
&= \bbox[5px, border:2px solid black]{{t\left(e^{2x} + e^{-2x}\right)\over 8}}\\\
\end{align}
$$
######b)
$$
\begin{align}
\ddot{x} + x &= t^2 + cos(2t-1)\\\
\ddot{x} + x &= t^2\\\
x\_{p1} &= At^2 + Bt + C\\\
\dot{x\_{p1}} &= 2At + B\\\
\ddot{x\_{p1}} &= 2A\\\
\ddot{x\_{p1}} + {x\_{p1}} &= t^2\\\
2A + At^2 + Bt + C &= t^2\\\
A &= 1\\\
B &= 0\\\
C &= -2\\\
x_{p1} &= \bbox[5px, border:2px solid black]{t^2-2}\\\
\ddot{x} + x &= cos(2t-1)\\\
\ddot{x} + x &= cos(2t)\\\
p(D) &= D^2 + 1\\\
p(D)x\_{p2} &= Re\left\\{e^{2it}\right\\}\\\
x\_{p2} &= Re\left\\{{e^{2it}\over p(2i)}\right\\}\\\
x\_{p2} &= Re\left\\{e^{2it}\over (2i)^2+1\right\\}\\\
x\_{p2} &= Re\left\\{cos(2t) + isin(2t)\over -3\right\\}\\\
x\_{p2} &= \bbox[5px, border:2px solid black]{-{cos(2t) \over 3}}\\\
x\_p &= \bbox[5px, border:2px solid black]{t^2 - 2 - {cos(2t-1)\over 3}}\\\
\end{align}
$$

#####Part II
######17)


