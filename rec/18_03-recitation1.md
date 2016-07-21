$$$\require{cancel}$$$
# 18.03
##### Recitation 1 - 
######Introduction, natural growth and decay, review of logarithm.
[Problem Source](http://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/recitations/MIT18_03S10_rec_01.pdf)

1. A model of the oryx population can be as follows:
$$f(t + \Delta t) = kf(t)\Delta t+ f(t)- a \Delta t$$
$${f(t + \Delta t) - f(t) \over \Delta t} = k f(t) - a$$
As $$$\Delta t \rightarrow 0$$$:
$$\bbox[5px, border:2px solid black] {{df(t)\over dt} = kf(t)-a}$$
This model is consistent if we choose the following units:
$$f(t + \Delta t)=> oryxes $$
$$k => {oryxes \over oryxes * year}$$
$$t => year$$
$$a => oryxes / year $$
$$\Delta t => year $$
$$f(t) => oryxes$$
Dimensional Analysis: $$oryxes = {\cancel{oryxes} \over \cancel{oryxes} * \cancel{year}} * oryxes * \cancel{year} - {oryxes \over \cancel{year}} * \cancel{year} + oryxes $$
which results in
$$oryxes = oryxes$$
2. In (1), we gave a model for modeling oryx populations at time $$$t + \Delta t$$$. Now, the problem revolves around finding the value of t that doubles the population. As in, we are looking for 
$$f(t + \Delta t) = 2 f(t)$$
We have a bit of a differential equation, as we can rewrite the original model to have a differential form, reproduced below with $$$a=0$$$:
$${d\over dt}f(t) = kf(t)$$
If we had the function $$$f(t)$$$, then we could solve the desired equation by plugging in $$$t$$$ and $$$\Delta t$$$.
Rewrite the function as:
$${1 \over f(t)}{d\over dt}f(t) = k$$
Take integral with respect to $$$dt$$$ on both sides:
$$\int {1\over f(t)}{d\over dt}f(t)\; dt = \int k\; dt$$
Now we can notice that the left side can be expressed as:
$$ {d \over df(t)}g(f(t)){d\over dt}f(t) = {d\over dt}g(f(t))$$
If we make the substitution:
$$ {d \over df(t)}g(f(t)) = {1 \over f(t)}$$
we can rewrite the left integral as:
$$ \int {d \over dt}g(f(t))\; dt$$
By the first fundamental theorem of calculus this reduces to:
$$ g(f(t)) $$
To solve for $$$g(f(t))$$$, we have:
$$ {d \over df(t)}g(f(t)) = {1 \over f(t)}$$
$$ \int {d \over df(t)} g(f(t))\; df(t) = \int {1 \over f(t)}\; df(t)$$
Again using the first fundamental theorem of calculus:
$$ g(f(t)) = ln(f(t)) + C$$
Which is the solution for the left side integral, so we have:
$$ ln(f(t)) = kt + C$$
Solving for f(t):
$$ f(t) = e^{C}e^{kt}$$
We want a factor of 2 between the f(t)s:
$$ {f(t + \Delta t) \over f(t)} = {e^{C}e^{k(t + \Delta t)} \over e^{C}e^{kt}}$$
$$ 2 = e^{k(t + \Delta t) - kt} $$
$$ 2 = e^{k\Delta t} $$
$$ \bbox[5px, border:2px solid black] { {ln(2) \over k} = \Delta t }$$
3. The general solution of this problem is the solution of the following differential equation:
$$ {d \over dt} f(t) = kf(t) - a $$
Let's substitute $$$y(t) = f(t) - {a \over k}$$$ to get:
$${dy(t)\over dt } = {df(t)\over dt} = ky(t)$$
because the $$${a\over k}$$$ is a constant and disappears during differentiation.
$$\int {1\over y(t)}{dy(t)\over dt}\;dt = \int k\;dt$$
Solving as before we end up with
$$ln(y(t)) = kt + C$$
Substituting the y(t) back for f(t) we receive:
$$ln(f(t)-{a\over k}) = kt + C$$
$$f(t) - {a \over k} = e^{kt+C}$$
$$\bbox[5px, border:2px solid black] {f(t) = Ce^{kt} + {a\over k}}$$
4. We can take the derivative of $$$(3)$$$ and compare it to plugging $$$(3)$$$ into $$$(1)$$$.
$$f(t) = Ce^{kt} + {a\over k} \qquad (3)$$
$${df(t)\over dt} = {d\over dt}\left( Ce^{kt} + {a\over k}\right)$$
$${df(t)\over dt} = {Cke^{kt}}$$
Combining $$$Ck$$$ into $$$C$$$:
$$\bbox[5px, border:2px solid black] {{df(t)\over dt} = {Ce^{kt}}\quad\checkmark}$$
From $$$(1)$$$ we have:
$${df(t)\over dt} = kf(t) - a$$
Plugging in $$$(3)$$$ we end up with:
$${df(t)\over dt} = k\left(Ce^{kt} + {a\over k}\right) - a$$
$${df(t)\over dt} = kCe^{kt} + k{a\over k} - a$$
$$\bbox[5px, border:2px solid black] {{df(t)\over dt} = Ce^{kt}\quad\checkmark}$$
And thus the solution $$$(3)$$$ is valid for the ODE presented in $$$(1)$$$.

