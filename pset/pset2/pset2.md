$$$\require{cancel}$$$
# 18.03
### Pset 1
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/assignments/MIT18_03S10_ps2.pdf)
###Table of Contents:
[Part 1](#part1)  
####[Part I.](id:part1)
===
#####Section 2
===
######2E-1a)
$$-1 + i$$
$$\begin{split}r=\sqrt{(-1)^2 + 1^2}\end{split},\quad\begin{split}tan(\theta)={1\over-1}\end{split}$$
$$\begin{split}r = \sqrt{2}\end{split} ,\quad\begin{split}\theta=-{\pi\over 4}\end{split}$$
$$\sqrt {2}\left(\cos\left(-{\pi\over4}\right)+i\sin\left(-{\pi\over 4}\right)\right)$$
$$\bbox[5px, border:2px solid black]{\sqrt2e^{{-{\pi\over 4}}i}}$$
######2E-1b)
$$\sqrt{3} - i$$
$$\begin{split}r=\sqrt{(\sqrt{3})^2 + (-1)^2}\end{split},\quad\begin{split}tan(\theta)={-1\over\sqrt{3}}\end{split}$$
$$\begin{split}r = 2\end{split} ,\quad\begin{split}\theta=-{\pi\over 6}\end{split}$$
$$2\left(\cos\left(-{\pi\over6}\right)+i\sin\left(-{\pi\over 6}\right)\right)$$
$$\bbox[5px, border:2px solid black]{2e^{-{\pi\over 6}i}}$$
######2E-2)
$${1-i\over 1+i}$$
Rectangular:
$${1-i\over 1+i} = {(1-i)\cdot(1-i)\over (1+i)\cdot(1-i)}$$
$${1-i\over 1+i} = -2i\over 2$$
$$\bbox[5px, border:2px solid black]{{1-i\over 1+i} = -i}$$
Polar:
$$1-i \rightarrow \sqrt2 \left(\cos\left(-{\pi\over 4}\right)+i\sin\left(-{\pi\over 4}\right)\right) \rightarrow \sqrt2e^{{-{\pi\over 4}i}}$$
$$1+i \rightarrow \sqrt2 \left(\cos\left({\pi\over 4}\right)+i\sin\left({\pi\over 4}\right)\right)\rightarrow \sqrt2e^{{\pi\over 4}i}$$
$${1-i\over 1+i} = {\cancel{\sqrt2}e^{-{\pi\over 4}i} \over \cancel{\sqrt2}e^{{\pi\over 4}i}}$$
$${1-i\over 1+i} = e^{-{\pi\over 4}i}e^{-{\pi\over 4}i}$$
$${1-i\over 1+i} = e^{-{\pi\over 2}i}$$
$${1-i\over 1+i} = \cos(-{\pi\over2}) + i \sin(-{\pi\over2})$$
$${1-i\over 1+i} = 0 + i (-1)$$
$$\bbox[5px, border:2px solid black]{{1-i\over 1+i} = -i}$$
Comparing the answers from the rectangular method and the polar method we find that they are the same:
$$-i=-i\quad\checkmark$$

#####Section 1
===
######1.5 #1)
$${dy\over dx} + y(x) = 2,\ y(0) = 0$$
This is actually separable, and can be solved with:
$${dy\over dx} = 2-y(x)$$
$$\int {1\over 2 - y(x)}\ dy = \int dx$$
$$ln(2-y(x)) = t + C$$
$$2 - y(x) = e^{t+C_0}$$
$$y(x) = Ce^{x}-2$$
Using the initial condition $$$y(0) = 0$$$:
$$y(0) = Ce^{0}-2$$
$$0 = C - 2$$
$$C=2$$
$$\bbox[5px, border:2px solid black]{y(x) = 2e^{x}-2}$$
######1.5 #2)
$${dy\over dx}-2y(x)=3e^{2x}$$
This is unseparable. Proceed by method of integrating factors.
$${d\over dx}a(x) = -2a(x)$$
Separate variables:
$$\int {1\over a(x)} da(x) = \int -2\ dx$$
$$ln(a(x)) = -2x + C_0$$
$$a(x) = Ce^{-2x}$$
Multiplying this back into the original equation:
$${dy\over dx}e^{-2x} - 2y(x)e^{-2x} = 3e^{2x}e^{-2x}$$
$${d\over dx}\left(y(x)e^{-2x}\right)=3$$
$$\int{d\over dx}\left(y(x)e^{-2x}\right)\ dx = \int 3 \ dx$$
$$y(x)e^{-2x} = 3x$$
$$\bbox[5px, border:2px solid black]{y(x) = 3xe^{2x}}$$
######1.5 #5)
$$x{dy\over dx} + 2y(x) = 3x, y(1) = 5$$
$${dy\over dx} + {2\over x}y(x) = 3$$
This equation is not separable. We can write this in standard form though, so proceed by method of integrating factors.
$${2\over x}a(x) = {da(x)\over dx}$$
Separate variables:
$$\int {1\over a(x)}\ da(x) = \int {2\over x}\ dx$$
$$ln(a(x)) = 2ln(x) + C$$
$$a(x) = e^{2ln(x)+C}$$
$$a(x) = Cx^2$$
Substitute back into the original equation:
$${dy\over dx}x^2 + {2\over x}y(x)x^2 = 3x^2$$
$${dy\over dx}x^2 + 2xy(x) = 3x^2$$
$${d\over dx}\left(y(x)x^2\right) = 3x^2$$
$$\int {d\over dx}\left(y(x)x^2\right)\ dx = \int 3x^2\ dx$$
$$y(x)x^2 = x^3 + C$$
$$y(x) = {x^3 + C \over x^2}$$
$$y(x) = x + Cx^{-2}$$
Using the initial condition of $$$y(1)=5$$$:
$$y(1) = (1) + C(1)^{-2}$$
$$5 = 1 + C$$
$$C = 4$$
$$\bbox[5px, border:2px solid black]{\therefore y(x) = x + 4x^{-2}}$$

