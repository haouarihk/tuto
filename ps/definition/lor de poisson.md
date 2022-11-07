## $X\sim P(\lambda)$


(1)
$$P(x=R) = e^{-\lambda}\times\frac{\lambda^{R}}{R!}$$


calculating E(x) gonna be easy:
$E(x) = \lambda$

calculating V(x) also is easy:
$V(x) = \lambda$



## Proof (most likely be in the exam):

### ----------- $E(x)=\lambda$ -----------

we know 
(2)
$$e^x = \sum_{k\geq0}\frac{x^k}{k!} $$
(3)
$$E(x)=\sum_{x_{i}\geq0}^{x} x_{i}\times P(x=x_{i})$$
by puttiig (1) in (3) and replacing i with k
and $e^{-\lambda}$ has no relation with the sum, so we can take it aside
$$
E(x) = e^{-\lambda}\sum_{k\geq0}^{x} k\times\frac{\lambda^{k}}{k!}  
$$

we know: $k! = k\times(k-1)!$
$$ \to e^{-\lambda}\sum_{k\geq1} k\times\frac{\lambda^{k}}{k\times(k-1)!}$$

then we can just, take k with k.
$$ \to e^{-\lambda}\sum_{k\geq1}\frac{\lambda^{k}}{(k-1)!}  $$
if we can get the fraction in the form of (2), we can get it to be $e^{\lambda}$
we know that: $\lambda^{k} = \lambda\times\lambda^{k-1}$
and since lambda is not related to the sum, we can take it aside
therefore
$$\to\lambda\times e^{-\lambda}\sum_{k\geq1}\frac{\lambda^{k-1}}{(k-1)!}  $$
after replacing sum part, according to equation (2). we get
$$\to\lambda\times e^{-\lambda}\times e^{\lambda} $$
which equals to: $\lambda$


### ----------- $V(x)=\lambda$ -----------

we know 
$$
V(x) = \sum\limits_{x_{i}\geq0}\left(x_{i}^{2}\times P(x_{i})\right) - E^{2}(x)
$$

lets forget about E(x) for now, because we know it's value already.
let's replace i with k, and also replace P(x) with it's value
$$
\to e^{-\lambda}\sum\limits_{k\geq0} k^{2}\times\frac{\lambda^{k}}{k!}
$$
we know: $k! = k\times(k-1)!$
$$ \to e^{-\lambda}\sum_{k\geq1} k^{2}\frac{\lambda^{k}}{k\times(k-1)!}  $$
then we can just, take k with k.
and $e^{-\lambda}$ has no relation with the sum, so we can take it aside
$$ \to e^{-\lambda}\sum_{k\geq1}k\frac{\lambda^{k}}{(k-1)!}$$
isn't k just k-1+1.
we can put it there
$$ \to e^{-\lambda}\sum_{k\geq1}(k-1+1)\frac{\lambda^{k}}{(k-1)!}$$
we spread the equation between k-1, and 1 (watch out, this is where some people fail).
$$ \to e^{-\lambda}\sum_{k\geq1}\left((k-1)\frac{\lambda^{k}}{(k-1)!}+ \frac{\lambda^{k}}{(k-1)!}\right)$$
isn't $(k-1)! = (k-1)\times(k-2)!$
we can apply that, and take it away
$$ \to e^{-\lambda}\sum_{k\geq1}\left(\frac{\lambda^{k}}{(k-2)!}+\frac{\lambda^{k}}{(k-1)!}\right)$$

let's do the same thing we did while solving E(x) by taking away one lambda from the second fraction, and two from the first fraction, we end up with 
$$ \to e^{-\lambda}\sum_{k\geq1}\left(\lambda^{2}\frac{\lambda^{k-2}}{(k-2)!}+\lambda\frac{\lambda^{k}}{(k-1)!}\right)$$
since between the sides we have addition, we can safely give each one the sum operator
we can get the lambdas out because they are not related to the sum
$$ \to e^{-\lambda}\lambda^{2}\sum_{k\geq2}\frac{\lambda^{k-2}}{(k-2)!}+e^{-\lambda}\lambda\sum_{k\geq1}\frac{\lambda^{k}}{(k-1)!}$$

note: I almost always forget to also spread the $e^{-\lambda}$ along with the sum operator.

from (2) we get
$$ \to e^{-\lambda}\lambda^{2} e^{\lambda}+e^{-\lambda}\lambda e^{-\lambda}$$

which is after subtracting $E^{2}(x) = \lambda^{2}$
$$ \to \lambda^{2} +\lambda - \lambda^{2}$$
which equals to: $\lambda$
