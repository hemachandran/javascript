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
//Object Literal
const person = {
  name: ['Bob', 'Smith'],
  age: 32
};

//Object instance
var emp = new Object();
emp.id=101:
emp.name="Ravi Malik";
emp.salary=50000;
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
