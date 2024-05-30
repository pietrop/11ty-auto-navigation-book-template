# multiplication table

> Write a program that prints a multiplication table for numbers up to 12 or up to `k`

```jsx
/**
 * returns core logic to make a 2D array of multiplication table
 * @returns 2D array
 */
const printMultiplicationTable = (num=12) => {
  const table = [];
  // counter starting at 1 to avoid zero padding on table
  for (let j = 1; j <= num; j++) {
    let row = new Array(num).fill(1);
    for (let i = 0; i < num; i++) {
      row[i] = (i + 1) * j;
    }
    table.push(row);
  }
  return table;
};

let res = printMultiplicationTable(24);
console.log(res)
```

![multiplication%20table%20154295e12e744922ac7caa7f31535db5/Screen_Shot_2021-06-03_at_7.38.52_PM.png](multiplication%20table%20154295e12e744922ac7caa7f31535db5/Screen_Shot_2021-06-03_at_7.38.52_PM.png)