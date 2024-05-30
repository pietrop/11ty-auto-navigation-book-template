# Find intersection

eg find intersection between two lists

## Use a hash table

```jsx
// have a result array 

// put one list in a hash table

// then iterate on second list and check if it's present in hash table

	// if it's present then add to result array

// at the end check if result array is empty

	// if it's empty return false

  //  if it's not empty return the result array
```

```jsx
function findIntersection(firstList, secondList){
	const map = {};
	const result = [];

	firstList.forEach((n)=>{
		map[n] = true;
	})

	secondList.forEach((m)=>{
		if(map[m]){
			result.push(m)
		}
	})

	if(result.length ===0){
		return false;
	}
	else{
		return result;
	}
	
}
```

[Coderbyte | The #1 Coding Assessment Platform](https://coderbyte.com/video/find-intersection-solution)