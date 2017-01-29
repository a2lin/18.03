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
$$
y(x) = C_1 + C_2e^{-10x}
$$
The characteristic polynomial from the structure of the above equation is:
$$
\begin{align}
&r(r+10)
&r^2+10r
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{y''(x) + 10y'(x) = 0}
$$

######2.1 44)
$$
y(x) = C_1e^{10x} + C_2e^{-10x}
$$
The characteristic polynomial from the structure of the above equation is:
$$
\begin{align}
&(r-10)(r+10)\\\
&r^2-100
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{y''(x)-100y(x)}
$$

######2.1 47)
$$
y(x) = c_1 + c_2x
$$

We just need any equation satisfying $$$ay'' + by' + cy = 0$$$:
$$
\begin{align}
y(x) &= c_1 + c_2x \\\
y'(x) &= c_2 \\\
y''(x) &= 0 \\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{1(y'') + 0y' + 0y = 0}
$$