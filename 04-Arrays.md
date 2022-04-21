# Js Array
- It use to store a collection of multiple items into a single variable name
- Resizable and can contain a mix of different data types (String, Objects, Numbers, Boolean)

### Creating Arrays
```javascript
const shopping = ['bread', 'milk', 'cheese', 'hummus', 'noodles'];
console.log(shopping); //['bread', 'milk', 'cheese', 'hummus', 'noodles']
```

### Adding Items
- **`Array.push()`** To add one or more items to the end of an array 

```javascript
const cities = ['Manchester', 'Liverpool'];

cities.push('Cardiff');
console.log(cities);      // [ "Manchester", "Liverpool", "Cardiff" ]

cities.push('Bradford', 'Brighton');
console.log(cities);      // [ "Manchester", "Liverpool", "Cardiff", "Bradford", "Brighton" ]
```
### Removing Items
- **`Array.pop()`** To remove the last item from the array

```javascript
const cities = ['Manchester', 'Liverpool'];
cities.pop();
console.log(cities);     // [ "Manchester" ]
```
### Reverse Items
- **`Array.reverse()`** The first array element becomes the last, and the last array element becomes the first
```javascript
const shopping = ['bread', 'milk', 'cheese', 'hummus', 'noodles'];
cosnt reversedShopping = shopping.reverse()
console.log(reversedShopping); //['noodles', 'hummus', 'cheese', 'milk', 'bread']
```

### Convert `strings` into array
- **`String.split()`** It divides a String into an ordered list of substrings, puts these substrings into an array, and returns the array

```javascript
const data = 'Manchester,London,Liverpool,Birmingham,Leeds,Carlisle';
const cities = data.split(',');

console.log(cities); //['Manchester', 'London', 'Liverpool', 'Birmingham', 'Leeds', 'Carlisle']
```

### Access items by `index`
#### The first element of an array is at index `0`, the second is at index `1`

```javascript
const fruits = ['Apple', 'Banana'];

// The index of an array's first element is always 0.
fruits[0]; // Apple

// The index of an array's second element is always 1.
fruits[1]; // Banana

// The index of an array's last element is always one
// less than the length of the array.
fruits[fruits.length - 1]; // Banana

// Using a index number larger than the array's length
// returns 'undefined'.
fruits[99]; // undefined
```

### Iterate `Array`
- **`for...of`** creates a loop iterating over iterable objects, including: built-in String, Array, array-like objects

```javascript
const iterable = [10, 20, 30];

for (const value of iterable) {
  console.log(value);
}
// 10
// 20
// 30
```

### Spread syntax (`...`)
- Can be used when all elements from an object or array need to be included in a list of some kind.

```javascript
let parts = ['shoulders', 'knees'];
let lyrics = ['head', ...parts, 'and', 'toes'];
//  ["head", "shoulders", "knees", "and", "toes"]
```
- Without spread syntax, to create a new array using an existing method is a combination of `push()`, `splice()`, `concat()`, etc.
- **Spread syntax** is more powerful


#### References
JavaScript Array [click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)


<h3 align="left"><a href="04-Arrays">Prev: Arrays</a></h3>
<h3 align="right"><a href="05-Functions">Next: Functions</a></h3>
