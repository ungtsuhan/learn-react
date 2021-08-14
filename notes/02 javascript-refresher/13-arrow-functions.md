# Arrow Functions

Different syntax to create javascript function

Normal function:

```js
function myFnc() {
    //...
}
```

Arrow function:

```js
const myFnc = () => {
    //...
}
```

## Example 1

Normal Function

```js
const printMyName = (name) => {
    console.log(name);
}
printMyName('Max');
```

Arrow Function
```js
const printMyName = name => {
    console.log(name);
}
printMyName('Max');
```

## Example 2

Arrow Function

```js
const mutiply = (number) => {
    return number* 2;
}
console.log(multiply(2));
```

Simplified Arrow Function (if only have one line with `return` inside parentheses)

- remove curly braces
- remove `return` keyword

```js
const mutiply = (number) => number * 2;
console.log(multiply(2));
```

## Why use arrow functions

1. shorter, since function keyword is not required

2. no more issue with the `this` keyword!
