# Adriann's list

[Simple Programming Problems](https://adriann.github.io/programming_problems.html)

## Elementary

- [x]  Write a program that prints ‘Hello World’ to the screen.
- [x]  Write a program that asks the user for their name and greets them with their name.
- [x]  Modify the previous program such that only the users Alice and Bob are greeted with their names.
- [x]  Write a program that asks the user for a number `n` and prints the sum of the numbers 1 to `n`
- [x]  Modify the previous program such that only multiples of three or five are considered in the sum, e.g. 3, 5, 6, 9, 10, 12, 15 for `n`=17
- [x]  Write a program that asks the user for a number `n` and gives them the possibility to choose between computing the sum and computing the product of 1,…,`n`.
- [x]  Write a program that prints a multiplication table for numbers up to 12.
- [ ]  ~~Write a program that prints *all* prime numbers. (Note: if your programming language does not support arbitrary size numbers, printing all primes up to the largest number you can easily represent is fine too.)~~
- [ ]  ~~Write a guessing game where the user has to guess a secret number. After every guess the program tells the user whether their number was too large or too small. At the end the number of tries needed should be printed. It counts only as one try if they input the same number multiple times consecutively.~~
- [ ]  ~~Write a program that prints the next 20 leap years.~~
- [ ]  ~~Write a program that computes the sum of an alternating series where each element of the series is an expression of the form ((-1)^{k+1})/(2 * k-1) for each value of k from 1 to a million, multiplied by 4. Or, in more mathematical notation~~

    ```jsx
    ~~4\cdot \sum_{k=1}^{10^6} \frac{(-1)^{k+1}}{2k-1} = 4\cdot(1-1/3+1/5-1/7+1/9-1/11\ldots).~~
    ```

## Lists, Strings

- [x]  Write a function that returns the largest element in a list.
- [x]  Write function that reverses a list, preferably in place.
- [x]  Write a function that checks whether an element occurs in a list.
- [x]  Write a function that returns the elements on odd positions in a list.
- [x]  Write a function that computes the running total of a list.
- [x]  Write a function that tests whether a string is a palindrome.
- [ ]  Write three functions that compute the sum of the numbers in a list:
    - [ ]  using a `for`loop,
    - [ ]  a `while`loop
    - [ ]  and recursion. (Subject to availability of these constructs in your language of choice.)
- [ ]  Write a function `on_all` that applies a function to every element of a list. Use it to print the first twenty perfect squares. The perfect squares can be found by multiplying each natural number with itself. The first few perfect squares are `1*1= 1`, `2*2=4`, `3*3=9`, `4*4=16`. Twelve for example is not a perfect square because there is no natural number `m` so that `m*m=12`. (This question is tricky if your programming language makes it difficult to pass functions as arguments.)
- [x]  Write a function that concatenates two lists. `[a,b,c]`, `[1,2,3]` → `[a,b,c,1,2,3]`
- [x]  Write a function that combines two lists by alternatingly taking elements, e.g. `[a,b,c]`, `[1,2,3]` → `[a,1,b,2,c,3]`.
- [x]  Write a function that merges two sorted lists into a new sorted list. `[1,4,6]`,`[2,3,5]` → `[1,2,3,4,5,6]`. You can do this quicker than concatenating them followed by a sort.
- [ ]  Write a function that rotates a list by `k` elements. For example `[1,2,3,4,5,6]` rotated by two becomes `[3,4,5,6,1,2]`. Try solving this without creating a copy of the list. How many swap or move operations do you need?
- [ ]  Write a function that computes the list of the first 100 Fibonacci numbers. The first two Fibonacci numbers are 1 and 1. The `n+1`st Fibonacci number can be computed by adding the `n`th and the `n-1`th Fibonacci number. The first few are therefore 1, 1, 1+1=2, 1+2=3, 2+3=5, 3+5=8.
- [x]  Write a function that takes a number and returns a list of its digits. So for `2342` it should return `[2,3,4,2]`.
- [ ]  Write functions that add, subtract, and multiply two numbers in their digit-list representation (and return a new digit list). If you’re ambitious you can implement [Karatsuba multiplication](https://en.wikipedia.org/wiki/Karatsuba_algorithm). Try [different bases](https://en.wikipedia.org/wiki/Radix). What is the best base if you care about speed? If you couldn’t completely solve the prime number exercise above due to the lack of large numbers in your language, you can now use your own library for this task.
- [ ]  Write a function that takes a list of numbers, a starting base `b1` and a target base `b2` and interprets the list as a number in base `b1` and converts it into a number in base `b2` (in the form of a list-of-digits). So for example `[2,1,0]` in base 3 gets converted to base 10 as `[2,1]`.
- [ ]  Implement the following sorting algorithms: (Check Wikipedia for descriptions.)
    - [ ]  Selection sort,
    - [ ]  Insertion sort,
    - [ ]  Merge sort,
    - [ ]  Quick sort,
    - [ ]  Stooge Sort.
- [ ]  Implement binary search.
- [ ]  Write a function that takes a list of strings an prints them, one per line, in a rectangular frame. For example the list ["Hello", "World", "in", "a", "frame"] gets printed as:

    ```jsx
    *********
    * Hello *
    * World *
    * in    *
    * a     *
    * frame *
    *********
    ```

- [x]  Write function that translates a text to Pig Latin and back. English is translated to Pig Latin by taking the first letter of every word, moving it to the end of the word and adding ‘ay’. “The quick brown fox” becomes “Hetay uickqay rownbay oxfay”.

[Largest element in a list](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Largest%20element%20in%20a%20list%2057b9394ea8f84adaa848f9744cad4d9d.md)

[Palindrome](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Palindrome%200ba8e634ae0b4d1f92d01d7871e72459.md)

[Insert element in array](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Insert%20element%20in%20array%20b189f025093f4f3482a1730cbce598d4.md)

[Pig latin](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Pig%20latin%206a445fb126064161b23328a3789b7957.md)

[multiplication table ](Adriann's%20list%200da982edaa0242abb2971994a84c822f/multiplication%20table%20154295e12e744922ac7caa7f31535db5.md)

[Reverse a list in place](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Reverse%20a%20list%20in%20place%20a954016623864a46a31653eeaa2d92f0.md)

[Merge Sorted Array](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Merge%20Sorted%20Array%20c02fb66467e34012b597179d03779a7c.md)

[Duplicate zeros](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Duplicate%20zeros%20ebbf0e3fe7da40cba285cd4e988154bc.md)

[Rotate an Array](Adriann's%20list%200da982edaa0242abb2971994a84c822f/Rotate%20an%20Array%2000cd2ecb3f8c4b4d8e71ffa0a0c77f55.md)