$$$\require{cancel}$$$
# 18.03
##### Recitation 1 - 
######Introduction, natural growth and decay, review of logarithm.
[Problem Source](http://ocw.mit.edu/courses/mathematics/18-03-differential-equations-spring-2010/recitations/MIT18_03S10_rec_01.pdf)

1. A model of the oryx population can be as follows:
$$f(t + \Delta t) = kf(t)\Delta t+ f(t)- a \Delta t$$
$${f(t + \Delta t) - f(t) \over \Delta t} = k f(t) - a$$
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
And we have our solution.
