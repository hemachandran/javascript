# Js Objects
- It is used to store various keyed collections and more complex entities
- Represents key-value pair structure

### Create an Object

```javascript
const person = {
  name: ['Bob', 'Smith'],
  age: 32
};
```

### Nested Objects

```javascript
const person = {
  name: {
    firstName: 'Bob',
    lastName: 'Sfffmith',
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
