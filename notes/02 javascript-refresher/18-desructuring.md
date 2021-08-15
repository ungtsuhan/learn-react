# Destructuring

Easily extract array elements or object properties and store them in variables

## Array Destructing

use square bracket at left side to get value of array and assign to variable 

```js
[a, b] = ['Hello', 'Max']
console.log(a); // Hello
console.log(b); // Max
```

### Examples

```js
const numbers = [1, 2, 3];
[num1, num2] = numbers;
console.log(num1, num2); // 1 // 2

[num1, ,num3] = numbers;
console.log(num1, num3); // 1 // 3
```

## Object Destructing

use curly brace at left side and specify the target property to be pull out from right side

```js
{name} = {name: 'Max', age: 28};
console.log(name); //Max
console.log(age); // undefined
```