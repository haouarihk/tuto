# Mutual Exclusion
The process needs to block the resources from the other processes so that no problems will occure, until the process finishes with these resources.


## Example:
| n    | seats |
| ---- | ----- |
| 1616 | 3     |
| 2525 | 0     |
| 1537 | 7     |
```js
for(let n=0; n < table.length; n++){
	const E = table[n]
	if(E < 0){
		print(n)
		table[n]--;	
	}else
		print("ne Pa de place")
}
```


