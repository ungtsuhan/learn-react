# Refrence and Primitive Types

## Primitive Type

number, string, boolean etc is a primitive type.

When reassign priitive type to a new variable, it will copy the value

```js
const number = 1; // is a primitive type
const num2 = number;

console.log(num2); // 1
```

## Reference Type

Object and Array are reference types.

When assign object to new object, it does not copy the object!

It just copy the pointer!

So if you change the old object value, the value of new object also changed as it is just a pointer to old object!

```js
const person = {
    name: 'Max'
};
const secondPerson = person;
console.log(secondPerson); // {name: "Max"}
person.name = 'Manu';
console.log(secondPerson); // {name: "Manu"}
```

If you want to copy in immutable way, use spread operator!

```js
const person = {
    name: 'Max'
};
const secondPerson = {...person}; // use spread operator to copy object instead of pointer
console.log(secondPerson); // {name: "Max"}
person.name = 'Manu'; 
console.log(secondPerson); // {name: "Max"}
```