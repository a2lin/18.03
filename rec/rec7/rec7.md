$$$\require{cancel}$$$

# 18.03
###Recitation 5
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/recitations/MIT18_03S10_rec_07.pdf)
######1a)
$$
\begin{align}
x = cos(\omega t)\\\
{d^2\over dt^2}x(t) + \omega^2x(t) &= 0\\\
{d^2\over dt^2}cos(\omega t) + \omega^2cos(\omega t) &= 0\\\
-\omega^2 cos(\omega t) + \omega^2cos(\omega t) &= 0 \\\
0 &= 0 \quad \checkmark\\\
\end{align}
$$
######1b)
$$
\begin{align}
x = sin(\omega t)\\\
{d^2\over dt^2}x(t) + \omega^2x(t) &= 0 \\\
{d^2\over dt^2}sin(\omega t) + \omega^2sin(\omega t) &= 0 \\\
-\omega^2sin(\omega t) + \omega^2 sin(\omega t) &= 0\\\
0 &= 0 \quad \checkmark\\\
\end{align}
$$

######2)
$$
\begin{align}
x &= A cos(\omega t - \phi)\\\
{d^2\over dt^2}x(t) + \omega^2x(t) &= 0 \\\
{d^2\over dt^2}Acos(\omega t - \phi) + \omega^2Acos(\omega t - \phi) &= 0\\\
-A\omega^2cos(\omega t - \phi) + \omega^2Acos(\omega t - \phi) &= 0\\\
0 &= 0 \quad \checkmark\\\
\end{align}
$$

######3)
The uniqueness theorem only applies to first order equations. The given equation is second order, and thus uniqueness doesn't apply.

######4)
$$
\begin{align}
x(0) &= x_0 \\\
\dot{x}(0) &= \dot{x}_0 \\\
\ddot{x} + \omega^2x &= 0\\\
\end{align}
$$
The characteristic equation here is:
$$r^2 + \omega^2 = 0$$

with roots $$$\pm i\omega$$$.  
We know that if the characteristic equation has complex root $$$a+bi$$$, $$$e^{at}cos(bt)$$$ and $$$e^{at}sin(bt)$$$ are solutions, and therefore we can write:

$$
C_1e^{at}cos(\omega t) + C_2e^{at}sin(\omega t) = x(t)
$$

Using the initial condition $$$x(0) = x_0$$$:

$$
\begin{align}
C_1e^{0}cos(0) + \cancel{C_2e^{0}sin(0)} &= x(0) \\\
C_1 &= x_0
\end{align}
$$

Using the initial condition $$$\dot{x}(0) = \dot{x}_0$$$:

$$
\begin{align}
{d\over dt}\left(C_1e^{at}cos(\omega t) + C_2e^{at}sin(\omega t)\right) &= {d\over dt}x(t)\\\
-C_1e^{at}\omega sin(\omega t) + C_2e^{at}\omega cos(\omega t) &= {d\over dt}x(t)\\\
\cancel{-C_1e^{0}\omega sin(0)} + C_2e^{0}\omega cos(0) &= {d\over dt}x(0) \\\
C_2\omega &= \dot{x}(0)\\\
C_2 &= {\dot{x}(0)\over \omega}\\\
\end{align}
$$

Therefore we can write the solution as:
$$
x(t) = \bbox[5px, border:2px solid black]{x_0e^{at}cos(\omega t) + {\dot{x}(0)\over \omega}e^{at}sin(\omega t)}
$$
And there is only one solution.

######5)
Assuming $$$e^{rt}$$$ is a solution:

$$
\begin{align}
\ddot{x} + kx &= 0 \\\
{d^2\over dt^2}x(t) + kx(t) &= 0 \\\
{d^2\over dt^2}e^{rt} + ke^{rt} &= 0 \\\
r^2e^{rt} + ke^{rt} &= 0 \\\
r^2 &= -k
\end{align}
$$

$$\therefore \bbox[5px, border:2px solid black]{r = i\sqrt{k}}$$

######6)