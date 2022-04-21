# Js Objects
- A JavaScript object literal is a comma-separated list of **`name-value`** pairs wrapped in curly braces. 

### Things to Remember
- A property name that has a space or a hyphen, or that starts with a number) can only be accessed using the square bracket notation
- Each property name before colons is an identifier


### Create an Object
1. By object literal
2. By object instance
3. By object constructor

```javascript
//Object literal
const person = {
  name: ['Bob', 'Smith'],
  age: 32
};

//Object instance
var emp = new Object();
emp.id=101:
emp.name="Ravi Malik";
emp.salary=50000;

//Object constructor
let o = new Object()
o.foo = 42

console.log(o);
// Object { foo: 42 }

```

### Nested Objects

```javascript
const person = {
  name: {
    firstName: 'Bob',
    lastName: 'Smith',
  },
  age: 32
};

person.name.firstName; //"Bob"
```

### Accessing the object
- By using **dot** and **brackets** notation

```javascript
person.name.firstName; //Bob
person['name']['firstName']: //Bob
```

### Update Object Properties
```javascript
person.age = 45;
person.name.lastName = 'Robert';
```

### Adding New Object Property
```javascript
person['eyes'] = 'hazel';
person.hairColor = 'brown';
```
### Deleting Items
```javascript
delete person.age;
```
### Object Methods
```javascript
const person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};

// `this` refers to person object
```
#### `this`
- It is a keyword. Cannot change the value
- `this` refers to global objects in both inside and outside of a function
- In object, this refers to object properties
