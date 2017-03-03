$$$\require{cancel}$$$

# 18.03
###Pset 4
[Problem Source](https://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/assignments/MIT18_03S10_ps4.pdf)
#####Part 2.
######13a)
$$
\begin{align}
\dot{x} + 2x &= e^{3t}cos(4t)\\\
{dx\over dt} + 2x &= Re\\{e^{3t}e^{4it}\\}\\\
{dx\over dt} + 2x &= Re\\{e^{(3+4i)t}\\}\\\
x_p &= Re\left\\{{e^{(3+4i)t}\over p(3+4i)}\right\\}\\\
p(D) &= D + 2\\\
p(3+4i) &= 3 + 4i + 2\\\
&= 5 + 4i\\\
x_p &= Re\left\\{{e^{(3+4i)t}\over 5+4i}\right\\}\\\
x_p &= Re\left\\{e^{3t}{cos(4t)+isin(4t)\over 5+4i}\right\\}\\\
x_p &= Re\left\\{e^{3t}{cos(4t)+isin(4t)\over 5+4i}\right\\}\\\
x_p &= Re\left\\{e^{3t}{\left(cos(4t)+isin(4t)\right)\left(5-4i\right)\over(5+4i)(5-4i)}\right\\}\\\
x_p &= \bbox[5px, border:2px solid black]{e^{3t}{5cos(4t)-4sin(4t)\over 41}}\\\
\dot{x_h} + 2x_h &= 0\\\
{dx_h\over dt} + 2x_h &= 0\\\
{dx_h\over dt} &= -2x_h\\\
\int {1\over -2x_h} dx_h &= \int dt\\\
-{1\over 2}ln(x_h) &= t\\\
x_h &= \bbox[5px, border:2px solid black]{e^{-2t}}\\\
x &= x_p + x_h\\\
x &= \bbox[5px, border:2px solid black]{e^{3t}{5cos(4t)-4sin(4t)\over 41} + e^{-2t}}\\\
\end{align}
$$

######13b)
$$
\begin{align}
\ddot{x} + \dot{x} + 2x &= cos(t)\\\
\ddot{x} + \dot{x} + 2x &= Re\\{e^{it}\\}\\\
p(D) &= D^2 + D + 2\\\
x_p &= Re\left\\{{e^{it}\over p(i)}\right\\}\\\
x_p &= Re\left\\{{e^{it}\over (i)^2+i
+2}\right\\}\\\
x_p &= Re\left\\{{e^{it}\over i
+1}\right\\}\\\
x_p &= Re\left\\{{\left(cos(t) + isin(t)\right)\left(i-1\right)\over (i-1)(i+1)}\right\\}\\\
x_p &= {-cos(t)-sin(t)\over -2}\\\
x_p &= \bbox[5px, border:2px solid black]{{cos(t) + sin(t) \over 2}}\\\
x_p &= \bbox[5px, border:2px solid black]{{1\over 2}cos\left(t-{\pi\over 4}\right)}\\\
\ddot{x_h} + \dot{x_h} + 2x_h &= 0\\\
r^2 + r + 2 &= 0\\\
r &= {-1\pm\sqrt{1-8}\over 2}\\\
r &= {-1\pm\sqrt{-7}\over 2}\\\
x_h &= \bbox[5px, border:2px solid black]{C_1e^{{-1+i\sqrt{7}\over 2}t} + C_2e^{{-1-i\sqrt{7}\over 2}t}}\\\
x &= x_p + x_h\\\
x &= \bbox[5px, border:2px solid black]{{1\over 2}cos\left(t-{\pi\over 4}\right) + C_1e^{{-1+i\sqrt{7}\over 2}t} + C_2e^{{-1-i\sqrt{7}\over 2}t}} \\\
\end{align}
$$

######13c)
From the graph we see that the pseudoperiod is roughly:
$$$6.22-1.41=4.81$$$.

The predicted pseudoperiod was $$$2\pi$$$.

#####Part 1.
######2F6b)
$$
\begin{align}
y''' + y'' -y' + 2y &= 2 cos (x)\\\
p(D) &= r^3 + r^2-r + 2\\\
p(D)y(x) &= Re\left\\{2 e^{ix}\right\\}\\\
y(x) &= {2e^{ix}\over p(i)}\\\
p(i) &= i^3 + i^2-i+2\\\
&= -i-1-i+2\\\
&= -2i+1\\\
y(x) &= Re\left\\{{2e^{ix} \over -2i+1}\right\\}\\\
&= Re\left\\{{2\left(cos(x) + isin(x)\right)\over -2i+1}\right\\}\\\
&= Re\left\\{{2\left(cos(x) + isin(x)\right)\over -2i+1} \cdot {-2i-1\over -2i-1}\right\\}\\\
&= \bbox[5px, border:2px solid black]{{-2cos(x)+4sin(x)\over-5}}
\end{align}
$$

######2F6c)
$$
\begin{align}
y'' - 2y' + 4y &= e^{x}cos(x) \\\
p(D) &= r^2-2r+4 \\\
p(D)_{y(x)} &= Re\left\\{e^{x}e^{ix}\right\\}\\\
y(x) &= {e^{(i+1)x} \over (i+1)^2-2(i+1)+4}\\\
y(x) &= {e^{(i+1)x} \over -1+2i+1-2i-2+4}\\\
y(x) &= \bbox[5px, border:2px solid black]{{e^{(i+1)x} \over 2}}\\\
\end{align}
$$

######2F6d)
Notice that in this case the $$$p(\alpha) = 0$$$, and so
the rule $$${e^{\alpha x}\over p(\alpha)}$$$ is invalid for this equation.

The formula in the case of a double root is:
$$
\begin{align}
x_p &= {x^2e^{\alpha x}\over p''(\alpha)}\\\
\end{align}
$$

We can see that this is the case for $$$p(D) = (D-\alpha)(D-\alpha)$$$ through the following calculation:

$$
\begin{align}
p(D)e^{\alpha x}f(x) &= e^{\alpha x}p(D+\alpha)f(x)\\\
D\left(e^{\alpha x}f(x)\right) &= e^{\alpha x}Df(x) + \alpha e^{\alpha x}f(x) \\\
&= e^{\alpha x}(D+\alpha)f(x)\\\
\end{align}
$$
Applying the last equation repeatedly allows the first conversion (aka 'exponential shift rule') to hold.

To see that the double root formula holds (at least for second-order differential equations):
$$
\begin{align}
&p(D) = (D-\alpha)(D-\alpha)\\\
&p'(D) = 2(D-\alpha)\\\
&p''(D) = 2\\\
\end{align}
$$
$$
\begin{align}
p(D){x^2e^{\alpha x}\over p''(\alpha)} &= e^{\alpha x}\\\
&= {e^{\alpha x}p(D+\alpha)x^2\over p''(\alpha)}\\\
&= {e^{\alpha x}D^2x^2\over 2}\\\
&= {e^{\alpha x}2\over 2}\\\
&= e^{\alpha x}
\end{align}
$$

Applying the formula to the particular problem in this case:
$$
\begin{align}
y'' - 6y' + 9y &= e^{3x}\\\
y(x)_p &= \bbox[5px, border:2px solid black]{{x^2e^{3x}\over 2}}
\end{align}
$$

######14)
$$
\begin{align}
{d^3x\over dt^3}-x &= e^{2t}\\\
p(D) &= r^3-1\\\
x_p &= e^{2t}\over p(2)\\\
x_p &= \bbox[5px, border:2px solid black]{e^{2t}\over 7}
\end{align}
$$

To get the general solution, notice that:
$$
\begin{align}
{d^3x\over dt^3}-x &= 0\\\
r^3-1 &= 0\\\
(r+i)(r-i)(r-1) &= 0\\\
\end{align}
$$

And therefore we can write that the general solution is:
$$
\bbox[5px, border:2px solid black]{C_1e^{-it} + C_2e^{it} + C_3e^{t} + {e^{2t}\over 7}}
$$

######2C-8c)
$$
\begin{align}
y'' + y' + y &= 2xe^{x}\\\
p(D) &= D^2 + D + 1\\\
p(D)y &= 2xe^{x}\\\
y_p &= f(x)e^{x}\\\
p(D)f(x)e^{x} &= e^{x}p(D+1)f(x)\\\
e^{x}p(D+1)f(x) &= 2xe^{x}\\\
p(D+1)f(x) &= 2x\\\
p(D+1) &= (D+1)^2 + (D+1) + 1\\\
p(D+1) &= D^2 + 2D + 1 + (D+1) + 1\\\
p(D+1) &= D^2 + 3D + 3\\\
f(x) &= Ax + B\\\
f'(x) &= A\\\
f''(x) &= 0\\\
p(D+1)f(x) &= 2x\\\
D^2f(x) + 3Df(x) + 3f(x) &= 2x\\\
0 + 3A + (3Ax+3B) &= 2x\\\
3Ax + 3A + 3B &= 2x\\\
3A + 3B &= 0\\\
3A &= 2\\\
A &= {2\over 3}\\\
B &= -{2\over 3}\\\
y_p &= \bbox[5px, border:2px solid black]{e^{x}\left({2\over 3}x - {2\over 3}\right)}
\end{align}
$$

For the general solution, we need to find the associated equation:
$$
\begin{align}
y''+ y' + y &= 0\\\
r^2 + r + 1 &= 0 \\\
\left(r-{-1+i\sqrt3\over2}\right)\left(r-{-1-i\sqrt3\over2}\right) &= 0 \\\
\end{align}
$$
$$\bbox[5px, border:2px solid black]{y(x) = C_1e^{1-i\sqrt3\over2} + C_2e^{1+i\sqrt3\over2} + e^{x}\left({2\over3}x-{2\over3}\right)}$$

######2C-8d)
Step 1: Find a particular solution $$$y_p$$$:
$$
\begin{align}
y'' - y &= x^2\\\
p(D) &= D^2-1\\\
p(D)u(x) &= x^2\\\
u(x) &= Ax^2+Bx+C\\\
u'(x) &= 2Ax+B\\\
u''(x) &= 2A\\\
p(D)u(x) &= x^2\\\
D^2u(x)-u(x) &= x^2\\\
2A-Ax^2+Bx+C &= x^2\\\
A &= -1\\\
B &= 0\\\
C &= -2\\\
u(x) &= -x^2-2\\\
\end{align}
$$

Step 2: Find a complementary solution $$$y_c$$$:
$$
\begin{align}
y'' - y &= 0\\\
r^2-1 &= 0\\\
(r+1)(r-1) &= 0\\\
y(x) &= C_1e^{-x} + C_2e^{x}\\\
\end{align}
$$

$$\therefore \bbox[5px, border:2px solid black]{y(x) = -x^2-2+C_1e^{-x}+C_2e^{x}}$$

Step 3: Include the initial conditions:
$$
\begin{align}
y(0) &= 0\\\
y'(0) &= -1\\\
y(x) &= -x^2-2+C_1e^{-x}+C_2e^{x}\\\
y(0) &= -(0)^2-2+C_1e^{0}+C_2e^{0}\\\
0 &= -2 + C_1 + C_2\\\
y'(x) &= -2x - C_1e^{-x}+C_2e^{x}\\\
y'(0) &= -2(0) - C_1e^{0}+C_2e^{0}\\\
-1 &= -C_1 + C_2\\\
C_1-1 &= C_2\\\
0 &= -2 + C_1 + C_1-1\\\
3 &= 2C_1\\\
C_1 &= {3\over 2}\\\
C_2 &= {1\over 2}\\\
\end{align}
$$
$$\therefore \bbox[5px, border:2px solid black]{y(x) = -x^2-2 + {3\over 2}e^{-x} + {1\over 2}e^{x}}$$

######2.5 #2)
$$
\begin{align}
y'' - y' - 2y &= 3x+4\\\
y_p &= Ax+B\\\
y_p'(x) &= A \\\
y_p''(x) &= 0 \\\
-A -2Ax-2B &= 3x+4\\\
-A-2B &= 4\\\
-2A &= 3\\\
A &= {-3\over 2}\\\
B &= {-5\over 4}\\\
y_p &= \bbox[5px, border:2px solid black]{-{3\over 2}x - {5\over 4}}
\end{align}
$$

######2.5 #8)
$$
\begin{align}
y'' - 4y &= cosh 2x\\\
y'' - 4y &= {e^{x}+e^{-x} \over 2}\\\
\end{align}
$$
Split this into two equations and add them (linearity):
$$
\begin{align}
{y'' - 4y\over 2} &= {e^{x}\over 2}\\\
{y'' - 4y\over 2} &= {e^{-x}\over 2}\\\
\end{align}
$$

Solving the first one:
$$
\begin{align}
{y'' - 4y\over 2} &= {e^{x}\over 2} \\\
y'' - 4y &= e^{x}\\\
y_p(x) &= {e^{x}\over p(1)}\\\
p(D) &= D^2 - 4\\\
p(1) &= 1 - 4\\\
p(1) &= -3\\\
y_p(x) &= {e^{x}\over -3}
\end{align}
$$

Solving the second one:
$$
\begin{align}
{y'' - 4y\over 2} &= {e^{-x}\over 2}\\\
y'' - 4y &= e^{-x}\\\
y_p(x) &= {e^{-x}\over p(1)}\\\
p(D) &= D^2-4\\\
p(1) &= (1)^2-4\\\
p(1) &= -3\\\
y_p(x) &= {e^{-x}\over -3}\\\
\end{align}
$$

Combining the first and second (ensuring the equation has the right values):
$$
\bbox[5px, border:2px solid black]{y_p(x) = {e^{x} + e^{-x}\over -6}}
$$

######2.5 #11)
$$
\begin{align}
y''' + 4y' &= 3x - 1\\\
p(D) &= D^3+4D\\\
p(D)y_p &= 3x - 1\\\
y_p &= Ax^2 + Bx\\\
y_p(x) &= Ax^2 + Bx\\\
y_p'(x) &= 2Ax + B\\\
y_p''(x) &= 2A\\\
y_p'''(x) &= 0\\\
0 + 8Ax + 4B &= 3x - 1\\\
A &= {3\over 8}\\\
B &= -1\over 4 \\\
y_p(x) &= \bbox[5px, border:2px solid black]{{3\over 8}x^2 - {1\over 4}x}\\\
\end{align}
$$

######2.5 #14)
$$
\begin{align}
y^{(4)} - 2y'' + y &= xe ^{x}\\\
p(D) &= D^4 - 2D^2 + 1\\\
p(D)u(x) &= xe^{x}\\\
u(x) &= e^{x}f(x)\\\
p(D)e^{x}f(x) &= e^{x}p(D+1)f(x)\\\
e^{x}p(D+1)f(x) &= xe^{x}\\\
p(D+1)f(x) &= x\\\
(D+1)^4 &= D^4 + 4D^3 + 6D^2 + 4D + 1\\\
(D+1)^2 &= D^2 + 2D + 1\\\
p(D+1) &= D^4 + 4D^3 + 6D^2 + 4D + 1 -2( D^2 + 2D + 1)+ 1\\\
p(D+1) &= D^4 + 4D^3 + 6D^2 + 4D + 1 - 2D^2 -4D - 2 + 1\\\
p(D+1) &= D^4 + 4D^3 + 4D^2\\\
f(x) &= Ax^3 + Bx^2\\\
f'(x) &= 3Ax^2 + 2Bx\\\
f''(x) &= 6Ax + 2B\\\
f'''(x) &= 6A\\\
f''''(x) &= 0\\\
p(D+1)f(x) &= D^4f(x) + 4(D^3f(x)) + 4(D^2f(x))\\\
p(D+1)f(x) &= 0 + 4(6A) + 4(6Ax+2B)\\\
p(D+1)f(x) &= 24A + 24Ax + 8B\\\
A &= {1\over 24}
B &= {-1\over 8}
f(x) &= {1\over 24}x^3 - {1\over8}x^2\\\
y_p(x) &= \bbox[5px, border:2px solid black]{e^{x}\left({1\over 24}x^3 - {1\over 8}x^2\right)}\\\  
\end{align}
$$

######2.6 #17)
$$
\begin{align}
mx'' + cx' + kx &= F_0cos(\omega t)\\\
mx'' + cx' + kx &= F_0Re\\{e^{i\omega t}\\}\\\
x'' + {c\over m}x' + {k\over m}x &= F_0Re\\{e^{i\omega t}\\}\\\
p(d) &= D^2 + 2pD + w_1^2\\\
x_p &= {F_0e^{i\omega_0 t}\over i\omega_0^2+2pi\omega_0 + \omega_1^2}\\\
&= {F_0e^{i\omega_0 t}\over \omega_1^2-\omega_0^2+2pi\omega_0}\\\
&= {F_0\left(cos(\omega_0 t) + isin(\omega_0 t)\right)\left((\omega_1^2-\omega_0^2)-2pi\omega_0\right)\over (\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2}\\\
&= {F_0\left((\omega_1^2-\omega_0^2)(cos(\omega_0 t)) + 2p\omega_0 sin(\omega_0 t)\right) \over (\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2}\\\
&= F_0\left({\omega_1^2-\omega_0^2 \over (\omega_1^2-\omega_0^2)^2+(2p\omega_0)^2}cos(\omega_0 t) + {2p\omega_0\over (\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2}sin(\omega_0 t)\right)\\\
\end{align}
$$
Let:
$$
\begin{align}
A = F_0{\omega_1^2-\omega_0^2 \over (\omega_1^2-\omega_0^2)^2+(2p\omega_0)^2}\\\
B = F_0{2p\omega_0\over (\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2}
\end{align}
$$
Then:
$$
\begin{align}
C&=\sqrt{A^2+B^2}\\\
\omega_r &= \omega_0t - {tan}^{-1}\left({B\over A}\right)\\\
\end{align}
$$

We know that the practical resonance frequency can be found through taking the derivative of the amplitude and looking for maxima, as the practical resonance frequency is defined as the maximal $$$\omega$$$ in the amplitude graph $$$C(\omega)$$$.

$$
\begin{align}
A &= F_0{\omega_1^2-\omega_0^2 \over (\omega_1^2-\omega_0^2)^2+(2p\omega_0)^2}\\\
B &= F_0{2p\omega_0\over (\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2} \\\
A^2+B^2 &= F_0^2\left({\left(\omega_1^2-\omega_0^2\right)^2+\left(2p\omega_0\right)^2\over \left((\omega_1^2-\omega_0^2)^2+(2p\omega_0)^2\right)^2}\right)\\\
&= F_0^2\left({1\over(\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2}\right)\\\
\sqrt{A^2+B^2} &= F_0\sqrt{{1\over(\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2}}\\\
\end{align}
$$

So $$C(\omega_1) = F_0\sqrt{{1\over(\omega_1^2-\omega_0^2)^2 + (2p\omega_0)^2}}$$

Plugging in the values given: $$$m=1$$$, $$$c=6$$$, $$$k=45$$$: 

$$$F_0=50$$$

$$${k\over m} = \omega_0^2 = 45$$$

$$${c\over m} = 2p = 6$$$:

$$C(\omega_1) = 50\sqrt{{1\over(\omega_1^2-45)^2 + (6\cdot45)^2}}$$
![Image](fig_1.png =400x300)
$$
\begin{align}
C'(\omega_1) &= {d\over d\omega_1}50\sqrt{{1\over(\omega_1^2-45)^2 + (270)^2}}\\\
&= {d\over d\omega_1}50\left((\omega_1^2-45)^2+270^2\right)^{-{1\over2}}\\\
&= {d\over d\omega_1}50\left(\omega_1^4-90\omega_1^2 + 2025 + 72900\right)^{-{1\over2}}\\\
&= {d\over d\omega_1}50\left(\omega_1^4-90\omega_1^2+74925\right)^{-{1\over2}}\\\
&= 50\left(-{1\over2}\left(\omega_1^4-90\omega_1^2+74925\right)^{-{3\over2}}\right)\left(4\omega_1^3-180\omega_1\right)\\\
\end{align}
$$
Setting $$$C'(\omega_1)=0$$$ in order to find the practical resonance frequency:
$$
\begin{align}
C'(\omega_1) &= 50\left(-{1\over2}\left(\omega_1^4-90\omega_1^2+74925\right)^{-{3\over2}}\right)\left(4\omega_1^3-180\omega_1\right)\\\
0 &= 50\left(-{1\over2}\left(\omega_1^4-90\omega_1^2+74925\right)^{-{3\over2}}\right)(4\omega_1^3) - 50\left(-{1\over2}\left(\omega_1^4-90\omega_1^2+74925\right)^{-{3\over2}}\right)(180\omega_1)\\\
50\left(-{1\over2}\left(\omega_1^4-90\omega_1^2+74925\right)^{-{3\over2}}\right)(180\omega_1) &= 50\left(-{1\over2}\left(\omega_1^4-90\omega_1^2+74925\right)^{-{3\over2}}\right)(4\omega_1^3)\\\
180\omega_1 &= 4\omega_1^3\\\
{180\over 4} &= \omega_1^2\\\
\sqrt{45} &= \omega_1\\\
\omega_1 &= \pm \bbox[5px, border:2px solid black]{6.7082}\\\
\end{align}
$$
