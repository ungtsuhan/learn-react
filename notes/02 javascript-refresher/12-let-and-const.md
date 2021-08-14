# Let and Const

`let` and `const` is used to declare variable

- `let`: used to declare a variable (can be reassigned)

- `const`: used to decalre a constant variable (cannot be reassigned)

## Example

Can assigned to variable declared using `let` keyword

```js
let myName = 'Max';
console.log(myName); // Max
myName = 'Bob';
console.log(myName); // Bob
```

Error is throwed when reassigned a constant variable

```js
const myName = 'Max';
console.log(myName); // Max
myName = 'Bob'; // TypeError: invalid assignment to const
console.log(myName); 
```

## Additional information

- `var` is globally scoped while `let` is blocked scoped
