$$$\require{cancel}$$$

# 18.03
###Pset 3a
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/assignments/MIT18_03S10_ps3a.pdf)
#####Section 1
===
######1E-1a)

![Image](a_p1i.png =400x300)

######1E-1b)
![Image](a_p1ii.png =400x300)

######1E-1c)
![Image](a_p1iii.png =400x300)

######1E-1d)
![Image](a_p1iv.png =400x300)

######2ai)
$$
\begin{align}
{d\over dt} + 2x(t) &= 1 \\\
{d\over dt} &= 1 - 2x(t)\\\
\int {1\over 1-2x}\ dx &= \int 1\ dt \\\
-{1\over 2} ln(1-2x(t)) &= t + C_0\\\
ln(1-2x(t)) &= -2t + C_0\\\
1 - 2x(t) &= Ce^{-2t} \\\
-2x(t) &= Ce^{-2t}-1 \\\
x(t) &= \bbox[5px, border:2px solid black]{Ce^{-2t}+{1\over2}}\\\
\end{align}
$$

######2aii)
$$
\begin{align}
{d\over dt}x(t) + 2x(t) &= 1 \\\
{d\over dt}x(t)e^{2t} + 2x(t)e^{2t} &= e^{2t} \\\
{d\over dt}\left(x(t)e^{2t}\right) &= e^{2t} \\\
\int {d\over dt}\left(x(t)e^{2t}\right)\ dt &= \int e^{2t}\ dt \\\
x(t)e^{2t} &= {1\over 2}e^{2t} + C \\\
x(t) &= \bbox[5px, border:2px solid black]{{1\over 2} + Ce^{-2t}}\\\
\end{align}
$$

######2aiii)
Regard RHS as $$$e^{0t}$$$, and assume solution takes the form $$$Ae^{0t}$$$:  
$$
\begin{align}
{d\over dt}x(t) + 2x(t) &= e^{0t}\\\
{d\over dt}Ae^{0t} + 2Ae^{0t} &= e^{0t}\\\
0 + 2A &= 1 \\\
A &= {1\over 2} \\\
\end{align}
$$
$$\therefore x_p = {1\over 2}$$
Because we know that the solution for an equation of the form
$$${d\over dt}x(t) + kx(t) = 0$$$ is $$$x(t) = Ce^{-kt}$$$, we can add in a transient, and write the solution as:
$$
\bbox[5px, border:2px solid black]{{1\over 2} + Ce^{-2t}}
$$

