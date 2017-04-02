$$$\require{cancel}$$$

# 18.03
###Pset 5
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/assignments/MIT18_03S10_ps5a.pdf)

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
######17a)
$$
\begin{align}
&R=  100\Omega\\\
&L= 500mH\\\
&C= 50\mu F\\\
&V_0= 250V\\\
&\omega= 200 rad/s\\\
\end{align}
$$
In terms of putting I in phase with V, it seems like only changes in $$$C$$$ have effect, if $$$L$$$ and $$$\omega$$$ are fixed.

######17b)
$$
\begin{align}
V(t) &= V_0sin(\omega t)\\\
{dV(t)\over dt} &= {d\over dt}V_0sin(\omega t)\\\
&= V_0\omega cos(\omega t)\\\
&= Re\left\\{V_0\omega e^{i\omega t}\right\\}\\\
L{d^2I(t)\over dt^2} + R{dI(t)\over dt} + {1\over C}I(t) &= {dV(t)\over dt}\\\
p(D) &= {LD}^2 + RD + {1\over C}\\\
p(D)I(t) &= Re\left\\{V_0\omega e^{i\omega t}\right\\}\\\
I(t) &= Re\left\\{{e^{i\omega t} \over p(i\omega)}\right\\}\\\
&= Re\left\\{{e^{i\omega t}\over L(i\omega)^2 + R(i\omega) + {1\over C}}\right\\}\\\
&= Re\left\\{{e^{i\omega t}\over \left({1\over C} - L\omega^2\right) + i\left(R\omega\right)}\right\\}\\\
&= Re\left\\{{e^{i\omega t}\left(\left({1\over C} - L\omega^2\right) - i\left(R\omega\right)\right)\over \left(\left({1\over C} - L\omega^2\right) + i\left(R\omega\right)\right)\left(\left({1\over C} - L\omega^2\right) - i\left(R\omega\right)\right)}\right\\} \\\
&= Re\left\\{{e^{i\omega t}\left(\left({1\over C} - L\omega^2\right) - i\left(R\omega\right)\right)\over \left({1\over C} - L\omega^2\right)^2 + \left(R\omega\right)^2}\right\\}\\\
&= Re\left\\{{\left(cos(\omega t) + isin(\omega t)\right)\left(\left({1\over C} - L\omega^2\right) - i\left(R\omega\right)\right)\over \left({1\over C} - L\omega^2\right)^2 + \left(R\omega\right)^2}\right\\}\\\
&= {\left({1\over C} - L\omega^2\right)cos(\omega t) + R\omega sin(\omega t)\over \left({1\over C} - L\omega^2\right)^2 + \left(R\omega\right)^2}\\\
&= {\sqrt{\left({1\over C} - L\omega^2\right)^2 + \left(R\omega\right)^2}\left(cos\left(\omega t - \arctan\left({R\omega\over{1\over C}- L\omega^2}\right)\right)\right)\over \left({1\over C} - L\omega^2\right)^2 + \left(R\omega\right)^2}
\end{align}
$$
For the case where $$$I(t)$$$ and $$$V(t)$$$ are in phase, note that:
$$
\begin{align}
V(t) &= V_0sin(\omega t)\\\
&= V_0cos\left(\omega t - \pi\over2\right)\\\
\end{align}
$$
Therefore:
$$
\begin{align}
{\pi\over2} &= \arctan\left({R\omega\over{1\over C}- L\omega^2}\right)\\\
tan\left({\pi\over2}\right) &= {R\omega\over{1\over C}- L\omega^2}\\\
\infty &= {R\omega\over{1\over C}- L\omega^2}\\\
0 &= {1\over C} - L\omega^2\\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{{1\over C} = L\omega^2}
$$

######17c)
$$
\begin{align}
\omega &= 100 \text{rad/s}\\\
Amp\left\\{I(t)\right\\}_{max} &= 5 A\\\
\phi &= 0\\\
I(t) &= 5sin(\omega t)\\\
\end{align}
$$

######17d)




