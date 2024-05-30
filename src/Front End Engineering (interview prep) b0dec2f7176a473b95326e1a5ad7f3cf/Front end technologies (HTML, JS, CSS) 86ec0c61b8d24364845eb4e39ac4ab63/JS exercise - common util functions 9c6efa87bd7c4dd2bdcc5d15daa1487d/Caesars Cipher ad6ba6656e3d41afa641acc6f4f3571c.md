# Caesars Cipher

```jsx
// Using modulus operator; makes the sentence uppercase;
function cipherRot13(str) {
  str = str.toUpperCase();
  return str.replace(/[A-Z]/g, rot13);

  function rot13(correspondance) {
    const charCode = correspondance.charCodeAt();
    //A = 65, Z = 90
    return String.fromCharCode(
            ((charCode + 13) <= 90) ? charCode + 13
                                    : (charCode + 13) % 90 + 64
           );
    
  }
}
```

[Caesar Cipher in Javascript](https://stackoverflow.com/questions/44232645/caesar-cipher-in-javascript#:~:text=%22A%20common%20modern%20use%20is,and%20returns%20a%20decoded%20string.%22)

[Code Avenger](https://www.codeavenger.com/2017/05/19/JavaScript-Modulo-operation-and-the-Caesar-Cipher.html)