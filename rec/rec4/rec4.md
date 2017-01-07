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
