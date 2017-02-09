$$$\require{cancel}$$$

# 18.03
###Rec 9
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/recitations/MIT18_03S10_rec_09.pdf)

######1)
$$
\begin{align}
\ddot{x} + 4x &= sin(3t)\\\
{d\over dt}\left(Asin(3t)\right) + 4Asin(3t) &= sin(3t)\\\
-9Asin(3t) + 4Asin(3t) &= sin(3t)\\\
-5Asin(3t) &= sin(3t)\\\
A &= \bbox[5px, border:2px solid black]{{-1\over5}}\\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{x_p = {-1\over5}sin(3t)}
$$
General solution:
$$
\begin{align}
\ddot{x}+4x &= 0\\\
r^2+4r &= 0 \\\
r(r+4) &= 0 \\\
r=0,&\ r=4 \\\
C_1 + C_2e^{4t} &= 0 \\\
\end{align}
$$
$$\therefore \bbox[5px, border:2px solid black]{x(t) = {-1\over5}sin(3t) + C_1 + C_2e^{4t}}$$

######2)
$$
\begin{align}
\ddot{x}+4x &= cos(\omega t) \\\
\ddot{Acos(\omega t)} + 4Acos(\omega t) &= cos(\omega t)\\\
-\omega^2Acos(\omega t) + 4Acos(\omega t) - cos(\omega t) &= 0\\\
cos(\omega t)\left(-\omega^2A + 4A - 1\right) &= 0\\\
-\omega^2A + 4A - 1 &= 0\\\
A\left(4-\omega^2\right) &= 1\\\
A &= \bbox[5px, border:2px solid black]{{1\over 4-\omega^2}}\\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{{1\over 4-\omega^2}cos(\omega t)}
$$
![image](2-1w0.png =300x300)
![image](2-1w1.png =300x300)
![image](2-1w3.png =300x300)
![image](2-2res.png =300x300)   
Seems like resonance is achieved at w=2?

######3)



