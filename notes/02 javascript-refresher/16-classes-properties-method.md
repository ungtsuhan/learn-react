# Classes, Properties and Method

## ES7 way of properties declaration

Traditional way:

```js
constructor() {
    this.myProperty = 'value'
}
```

New way:

- can remove constructor function

- and declare without `this` keyword

- also dont need to call `super` to inherit function

```js
myProperty = 'value'
```

## ES7 way of method declaration

Traditional way:

```js
myMethod() {
}
```

New way:

- use arrow function

```js
myMethod = () => {/*...*/}
```

## Example

```js
class Master {
    gender = 'male';

    printGender = () => {
        console.log(this.gender)
    }
}

class Person extends Master {
    name = 'Max';
    
    printMyName = () => {
        console.log(this.name);
    }
}
const person = new Person();
person.printMyName();
person.printGender();
```