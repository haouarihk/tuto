a process in which events occur continuously and independently at a constant average rate.

## $x\sim E(a)$
the function is [[Continuous]].


## [[Density]]
 $$f(x) = \begin{cases} \lambda\cdot e^{-\lambda x} & x \in [0,+\infty[ \\ 0 & \text{else} \end{cases}$$
### Proof
$$\int_{0}^{+\infty} a\cdot e^{-ax}\,dx = 1$$
$= a\times\int_{0}^{+\infty} e^{-ax}\,\,dx$
$= -e^{-ax}  \mid_{0}^{+\infty}$
$= \lim_{x\to+\infty} (-e^{-ax})  - (-e^{0})$ 
$= 0 + 1$
$= 1$



## [[Spovence]] 

$$E(x) = \frac{1}{\lambda}$$
### Proof
$$
E(x) = \int_{0}^{+\infty} x\cdot\lambda e^{-\lambda x} \,\,dx
$$


$= \lambda\times\int_{0}^{+\infty}x e^{-\lambda x}\,\,dx$
> using the law $\int z\cdot h^{'} = z\cdot h - \int z^{'}\cdot h$
	$z = x$
	$h^{'} = e^{-\lambda x}$
   we get 
	$h = \frac{e^{-\lambda x}}{-\lambda}$
	$z^{'} = 1$

$=\lambda\times [x\frac{e^{-\lambda x}}{-\lambda} - \int\frac{e^{-\lambda x}}{-\lambda}]_{0}^{+\infty}$

$=[-xe^{-\lambda x} + \int e^{-\lambda x}]_{0}^{+\infty}$

$=-[xe^{-\lambda x} + \frac{e^{-\lambda x}}{\lambda}]_{0}^{+\infty}$

$= \overbrace{\lim_{x \to+\infty} (\overbrace{x\underbrace{e^{-\lambda x}}_{\text{dominant}}}^{0} + \frac{\overbrace{e^{-\lambda x}}^{0}}{\lambda})}^{0} +\frac{1}{\lambda}$

$= \frac{1}{\lambda}$


## [[Variance]] 
$$V(x) = \frac{1}{\lambda^{2}}$$

### Proof
soon.
