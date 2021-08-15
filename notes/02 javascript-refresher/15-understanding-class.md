# Understanding Class

- Class is blueprint of object

- Class can have properties and method

- Class can inherit from other class

```js
class Person {
    let name = 'Max'; // Property
    call = () => {/**/}; //Method
}
```

## How to use class

```js
const myPerson = new Person(); //instantiate an instance of object of class Person
myPerson.call(); // call its method
console.log(myPerson.name); // access and get its property
```

### Example

```js
// Define class
class Person {
    constructor() {
        this.name = 'Max';
    }
    printMyName() {
        console.log(this.name);
    }
}

const person = new Person();
person.printMyName(); // Max
```

## Inheritance

```js
class Person extends Master {} // Person inherit from Master
```
**Note**: to allow execute the derived class constructor, need to call `super()` method in constructor of inherited class

### Example

```js
class Master {
    constructor() {
        this.gender = 'male';
    }

    printGender() {
        console.log(this.gender)
    }
}

class Person extends Master {
    constructor() {
        super(); // to allow execute the derived class constructor
        this.name = 'Max';
    }
    printMyName() {
        console.log(this.name);
    }
}
const person = new Person();
person.printMyName(); // Max
person.printGender(); // male (we can also call method of the inherited function)
```