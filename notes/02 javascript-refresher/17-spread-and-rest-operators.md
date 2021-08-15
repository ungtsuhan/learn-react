# Spread and Rest Operators

Spread and Rest Operator use 3 dots `...`

## Spread 

- used to split up array elements OR object properties

- Three dot in front of array will pull out all element and add to new array

```js
const newArray = [...oldArray, 1 , 2];
```

- Three dot in front of object will pull out all properties and add to new object

- If old object have new property, it will overwrite with new property 

```js
const newObject = {...oldObject, newProp: 5};
```

### Examples:

```js
const numbers = [1, 2, 3];
const newNumbers = [...numbers, 4];
console.log(newNumbers);
```

```js
const person {
    name: 'Max'
}

const newPerson = {
    ...person,
    age: 28
}

console.log(newPerson);

// Result
// {
//     name: 'Max',
//     age: 28 
// }
```
## Rest

- used to merge a list of function arguments into an array

```js
function sortArgs(...args) {
    return args.sort();
}
```

### Examples

```js
const filter = (...args) => {
    return args.filter(el => el === 1);
}
console.log(filter(1,2,3)); // [1]
```

**Notes**: `===` check for type and value