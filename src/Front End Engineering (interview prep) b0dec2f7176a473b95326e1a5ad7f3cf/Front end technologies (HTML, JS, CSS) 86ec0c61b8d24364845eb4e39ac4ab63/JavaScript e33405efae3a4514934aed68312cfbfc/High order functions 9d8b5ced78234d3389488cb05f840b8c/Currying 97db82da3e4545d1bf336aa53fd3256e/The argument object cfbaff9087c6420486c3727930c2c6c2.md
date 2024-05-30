# The argument object

Default argument name, useful when currying. 

## Option 1. `arguments`

[The arguments object - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)

[Rest parameters and spread syntax](https://javascript.info/rest-parameters-spread#the-arguments-variable)

The “arguments” variable

```jsx
function test( ) {
		// arguments gives you access to the 
		// you can access it as an array but it's not an array
		// altho you can convert it into an array
    console.log('arguments', arguments );
}

```

To convert `arguments` to array you can do 

```jsx
Array.from(arguments)
```

or 

```jsx
const newList = [...arguments]
```

## Option 2. Rest parameters / Spread operator

ES6 more recent way to do option 1.

[Rest parameters - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters)

[Rest parameters and spread syntax](https://javascript.info/rest-parameters-spread)

Rest parameters `...`

```jsx
function test(...args) {
	// using spread operator, converts default arguments it into an array 
	// altho `args` could be named anything
  console.log('args', args );
}
```

you can also do 

```jsx
function test(one,...args) {
	// you can also add it as last argument to catch 
	// anything else that has been passed extra 
  console.log('args', args );
}
```