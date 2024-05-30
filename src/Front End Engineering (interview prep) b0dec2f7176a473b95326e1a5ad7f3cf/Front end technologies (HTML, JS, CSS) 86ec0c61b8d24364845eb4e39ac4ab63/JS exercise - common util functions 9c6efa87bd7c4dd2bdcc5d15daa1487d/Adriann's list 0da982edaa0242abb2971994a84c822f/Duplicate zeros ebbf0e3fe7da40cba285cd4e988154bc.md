# Duplicate zeros

Start from the end of the array 

```jsx
let input = [1,0,2,3,0,4,5,0];

function duplicateZeros(arr) {
    for (let i=arr.length-1; i>=0; i--){
        const currentElement = arr[i];
        if(currentElement === 0){
             arr[i+1]=arr[i]
							// decrement counter to skip next elements
              i--;
        }
        else{
            arr[i+1]=arr[i]
        }
    }
    return arr;
};

let result = duplicateZeros(input);
console.log(result)
// [1, 0, 0, 2, 0, 0, 4, 0, 0]
```

Leet code solution, is more efficient, but also more complicated to wrap your head around it. It optimizes for the elements that end up "outside" of the array, once you have added the extra zeros - if that makes sense.

[Duplicate Zeros - LeetCode](https://leetcode.com/problems/duplicate-zeros/)