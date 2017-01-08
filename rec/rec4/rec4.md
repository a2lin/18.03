$$$\require{cancel}$$$

# 18.03
###Recitation 4
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/recitations/MIT18_03S10_rec_04.pdf)
#####Section 1
===
######a)
If $$$k$$$ is the proportional constant, $$$y(t)$$$ is the height of the ocean, and $$$x(t)$$$ is the height of the bay, we can represent the fact that the change is proportional to the difference between ocean and bay with the following equation:
$${d\over dt}x(t) = k(y(t)-x(t))$$
Written in standard form:
$${d\over dt}x(t) = ky(t)-kx(t)$$
$$\bbox[5px, border:2px solid black]{\underbrace{{d\over dt}x(t) + k\underbrace{x(t)}\_{output}}\_{system} = k\underbrace{y(t)}_{input}}$$
######b)
If we are modeling the tide using 
$$y(t) = cos(\omega t)$$
and expecting it to have a period of $$$4\pi$$$, which is double the normal period:
$$\bbox[5px, border:2px solid black]{\omega={1\over 2}}$$
######c)
$$
\begin{align}
{d\over dt}x(t) + kx(t) &= ky(t) \\\
{d\over dt}x(t)e^{kt} + kx(t)e^{kt} &= ky(t)e^{kt}\\\
{d\over dt}\left(x(t)e^{kt}\right) &= ky(t)e^{kt} \\\
\int {d\over dt}\left(x(t)e^{kt}\right)\ dt &= \int ky(t)e^{kt}\ dt\\\
x(t)e^{kt} &= k\left({1\over k^2+\omega^2}e^{kt}\left(k\cos(\omega t)+ \omega\sin(\omega t)\right)+C\right)\\\
x(t) &= \bbox[5px, border:2px solid black]{{k\over k^2+\omega^2}\left(k\cos(\omega t)+ \omega\sin(\omega t)\right)+{C\over e^{k t}}}
\end{align}
$$
######d)
Assuming $$$x(t)=a\cos(\omega t) + b\sin(\omega t)$$$:
$$
\begin{align}
{d\over dt}x(t) &= {d\over dt}\left(a\cos(\omega t) + b\sin(\omega t)\right)\\\
&= -a\omega\sin(\omega t) + b\omega\cos(\omega t)
\end{align}
$$
Plugging this back into the original diffeq and substituting $$$y(t)=\cos(\omega t)$$$:
$$
\begin{align}
ky(t) &= {d\over dt} x(t)+kx(t)\\\
k\cos(\omega t) &= -a\omega\sin(\omega t) + b\omega\cos(\omega t) + k\left(a\cos(\omega t) + b\sin(\omega t)\right)\\\
&= (ka+b\omega)\cos(\omega t) + (kb-\omega a)sin(\omega t)\\\
\end{align}
$$
We can see that:  
$$ka+b\omega = k$$
$$kb-\omega a = 0$$
Solving this system of equations:
$$
\begin{align}  
kb - \omega a &= 0\\\
kb &= \omega a\\\
b &= {\omega a\over k}\\\
\end{align}
$$
Plugging this b into the other equation:  
$$
\begin{align}
ka + b\omega &= k\\\
ka + {\omega a\over k}\omega &= k\\\
ka + {\omega^2a\over k} &= k\\\
a\left({k+\omega^2\over k}\right) &= k\\\
a = {k^2\over k+\omega^2}\\\
\end{align}
$$
Plugging this back into the first equation to get an expression for b:
$$
\begin{align}
b &= {\omega a\over k}\\\
b &= {\omega{k^2\over k + \omega^2}\over k}\\\
b &= \omega{k\over k+\omega^2}
\end{align}
$$
$$\therefore \bbox[5px, border:2px solid black]{a = {k^2\over k+\omega^2},\ b=\omega{k\over k+\omega^2}}$$
#####Section 2
===
######a)
$$
\begin{align}
{d\over dx}y(x) &= x - 2y(x)\\\
{d\over dx}y(x) + 2y(x) &= x\\\
{d\over dx}y(x) e^{2x} + 2y(x)e^{2x} &= xe^{2x}\\\
{d\over dx}\left(y(x)e^{2x}\right) &= xe^{2x}\\\
\int{d\over dx}\left(y(x)e^{2x}\right)\ dx &= \int xe^{2x}\ dx\\\
y(x)e^{2x} &= {x\over 2}e^{2x} - \int{1\over 2}e^{2x}\ dx + C\\\
y(x)e^{2x} &= {x\over 2}e^{2x} - {1\over 4}e^{2x} + C \\\
y(x) &= \bbox[5px, border:2px solid black]{{x\over 2} - {1\over 4} + Ce^{-2x}}\\\
\end{align}
$$
######b)
Evidently the straight line is at 
$$
y(x) = \bbox[5px, border:2px solid black]{{x\over 2} - {1\over 4}}
$$
######c)
Given the initial condition $$$y(0) = 1$$$:  
$$
\begin{align}
y(x) &= {x\over 2} - {1\over 4} + Ce^{-2x}\\\
y(0) &= {0\over 2} - {1\over 4} + Ce^{0}\\\
0 &= -{1\over 4} + C\\\
C &= {5\over 4}
\end{align}
$$
$$\therefore y_p(x) = \bbox[5px, border:2px solid black]{{x\over 2} - {1\over 4} + {5\over 4}e^{-2x}}$$
#####Section 3
===
$$
\begin{align}
x^2{d\over dx}y(x) + 2xy(x) &= \sin(2x)\\\
{d\over dx}\left(x^2y(x)\right) &= \sin(2x)\\\
\int {d\over dx}\left(x^2y(x)\right)\ dx &= \int \sin(2x)\ dx\\\
x^2y(x) &= -{1\over 2}\cos(2x)+C\\\
y(x) &= {-{1\over 2}\cos(2x)\over x^2} + Cx^{-2}\\\
y(x) &= \bbox[5px, border:2px solid black]{{-\cos(2x)\over 2x^2} + Cx^{-2}}\\\
\end{align}
$$