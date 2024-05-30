# Reverse a string

How would you implement `"123456789".reverse()`

## Solution(s)

Because `.reverse()` is run on the string, we need to add it to the prototype. 

Bonus, think of various options to achieve this. 

```jsx

String.prototype.reverse = function(){
  const tmpArray = Array.from(this);
  return tmpArray.reverse().join('');
} 

console.log("123456789".reverse())
```

as a variation of 

```jsx
String.prototype.revese = function(){
    const list =this.split('');
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
    return list.join('');
}

console.log("123456789".revese())
// 987654321
```