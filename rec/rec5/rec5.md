$$$\require{cancel}$$$

# 18.03
###Recitation 5
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/recitations/MIT18_03S10_rec_05.pdf)
#####Section 1
===
Polar coordinates: $$$(1, \sqrt3i)$$$  

| n | $$$a+bi$$$ | $$$Ae^{i\theta}$$$ | 
|---|----------|-----------|
|-4|$$${1\over 16}\left(-{\sqrt3\over2} + {1\over2}i\right)$$$|$$${1\over 16}e^{{-4\pi \over3}i}$$$|
|-3|$$${1\over 8}\left(-1 + 0i\right)$$$|$$${1\over 8}e^{-\pi i}$$$|
|-2|$$${1\over 4}\left(-{\sqrt3\over2} - {1\over2}i\right)$$$|$$${1\over 4}e^{{-2\pi \over 3}i}$$$|
|-1|$$${1\over 2}\left({\sqrt3\over2} - {1\over2}i\right)$$$|$$${1\over 2}e^{{-\pi \over 3}i}$$$|
|0|$$$1+0i$$$|$$$1$$$|
|1|$$$2\left({\sqrt3\over2} + {1\over2}i\right)$$$|$$$2e^{{\pi\over3}i}$$$|
|2|$$$4\left(-{\sqrt3\over2} + {1\over2}i\right)$$$|$$$4e^{{2\pi\over3}i}$$$|
|3|$$$8\left(-1 + 0i\right)$$$|$$$8e^{\pi i}$$$|
|4|$$$16\left(-{\sqrt3\over2} - {1\over2}i\right)$$$|$$$16e^{{4\pi\over3}i}$$$|

![image](p1.png =400x300)
#####Section 2
===
From (1) we know that one possible expression is:
$$2e^{i{\pi\over3}}$$
Rewriting this in the form $$$e^{a+bi}$$$:
$$e^{ln(2)}e^{i{\pi\over3}}$$
$$e^{ln(2)+i{\pi\over3}}$$
$$\therefore a=ln(2),\ b={\pi\over3}$$
Fixing b to be as small as possible:
$$e^{ln(2) + i{\pi\over3}}$$

It's clear that solving for $$$\left(e^{ln(2) + i{\pi\over3}}\right)^{n}$$$ where $$$n$$$ is $$$\\{-4\...4\\}$$$ will result in the same answers as in (1).
#####Section 3
===
######a)
Expression:
$$\cos(2t) + \sin(2t)$$
Writing in the form of $$$A\cos(\omega t - \phi)$$$:
$$A = \sqrt{(1^2+1^2)} = \sqrt2$$
$$\phi = \arctan({1\over2}) = {\pi\over4}$$
$$\therefore \cos(2t) + \sin(2t) = \bbox[5px, border:2px solid black]{\sqrt2\cos\left(2t-{\pi\over4}\right)}$$
######b)
Expression:
$$\cos(\pi t) - \sqrt 3 \sin(\pi t)$$
Writing in the form of $$$A\cos(\omega t - \phi)$$$:
$$A = \sqrt{1^2 + {\sqrt3}^2} = 2$$
$$\phi = -\arctan\left({\sqrt3\over1}\right) = -{\pi\over3}$$
$$\therefore \cos(\pi t) - \sqrt 3 \sin(\pi t) = \bbox[5px, border:2px solid black]{2\cos\left(\pi t - {\pi\over3}\right)}$$
######c)
Expression:
$$Re\left\\{{e^{it}\over 2 + 2i}\right\\}$$
Writing in the form of $$$A\cos(\omega t - \phi)$$$:
$$
\begin{align}
Re\left\\{{e^{it}\over 2 + 2i}\right\\} &= Re\left\\{{e^{it}\over 2\sqrt2e^{{\pi\over4}i}}\right\\}\\\
&= Re\left\\{2\sqrt 2 e^{it}e^{-{\pi\over4}i}\right\\}\\\
&= Re\left\\{2\sqrt 2 e^{\left(t-{\pi\over4}\right)i}\right\\}\\\
&= \bbox[5px, border:2px solid black]{2\sqrt 2 \cos\left(t-{\pi\over4}\right)}\\\
\end{align}
$$
#####Section 4
===
######a)
$$
\begin{align}
{d\over dt}x(t) + 2x(t) &= e^{t}\\\
{d\over dt}x(t)e^{2t} + 2x(t)e^{2t} &= e^{3t}\\\
{d\over dt}\left(x(t)e^{2t}\right) &= e^{3t}\\\
\int {d\over dt}\left(x(t)e^{2t}\right)\ dt &= \int e^{3t}\ dt\\\
x(t)e^{2t} &= \int e^{3t}\ dt\\\
x(t)e^{2t} &= {1\over 3} e^{3t} + C\\\
x(t) &= \bbox[5px, border:2px solid black]{{1\over 3}e^{t} + Ce^{-2t}}
\end{align}
$$
######b)
$$
\begin{align}
{d\over dt}z(t) + 2z(t) &= e^{2it}\\\
e^{2t}{d\over dt}z(t) + 2e^{2t}z(t) &= e^{2it}e^{t}\\\
\int {d\over dt}\left(e^{2t}z(t)\right)\ dt &= \int e^{2it}e^{2t}\ dt\\\
e^{2t}z(t) &= \int e^{t\left(2+2i\right)}\ dt\\\
e^{2t}z(t) &= {1\over 2+2i}e^{t\left(2+2i\right)} + C\\\
z(t) &= {1\over 2+2i}e^{t\left(2+2i\right)-2t} + Ce^{-2t}\\\
z(t) &= \bbox[5px, border:2px solid black]{{1\over 2+2i}e^{2it} + Ce^{-2t}}\\\
\end{align}
$$