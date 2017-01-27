$$$\require{cancel}$$$

# 18.03
###Pset 3 part 2
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/assignments/MIT18_03S10_pset_03_II.pdf)

######2C-1a)
$$
\begin{align}
y'' - 3y' + 2y &= 0 \\\
r^2-3r+2 &= 0 \\\
(r-2)(r-1)\\\
r_1 &= 2\\\
r_2 &= 1\\\
\end{align}
$$
$$
\bbox[5px, border:2px solid black]{C_1e^{2t} + C_2e^{t}}
$$
######2C-1b)
$$
\begin{align}
y'' + 2y' - 3y &= 0 \\\
r^2 + 2r - 3 &= 0\\\
(r+3)(r-1)\\\
r_1 &= -3 \\\
r_2 &= 1 \\\
\end{align}
$$
$$
\bbox[5px, border:2px solid black]{C_1e^{-3t}+C_2e^{t}}
$$
Using initial conditions $$$y(0) = 1$$$ and $$$y'(0) = -1$$$:
$$
\begin{align}
y(0) &= C_1e^{-3(0)} + C_2e^{0}\\\
1 &= C_1 + C_2\\\
\\\
y'(t) &= -3C_1e^{-3t}+C_2e^{t}\\\
y'(0) &= -3C_1e^{0} + C_2e^{0}\\\
-1 &= -3C_1 + C_2\\\
3C_1 - 1 &= C_2\\\
\\\
1 &= C_1 + 3C_1 - 1\\\
2 &= 4C_1\\\
{1\over 2} &= C_1\\\
{1\over 2} &= C_2\\\
\end{align}
$$
$$\therefore y(t) = \bbox[5px, border:2px solid black]{{1\over 2}e^{-3t} + {1\over 2}e^{t}}$$

######2.1 43)
