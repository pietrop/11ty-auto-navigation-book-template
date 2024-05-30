# % Remainder

> Ask any C# or JavaScript programmer what is the modulo operator in their language and there is a big chance that they’ll gone answer: % (e.g. the percentage sign). Plenty of documentation refer to the % sign as modulo operator.

Wow! This is a subtle but very dangerous mistake. In C# and JavaScript % operator is used actually to calculate the remainder (with sign) left over when one operand is divided by the second operand. Therefore the operand should be correctly referred to as the signed remainder operator.

At first sight the signed remainder operator functions similarly to the modulo operator. Let’s do some tests by comparing the results returned by JavaScript with the ones returned by Google.

Well … this shouldn’t be actually a surprise if we look at the definition of % operator in JavaScript (… or even C# or many other languages). Google calculates the true modulo, while these computer languages calculate a signed reminder.

from 

[Code Avenger](https://www.codeavenger.com/2017/05/19/JavaScript-Modulo-operation-and-the-Caesar-Cipher.html)

> The remainder operator (%) returns the remainder left over when one operand is divided by a second operand. It always takes the sign of the dividend.

> Note that while in most languages, ‘%’ is a remainder operator, in some (e.g. [Python, Perl](https://en.wikipedia.org/wiki/Modulo_operation#In_programming_languages)) it is a modulo operator. For positive values, the two are equivalent, but when the dividend and divisor are of different signs, they give different results. To obtain a modulo in JavaScript, in place of a % n, use ((a % n ) + n ) % n.

[Remainder (%) - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Remainder)