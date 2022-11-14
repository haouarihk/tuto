## $x\sim u_E$
the function is [[Continuous]].

**E:** is the set
$E=\{x_{1},\,x_{2},\cdots\}$

when the set is [[EquiProbability]]


If it's uniform, and we know the length of the set.
we can conclude the probability of each one
## $P(x_{n})= \frac{1}{length(E)}$


## [[Density]]
 $$f(x) = \begin{cases} \frac{1}{b-a} & x \in [a,b] \\ 0 & \text{else} \end{cases}$$

### Proof
$$\int_{a}^{b} \frac{1}{b-a}\,dx = 1$$
$= \frac{1}{b-a}\times\int_{a}^{b} 1\,\,dx$
$= \frac{1}{b-a}\times x   \mid_{a}^{b}$
$= \frac{1}{b-a}\times (b-a) = 1$


## [[Spovence]] 

$$E(x) = \frac{b+a}{2}$$


### Proof
$$
E(x) = \int_{a}^{b} x\cdot\frac{1}{b-a}\,\,dx
$$
$= \frac{1}{b-a}\times\int_{a}^{b} x\,\,dx$
$= \frac{1}{b-a}\times \frac{x^{2}}{2} \mid_{a}^{b}$
$= \frac{1}{b-a}\times \frac{b^{2}-a^{2}}{2}$
$= \frac{1}{b-a}\times \frac{(b-a)\cdot(b+a)} {2}$

$$E(x)= \frac{b+a}{2}$$

## [[Variance]] 
$$V(x) = \frac{(b-a)^{2}}{12}$$

### Proof

> from [[Spovence]] we can get 

$$
 E^{2}(x)=\frac{(b+a)^{2}}{4}
$$

> calculating for $E(x^2)$

$$
E(x^{2}) = \int_{a}^{b} x^{2}\cdot\frac{1}{b-a}\,\,dx
$$
$= \frac{1}{b-a}\times\int_{a}^{b} x^{2}\,\,dx$
$= \frac{1}{b-a}\times \frac{x^{3}}{3} \mid_{a}^{b}$
$= \frac{1}{b-a}\times (\frac{b^{3}}{3} - \frac{a^{3}}{3})$
$= \frac{1}{b-a}\times \frac{b^{3}-a^{3}}{3}$

> we know that $b^{3} - a^{3} = (b - a) (b^{2} + ab + a^{2})$

$$E(x^{2})= \frac{b^{2} + ab + a^{2}}{3}$$

> calculating V

$$
V(x) = E(x^{2}) - E^{2}(x)
$$

$= \frac{b^{2} + ab + a^{2}}{3} -\frac{(b+a)^{2}}{4}$
$= \frac{4b^{2} + 4ab + 4a^{2} -3b^{2}-3a^{2}-6ab}{12}$

$= \frac{b^{2} + a^{2} + 2ab }{12}$

$$V(x)= \frac{(a+b)^{2}}{12}$$
