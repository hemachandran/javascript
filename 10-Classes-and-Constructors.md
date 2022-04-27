# Constructors
- Using an object literals metod is fine to create one object, but if we needs to create more than one what is the best method? **`Constructors`**
- A constructor is just a function called using the **`new`** keyword

**Example**
```javascript
function createPerson(name) {
  const obj = {};
  obj.name = name;
  obj.introduceSelf = function() {
    console.log(`Hi! I'm ${this.name}.`);
  }
  return obj;
}

const salva = createPerson('Salva');
salva.name; //Salva
salva.introduceSelf(); //Hi! I'm Salva

const frankie = createPerson('Frankie');
frankie.name; //Frankie
frankie.introduceSelf(); //Hi! I'm Frankie
```

**This way we can create Objects using `Constructors` and highly usefull when having complex application data**

# Class
- The class declaration creates a new class with a given name using prototype-based (inherit features from one another) inheritance

**Example of Js Class**
```javascript
class Person {
  name;

  constructor(name) {
    this.name = name;
  }

  introduceSelf() {
    console.log(`Hi! I'm ${this.name}`);
  }
}
```

### Inheritance
- Inherit a feature/object from one to another using keyword of `extend`

**Example of Class Inheritance**
```javascript
class Professor extends Person {
  teaches;

  constructor(name, teaches) {
    super(name);
    this.teaches = teaches;
  }

  introduceSelf() {
    console.log(`My name is ${this.name}, and I will be your ${this.teaches} professor.`);
  }

  grade(paper) {
    const grade = Math.floor(Math.random() * (5 - 1) + 1);
    console.log(grade);
  }
}
```
- The `Professor` class adds a new property `teaches`
- The `super` keyword is used to access and call functions on an object's parent.

### Private methods
```javascript
class Example {

  somePublicMethod() {
    this.#somePrivateMethod();
  }
  #somePrivateMethod() {
    console.log('You called me?');
  }
}

const myExample = new Example();

myExample.somePublicMethod(); // 'You called me?'
myExample.#somePrivateMethod(); // SyntaxError
```

### References
- Javascript Constrcutor - [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/constructor)
- Javascript Class - [Click here](developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/class)

