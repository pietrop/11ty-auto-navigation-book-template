# Reverse a list in place

Write function that reverses a list, preferably in place.

## Feverse

```jsx
[1,2,3,4,5,6,7,8,9].reverse()
```

## Two pointers approach

In place 

```jsx
// Write function that reverses a list, preferably in place.
let sampleList = [1,2,3,4,5,6,7,8,9];

function reversesList(list){
    let startPointerIndex = 0;
    let endPointerIndex = list.length-1;
		// since the two pointers are converging to the middle
		// loop up to half the length of the array
    for(let i=0; i<list.length/2; i++){
        let tmpStart = list[startPointerIndex];
        let tmpEnd = list[endPointerIndex];
        // swap 
        list[startPointerIndex] = tmpEnd;
        list[endPointerIndex] = tmpStart;
        // update pointers;
        startPointerIndex++;
        endPointerIndex--;
    }
    return list;
}

let result = reversesList(sampleList)
console.log(result)
// [9, 8, 7, 6, 5, 4, 3, 2, 1]
```

## Question from

[Simple Programming Problems](https://adriann.github.io/programming_problems.html)

List, strings