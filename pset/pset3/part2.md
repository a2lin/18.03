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

######2.1 #43)
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

######2.1 #44)
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

######2.1 #47)
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

######2.3 #1)
$$
\begin{align}
y'' - 4y &= 0 \\\
r^2 - 4 &= 0 \\\
(r+2)(r-2) &= 0 \\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{C_1e^{-2x} + C_2e^{2x} = 0} 
$$

######2.3 #2)
$$
\begin{align}
2y'' - 3y' &= 0 \\\
2r^2 - 3r &= 0 \\\
r(2r-3) &= 0 \\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{C_1 + C_2e^{{3\over2}x}}
$$

######2.3 #7)
$$
\begin{align}
4y'' - 12y' + 9y &= 0 \\\
4r^2 - 12r + 9 &= 0 \\\
(2r - 3)(2r - 3) &= 0 \\\
\end{align}
$$
The singular root in this case is $$${3\over2}$$$, so we can write:
$$
\therefore 
\bbox[5px, border:2px solid black]{
C_1e^{{3\over2}x} + C_2xe^{{3\over2}x}
}
$$

######2.3 #15)
$$
\begin{align}
y^{(4)}-8y''+16y &= 0 \\\
r^4 - 8r^2 + 16 &= 0 \\\
(r^2-4)(r^2-4) &= 0 \\\
(r+2)(r-2)(r+2)(r-2) &= 0 \\\
\end{align}
$$
There are two roots here, $$$2$$$ and $$$-2$$$, but we need a total of 4, so we can write down:
$$
\bbox[5px, border:2px solid black]{
C_1e^{2x} + C_2xe^{2x} + C_3e^{-2x} + C_4xe^{-2x}
}
$$

######2C-1c)
$$
\begin{align}
y'' + 2y' + 2y &= 0 \\\
r^2 + 2r + 2 &= 0 \\\
r &= {-2\pm\sqrt{4-8}\over 2}\\\
r &= {-2\pm\sqrt{-4}\over 2}\\\
r &= -1\pm i\\\
\end{align}
$$
$$
\bbox[5px, border:2px solid black]{
C_1e^{t{-1+i}} + C_2e^{t{-1-i}}
}
$$

######2C-1d)
$$
\begin{align}
y'' - 2y' + 5y &= 0 \\\
r^2-2r+5 &= 0\\\
r &= {2\pm\sqrt{4-20}\over2}\\\
r &= 1\pm2i\\\
\end{align}
$$
$$
\begin{align}
C_1e^{t{1+2i}} +C_2e^{t{1-2i}}
\end{align}
$$
But its easier to try with the root $$$1+2i$$$ and the real-imaginary rules.
Suppose we have an imaginary root:
$$
e^{t{a+bi}}
$$
Then rewrite as $$$e^{at}e^{bit}$$$, and then
$$$e^{at}(cos(bt)+ isin(bt))$$$.  
Since the real and imaginary parts of this root must both be zero for their sum to be zero, we have two potential solutions, $$$e^{at}cos(bt)$$$ and $$$e^{at}sin(bt)$$$.
We can write these in the form:
$$C_1e^{at}cos(bt) + C_2e^{at}sin(bt)$$

For our use case, this is:
$$C_1e^{t}cos(2t) + C_2e^{t}sin(2t)$$

Given that $$$y(0) = 1, y'(0) = -1$$$ we have:
$$
\begin{align}
C_1e^{0}cos(0) + C_2e^{0}sin(0) &= 1\\\
C_1 &= 1 \\\
\\\
C_1\left(e^{t}cos(2t) + -2e^{t}sin(2t)\right) + C_2\left(e^{t}sin(2t) + 2e^{t}cos(2t)\right) &= y'(t) \\\
C_1\left(e^{0}cos(0) + -2e^{0}sin(0)\right) + C_2\left(e^{0}sin(0) + 2e^{0}cos(0)\right) &= -1 \\\
C_1(1) + 2C_2(1) &= -1\\\
1 + 2C_2 &= -1 \\\
2C_2 & = -2 \\\
C_2 &= -1
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{e^{t}cos(2t) -e^{t}sin(2t)}
$$

