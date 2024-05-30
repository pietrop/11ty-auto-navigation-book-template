# Remove duplicates form an array

## Solutions

### With sets

It's unlikely you'll be able to leverage ES6 features to solve this problem, but just in case, here's a solution using sets.

```jsx
const unique = [... new Set(array)]
```

### With filter

```jsx
arra.filter((item, index)=>{array.indexOf(item)===index})
```

### With two nested for loop (brute force)

O(n^2) coz you'd iterate over all the items twice

```jsx
function removeDuplicates(array) {
  const result = [];
  for (let i = 0; i < array.length; i++) {
    let exists = false;
    for (j = 0; j < result.length; j++) {
      if (array[i] === result[j]) {
        exists = true;
        break;
      }
    }
    if (!exists) {
      result.push(array[i]);
    }
  }
  return result;
}
```

### With hash map

Pseudo code

```jsx
// keep a hash map to keep track of duplicates

// have a result array to add unique elements to

// iterate over all the elements

// if the elements is not in the hash map already 
		// add it to the results array 
		// and to the hash map 

// return the result array 
```

Code

```jsx
function removeDuplicates(array) {
  const result = [];
  const map = {};
  for (let i = 0; i < array.length; i++) {
	 if (!map[array[i]]) {
      result.push(array[i]);
      map[array[i]] = true;
    } 
  }
  return result;
}
```

```jsx
function removeDuplicates(array){
    const results = [];
    const map = {};
    array.forEach((a)=>{
	    if(!map[a]){
	        results.push(a)
	        map[a] = true;
	    }
    })
    return results;
}
```

## Background

[How to Remove Duplicates from an Array in JavaScript](https://ajahne.github.io/blog/javascript/2020/02/04/how-to-remove-duplicates-from-an-array-in-javascript.html)

[](https://medium.com/dailyjs/how-to-remove-array-duplicates-in-es6-5daa8789641c)

## Possible follow up

Big O complexity for hash map solution?

O(n)

Big O complexity for brute force solution with two nested arrays? 

O(n2)

What if we want to compare strings in a case insensitive way?

What if we were comparing objects loads of nested attributes?

A: deep comparison 

Q: what are some ways to do deep comparison?