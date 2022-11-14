الكثافة


Each type has it's own equation to calculate it,

they all follow the same form,


 $f(x) = \begin{cases} F & x \in R \\ 0 & \text{else} \end{cases}$
 
F depends on the type of the distribution we are dealing with.
R is the area that this function works in, also depends on the distribution.


## How do we start with the proof

We always Need to prove that:
$$\int_{-\infty}^{+\infty} f(x)\,\, dx= 1$$
Almost always gonna use this equation to get the same segment \[a,b]
$$\int_{-\infty}^{+\infty}f(x) = \int_{-\infty}^{a} f(x) + \int_{a}^{b} f(x) + \int_{b}^{+\infty} f(x)$$
sometimes if you have a or b equal to infinity, you don't need the middle part.

and the first and last part will become 0. because they're out of the bounds of the first part of our equation

$$\int_{-\infty}^{+\infty}f(x) = \int_{a}^{b} f(x)$$

Therefore we will only need to prove that 
$$\int_{R_{0}}^{R_{1}} f(x)\,\, dx= 1$$