######2C-1e)
$$
\begin{align}
y''-4y'+4y &= 0\\\
r^2-4r+4 &= 0 \\\
(r-2)^2 &= 0\\\
r &= 2\\\
\end{align}
$$
Doubled roots, therefore the solution is:
$$
\bbox[5px, border:2px solid black]{C_1e^{2t} + C_2te^{2t}}
$$

The reason why this works:   
Assume that $$$e^{rt}$$$ is a solution to:
$$$y'' + Ay' + By = 0$$$.
$$
\begin{align}
y(t) &= e^{rt}\\\
y'(t) &= re^{rt}\\\
y''(t) &= r^2e^{rt}\\\
\end{align}
$$

$$
\begin{align}
y'' + Ay' + By &= 0 \\\
r^2e^{rt} + Are^{rt} + Be^{rt} &= 0 \\\
e^{rt}\left(r^2+Ar+B\right) &= 0 \\\
\end{align}
$$

$$
\begin{align}
y(t) &= te^{rt}\\\
y'(t) &= e^{rt} + tre^{rt}\\\
y''(t) &= re^{rt} + r\left(e^{rt} + tre^{rt}\right)\\\
y''(t) &= re^{rt} + re^{rt} + r^2te^{rt}\\\
y''(t) &= 2re^{rt} + r^2te^{rt}\\\
\end{align}
$$

$$
\begin{align}
y'' + Ay' + By &= 0 \\\
\left(te^{rt}\right)'' + A\left(te^{rt}\right)' + \left(te^{rt}\right) &= 0 \\\
2re^{rt} + r^2te^{rt} + A\left(e^{rt} + tre^{rt}\right) + B\left(te^{rt}\right) &= 0 \\\
2re^{rt} + r^2te^{rt} + Ae^{rt} + Atre^{rt} + Bte^{rt} &= 0 \\\
te^{rt}(r^2+Ar+B) + e^{rt}(2r+A) &= 0 \\\
t(0) + e^{rt}(2r+A) &= 0 \\\
e^{rt}(2r+A) &= 0 \\\
\end{align}
$$
So $$$te^{rt}$$$ is a root if $$$e^{rt}$$$ is a root and $$$r={-A\over2}$$$.   
By the characteristic equation:
$$
\begin{align}
y'' + Ay' + By &= 0 \\\
r^2 + Ar + B &= 0 \\\
r &= {-A \pm \sqrt{A^2-4B}\over 2}\\\
\end{align}
$$
Note that in the case where there is only one root, $$$A^2-4B = 0$$$, so we have:
$$
r={-A \over 2}
$$
And therefore, for any case in which there is only one root $$$A^2-4B=0$$$, $$$e^{rt},\ te^{rt}$$$ are solutions, with $$$r={-A\over2}$$$.

######2G-1i)
$$
\begin{align}
y'' + 2y' + cy &= 0 \\\
r^2 + 2r + c &= 0 \\\
{-2\pm\sqrt{4-4c}\over2} &= r\\\
\end{align}
$$
Case 1: 2 real roots:
$$
\begin{align}
4-4c &> 0 \\\
4 &> 4c\\\
1 &> c \\\
\end{align}
$$
$$\bbox[5px, border:2px solid black]{c < 1}$$

Case 2: 1 (doubled) real root:
$$
\begin{align}
4-4c &= 0 \\\
4 &= 4c\\\
1 &= c \\\
\end{align}
$$
$$\bbox[5px, border:2px solid black]{c = 1}$$

Case 3: 2 imaginary roots:
$$
\begin{align}
4-4c &< 0 \\\
4 &< 4c\\\
1 &< c \\\
\end{align}
$$
$$\bbox[5px, border:2px solid black]{c > 1}$$

######2G-1ii)
$$
\begin{align}
{-2\pm\sqrt{4-4c}\over2} &= r\\\
\end{align}
$$
2 real, negative roots:
$$
\begin{align}
-2 + \sqrt{4-4c} &< 0 \\\ 
\sqrt{4-4c} &< 2 \\\
4-4c &< 4 \\\
-4c &< 0 \\\
c &> 0\\\
\end{align}
$$
$$
\bbox[5px, border:2px solid black]{0 < c < 1}
$$

