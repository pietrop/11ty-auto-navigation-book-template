# Insert element in array

For these data structure exercises, we can assume that only insert is a native operation. 

So to insert at the beginning or at an arbitrary index, we need to shift all the elements.

We shift them from the end. Up to the index of the insert point.

Inserting at the start, index 0, is a special case, where you have to iterate through the all array.

```jsx
function insert(list, k, position=0){
    for(let i=list.length-1; i>=position; i--){
        list[i+1]=list[i];
    }
    list[position]=k
    return list;
}

let sampleList = [1,2,3,4,5]
let sampleK = 6;

let result = insert(sampleList,sampleK)
console.log(result)
// [6, 1, 2, 3, 4, 5]

let samplePosition = 2;
let result2 = insert(sampleList,sampleK, samplePosition)
console.log(result2)
// [1, 2, 6, 3, 4, 5]
```

[Account Login - LeetCode](https://leetcode.com/explore/featured/card/fun-with-arrays/525/inserting-items-into-an-array/3244/)