# Js Array
- It use to store a collection of multiple items into a single variable name
- Resizable and can contain a mix of different data types (String, Objects, Numbers, Boolean)

### Creating Arrays
```javascript
const shopping = ['bread', 'milk', 'cheese', 'hummus', 'noodles'];
console.log(shopping); //['bread', 'milk', 'cheese', 'hummus', 'noodles']
```
### The first element of an array is at index `0`, the second is at index `1`

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
