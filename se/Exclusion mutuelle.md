# Mutual Exclusion
The process needs to block the resources from the other processes so that no problems will occure, until the process finishes with these resources.

when 2 processes have the same task at the same time, they can make mistake of resolving it twice which is problematic

so this is the solution of blocking one of them, because the other one wont have the neccesary tools to finish the task

## Example:
| n    | seats |
| ---- | ----- |
| 1616 | 3     |
| 2525 | 0     |
| 1537 | 7     |
```js
for(let n=0; n < table.length; n++){
	const E = table[n];
	if(E < 0){
		print(n);
		table[n]--;
	}else
		print("Pas de place");
}
```


