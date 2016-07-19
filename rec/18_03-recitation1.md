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

