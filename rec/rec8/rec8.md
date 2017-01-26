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

######4)
$$
\begin{align}
x(t_0) &= Ae^{-at_0}cos(\omega t_0)\\\
x(t_1) &= Ae^{-at_1}cos(\omega t_1)\\\
{x(t_0)\over x(t_1)} &= {e^{-at_0}cos(\omega t_0)\over e^{-at_1}cos(\omega t_1)}\\\
{x(t_0)\over x(t_1)} &= e^{-a(t_0-t_1)}\\\
{x(t_0)\over x(t_1)} &= \bbox[5px, border:2px solid black]{e^{-a{2\pi\over \omega}}}\\\
\end{align}
$$
Using the facts that because $$$t_0$$$ and $$$t_1$$$ are maxima, their cosines should both occur at the cosine peak $$${2\pi\over \omega}$$$, and therefore the cosines are equal and the $$$t_x$$$ are separated by $$${2\pi\over \omega}$$$.

Therefore a method of finding $$$a$$$ is to find two consecutive maxima and calculate $$$\bbox[5px, border:2px solid black]{-ln\left({x(t_0)\omega\over x(t_1)2\pi}\right)}$$$.

######5a)
$$
\begin{align}
\ddot{x} + b\dot{x} + x &= 0 \\\
r^2 + br + 1 &= 0 \\\
{-b \pm \sqrt{b^2-4}\over 2} &= r \\\
b^2-4 &= 0\\\
b &= \pm 2\\\
\end{align}
$$
Thus this equation exhibits critical damping if $$$b$$$ is $$$\bbox[5px, border:2px solid black]{\pm 2}$$$.
$$
\begin{align}
r^2 + 2r + 1 &= 0 \\\
(r+1)^2 &= 0 \\\
r &= -1\\\
C_1e^{-1t} + C_2e^{r_2t} &= x(t) \\\
\end{align}
$$
To get the second root we guess $$$te^{-t}$$$ for no apparent reason.
$$
\begin{align}
{d\over dt}\left(te^{-t}\right) &= \left[e^{-t} - te^{-t}\right]\\\
{d^2\over dt^2}\left(te^{-t}\right) &= {d\over dt} \left[e^{-t}-te^{-t}\right]\\\
&= \left[-e^{-t}-\left[e^{-t}-te^{-t}\right]\right]\\\
\end{align}
$$
Substituting back in:
$$
\begin{align}
\left[-e^{-t}-\left[e^{-t}-te^{-t}\right]\right] + 2 \left[e^{-t}-te^{-t}\right] + te^{-t}\\\
-e^{-t}-e^{-t}+te^{-t}+2e^{-t}-2te^{-t} + te^{-t} &= 0\\\
-2e^{-t}+2e^{-t}-2te^{-t}+2te^{-t} &= 0 \\\
0 &= 0 \quad \checkmark\\\
\end{align}
$$
So we can use $$$te^{-t}$$$ as the second solution.
$$\therefore x(t) = C_1e^{-t} + C_2te^{-t}$$

######5b)
$$
\begin{align}
x_1(0) &= C_1e^{-t} + C_2te^{-t}\\\
1 &= C_1e^{-0} +C_20e^{-0}\\\
1 &= C_1\\\
\\\
\dot{x_1}(0) &= {d\over dt}\left(C_1e^{-t} + C_2te^{-t}\right)\\\
\dot{x_1}(0) &= -C_1e^{-t} + C_2\left[e^{-t}-te^{-t}\right]\\\
0 &= -C_1e^{0} + C_2\left[e^{0}-0e^{0}\right]\\\
0 &= -C_1 + C_2\left[1 - 0\right]\\\
0 &= -C_1 + C_2\\\
C_1 &= C_2\\\
1 &= C_1 = C_2\\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{x_1(t) = e^{-t}+te^{-t}}
$$

######5c)
$$
\begin{align}
x_2(0) &= C_1e^{-t} + C_2te^{-t}\\\
2 &= C_1e^{-0} + C_20e^{-0}\\\
2 &= C_1\\\
\\\
\dot{x_1}(0) &= {d\over dt}\left(C_1e^{-t} + C_2te^{-t}\right)\\\
\dot{x_1}(0) &= -C_1e^{-t} + C_2\left[e^{-t}-te^{-t}\right]\\\
3 &= -C_1e^{0} + C_2\left[e^{0}-0e^{0}\right]\\\
3 &= -C_1 + C_2\left[1 - 0\right]\\\
3 &= -C_1 + C_2\\\
3+C_1 &= C_2\\\
C_1 &= 2\\\
C_2 &= 5
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{x_2(t) = 2e^{-t}+5te^{-t}}
$$