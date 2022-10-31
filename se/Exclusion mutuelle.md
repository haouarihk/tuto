The process needs to block the resources from the other processes so that no problems will occure, until the process finishes with these resources.

- when 2 processes have the same task([[SC]]) at the same time, they can make mistake of resolving it twice which is problematic

- when 2 proccess access the same variable([[RC]]), to modify it or/and check it. it could result in errors, if they both get executed at the same time, in parralel. the if statement could become outdated the moment it checks, by the other proccess modifying the variable that is being used right after the first proccess checks for it.

So this is the solution of blocking one of them, because the other one wont have the neccesary tools to finish the task

## Example:
| n    | seats |
| ---- | ----- |
| 1616 | 3     |
| 2525 | 0     |
| 1537 | 7     |
```js
if(table[1616] < 0){
	print(table[1616]);
	table[1616]--;
} else
	print("Pas de place");
```


## How does the question comes:

Every line of code will be named ($I_1$ ..),

He will give you multiple proccesses Code.

He will give you a table with different modes, (order of execution of each line on each proccess)

He will ask you if the mode is correct, logically.

And also what was the *valeur ribrplace*, *nobmre billet impremes*

### example:
| Mode execution                       | valeur ribrplace | nobmre billet impremes | Resultant correct eu faux |       |
| ------------------------------------ | ---------------- | ---------------------- | ------------------------- |
| sequentielle: $P_1$ -> $P_2$ ->$P_3$           | 0                | 02                     | Correct                   |    
| parralel: $P_1\|P_2\|P_3$                          |                  |                     |                         |
|   Pseudo-parralel: case1: $I_0,I_{0}^{'}$                                   |                  |                        |                           |       |
|                                      |                  |                        |                           |       |



## solution:
sc: section critique;
snc: section non critique;
Process P1 & P2
```js
let bussy = false;

<snc>
while(bussy){};
bussy = true;
<sc>
bussy = false;
<snc>

```
It will block the process with the while loop, until it's not bussy.
