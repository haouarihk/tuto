
pour fabrici  P1 et P2


on utilizy 3 machines, 
les temps unitair son donnie par 

P1:
- 11min sur m1
- 7min sur m2
- 6min sur m3

P2:
- 9min sur m1
- 12min sur m2
- 16min sur m3

useable time for each machine
M1: 165h
M2: 140h
M3: 160h

profit
P1: 900DA
P2: 1000DA

Objective:
combian le p1 et p2 poour avaor un profit meszzsugie

donnie le piel <><><>< corispondon


# Solution
**x:** represents P1
**y:** represents P2

**red:** $11x + 9y \le 165*60$
**green:** $7x + 12y \le 140*60$
**blue:** $6x + 16y \le 160 * 60$

```desmos-graph
right=1116;top=754;
---
y=(165*60 - 11x)/9 |red
y=(140*60 - 7x)/12 |green
y=(160*60 - 6x)/16 |blue
```


finding the intersections:

- **M1(0, 600)**
from graph	
- **M2(900, 0)**
from graph	

- **M3(480, 420)**
green x blue:
	$\frac{140\times60-7x}{12}=\frac{160*60-6x}{16}$
	$\to 200-\frac{7}{6}x = -\frac{6}{8}x$
	$\to x=\textbf{480}$
	and we can find y by plugging it to one of the functions:
	$y=\frac{140\times60-7\times480}{12\times480}$
	$\to y = \textbf{420}$
	
- **M4(626, 335)**
green x red:
	$\frac{140\times60-7x}{12}=\frac{165*60-11x}{9}$
	$\to (11\times12- 7\times9)\times x  = 165\times60\times12-140\times60\times9$
	$\to x = \frac{43200}{69}\approx\textbf{626.08}$
	and we can find y by plugging it to one of the functions:
	$y \approx \textbf{334.78}$ 



### Calculating the optimal for maximum Profit

**Y:** represents the total profit
	$Y = 900x + 100y$

we plug every point and see which one has the best profit
- M1(0, 600)
	$y1=900\times0 + 1000\times600 = \textbf{600,000}$

- M2(900, 0)
	$y2=900\times900 + 1000\times0 = \textbf{810,000}$

- M3(480, 420)
	$y3=900\times480 + 1000\times420 = \textbf{852,000}$
	
- **M4(626, 335)**
	$y3=900\times626 + 1000\times335 = \textbf{898,400}$

 **Best Optimal Values For maximum Profit is M4(626. 335)**