2 real, positive roots:
$$
\begin{align}
-2 - \sqrt{4-4c} &> 0 \\\
-2 &> \sqrt{4-4c} \\\
\end{align}
$$
$$\bbox[5px, border:2px solid black]{\varnothing}$$

Differing root values:
$$\bbox[5px, border:2px solid black]{c < 0}$$

######2G-1iii)
<-1 pos 1 neg->$$$0$$$<-2x negative->$$$1$$$(doubled real)<-2x imaginary->

######2G-1iv)
This is stable if all roots have negative real part; so 2x negative roots.
It turns out that this is the section of 2x negative and also the doubled real happens to have negative real part. The 2x imaginary roots also have negative real part, so this region is the region $$$\bbox[5px, border:2px solid black]{c > 0}$$$.

######2.3 #5)
$$
\begin{align}
y'' + 6y' + 9y &= 0 \\\
r^2 + 6r + 9 &= 0 \\\
(r+3)^2 &= 0 \\\
r &= -3\\\
\end{align}
$$
$$
\bbox[5px, border:2px solid black]{C_1e^{-3t} + C_2te^{-3t}}
$$

######2.3 #21)
$$
\begin{align}
y'' - 4y' + 3y &= 0 \\\
r^2 - 4r + 3 &= 0 \\\
(r-3)(r-1) &= 0 \\\
\end{align}
$$
The general solution is:
$$
C_1e^{3t} + C_2e^{t}
$$
Using the initial conditions $$$y(0) = 7,\ y'(0) = 11$$$:   
$$
\begin{align}
y(t) &= C_1e^{3t} + C_2e^{t}\\\
y(0) &= C_1e^{0} + C_2e^{0}\\\
7 &= C_1 + C_2\\\
\\\
y'(t) &= 3C_1e^{3t} + C_2e^{t}\\\
y'(0) &= 3C_1e^{0} + C_2e^{0}\\\
11 &= 3C_1 + C_2\\\
\\\
11 - 7 &= 3C_1 - C_1 + C_2-C_2\\\
4 &= 2C_1\\\
2 &= C_1\\\
\\\
7 &= 2 + C_2\\\
5 &= C_2\\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{2e^{3t} + 5e^{t}}
$$

######2.3 #23)
$$
\begin{align}
y'' - 6y' + 25y &= 0 \\\
r^2 - 6r + 25 &= 0  \\\
r &= {6\pm \sqrt{36-100}\over 2}\\\
r &= 3 \pm 4i\\\
\end{align}
$$
Use the solution $$$e^{(3+4i)t}$$$:
$$
\begin{align}
e^{3+4i} &= e^{3t}e^{4it}\\\
&= e^{3t}\left(cos(4t) + i sin(4t)\right)\\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{C_1e^{3t}cos(4t) + C_2e^{3t}sin(4t)}
$$
Using the initial conditions $$$y(0) = 3,\ y'(0)=1$$$:
$$
\begin{align}
y(t) &= C_1e^{3t}cos(4t) + C_2e^{3t}sin(4t)\\\
y(0) &= C_1e^{0}cos(0) + C_2e^{0}sin(0)\\\
3 &= C_1\\\
\\\
y'(t) &= C_1\left(3e^{3t}cos(4t) -4sin(4t)e^{3t}\right) + C_2\left(3e^{3t}sin(4t) + e^{3t}cos(4t)\right)\\\
y'(0) &= C_1\left(3e^{0}cos(0) - \cancel{4sin(0)e^{0}}\right) + C_2\left(\cancel{3e^{0}sin(0)} + e^{0}cos(0)\right)\\\
1 &= C_1(3) + C_2(1)\\\
1 &= 3C_1 + C_2\\\
\\\
1 &= 3(3) + C_2\\\
-8 &= C_2\\\
\end{align}
$$
$$
\therefore \bbox[5px, border:2px solid black]{3e^{3t}cos(4t) -8e^{3t}sin(4t)}\\\
$$


