$$$\require{cancel}$$$

# 18.03
###Recitation 8
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/recitations/MIT18_03S10_rec_08.pdf)

######1a)
$$
\begin{align}
\ddot{x} + \omega^2x &= 0 \\\
\bbox[5px, border:2px solid black]{r^2 + \omega^2} &= 0\\\
r^2 &= -\omega^2\\\
r &= \bbox[5px, border:2px solid black]{\pm i\omega}
\end{align}
$$
Exponential solutions:
$$
\bbox[5px, border:2px solid black]{
C_1e^{i\omega t} + C_2e^{-i\omega t}
}
$$
This results in:
$$
\begin{align}
&C_1\left[cos(\omega t) + isin(\omega t)\right] + C_2\left[cos(-\omega t) + i sin(-\omega t)\right] \\\
&C_1\left[cos(\omega t) + isin(\omega t)\right] + C_2\left[cos(\omega t) - i sin(\omega t)\right]\\\
&K_1=C_1+C_2\\\
&K_2 = C_1-C_2\\\
&K_1cos(\omega t) + iK_2sin(\omega t)\\\
\end{align}
$$
So the real part is $$$\bbox[5px, border:2px solid black]{K_1cos(\omega t)}$$$ and the imaginary part is $$$\bbox[5px, border:2px solid black]{K_2sin(\omega t)}$$$.

######2a)
$$
\begin{align}
mr^2 + br + k &= 0 \\\
{-b \pm \sqrt{b^2 - 4mk}\over 2m} &= {-1\over2} + 3i\\\
\\\
{-1\over2} &= {-b\over 2m} \\\
b &= m\\\
\\\
{\sqrt{b^2-4mk}\over 2m} &= 3i \\\
{b^2-4mk} &= -36m^2 \\\
m^2 - 4mk &= -36m^2 \\\
-4mk &= -37m^2 \\\
k &= {37\over 4}m \\\
\end{align}
$$

######2b)
Since we know that $$$e^{-{t\over2}}cos(3t)$$$ is a solution, and that solutions for roots $$$a\pm bi$$$ come in pairs of $$$e^{at}cos(bt)$$$, $$$e^{at}sin(bt)$$$, we can say that another solution is:
$$
\bbox[5px, border:2px solid black]{e^{-{t\over2}}sin(3t)}
$$

######2c)
![Image](2ci.png =300x300)  
![Image](2cii.png =300x300)

The second graph (the real part) is the first graph (combined graph)'s x axis (real axis)'s movement over time.

######2d)
We can add the two exponential solutions that we have to arrive at:
$$
x(t) = \bbox[5px, border:2px solid black]{C_1e^{-{t\over2}}cos(3t) + C_2e^{-{t\over2}}sin(3t)}
$$

######3)
$$
\begin{align}
x(t) &= Ae^{-at}cos(\omega t)\\\
x'(t) &= A\left[\left(e^{-at}\right)'cos(\omega t)+e^{-at}\left(cos(\omega t\right)'\right]\\\
&= A\left[-ae^{-at}cos(\omega t) + e^{-at}\left(-\omega sin(\omega t)\right)\right]\\\
&= Ae^{-at}\left[-acos(\omega t) -\omega sin(\omega t)\right]\\\
\end{align}
$$
To find maxima, we set $$$x'(t) = 0$$$.
$$
\begin{align}
x'(t) &= Ae^{-at}\left[-acos(\omega t) -\omega sin(\omega t)\right]\\\
0 &= Ae^{-at}\left[-acos(\omega t)-\omega sin(\omega t)\right]\\\
&= -acos(\omega t)-\omega sin(\omega t)\\\
acos(\omega t) &= -\omega sin(\omega t)\\\
{a\over -\omega} &= tan(\omega t)\\\
\end{align}
$$
Since $$$tan(\omega t)$$$ has a period of $$$\pi\over \omega$$$, we can expect an extrema to occur every $$$\pi \over \omega$$$. However, since we want _maxima_, we take every other extrema, so $$$\bbox[5px, border:2px solid black]{2\pi \over \omega}$$$.
Since the LHS is does not depend on $$$t$$$, it does not differ from one pair of maxima to the next.