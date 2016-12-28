#18.03
###Recitation 3
######1)
| n | $$$x_n$$$| $$$y_n$$$ | $$$f(x_n, y_n)$$$ | $$$hf(x_n, y_n)$$$ |
|---|----------|-----------|-------------------|------------------- |
|0|0|-1|1|0.5|
|1|0.5|-0.5|0|0|
|2|1|-0.5|-0.75|-0.375|
|3|1.5|-0.875|0|0|

![image](r3p1.png =250x250)

######2)
To figure this out we can find out the double derivative at the target value of $$$x=1.5$$$.

$$y'' = (y^2 - x^2)'$$
$$y'' = 2*y' - 2x$$
$$y'' = 2\*(y^2-x^2) - 2x$$
$$y'' = 2y^2 - x^2 - 2x$$
$$y'' = 2y^2 - (1.5)^2 - 2\*(1.5)$$

We can see that the second derivative is negative, indicating that the curve is concave-down, and therefore the euler's approximation is likely to overshoot.
This is confirmed by the image from problem (1) where we can see that the red line (euler's approximation) is above the approximated solution curve for the given differential equation.

######3)


