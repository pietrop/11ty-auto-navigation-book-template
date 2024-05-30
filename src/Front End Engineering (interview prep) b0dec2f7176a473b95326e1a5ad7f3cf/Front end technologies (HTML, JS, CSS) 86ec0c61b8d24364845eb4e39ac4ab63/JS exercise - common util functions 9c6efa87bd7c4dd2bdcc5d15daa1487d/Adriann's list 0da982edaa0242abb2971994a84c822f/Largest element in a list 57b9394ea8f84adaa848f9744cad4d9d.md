# Largest element in a list

Write a function that returns the largest element in a list.

## Math Library

If can use Js Math library, then 

```jsx
let sampleList = [2,3,4,5,40,1,6,7,8];
Math.max(...sampleList)
```

## Loop

With a loop

```jsx
//Write a function that returns the largest element in a list.
let sampleList = [2,3,4,5,40,1,6,7,8];

function returnLargestElement(list){
    let max = list[0];
    list.forEach((l)=>{
        if(l>max){
            max = l;
        }
    })
    return max;
}

const result = returnLargestElement(sampleList);
console.log(result)
```

## Question from

[Simple Programming Problems](https://adriann.github.io/programming_problems.html)

List, strings