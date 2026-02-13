# JavaScript Learning Guide

## JavaScript Arrays
- An array is a collection of items stored at contiguous memory locations.
- You can store multiple values in a single variable using arrays.

### Example:
```javascript
let fruits = ['apple', 'banana', 'orange'];
```

## JavaScript Objects
- An object is a standalone entity, with properties and type.
- Objects are similar to real-life objects, like a car that has properties like color and model.

### Example:
```javascript
let car = {
  make: 'Toyota',
  model: 'Corolla',
  year: 2020
};
```

## Nested Arrays and Objects
- You can nest arrays and objects inside each other.

### Example:
```javascript
let users = [
  { name: 'Alice', age: 30 },
  { name: 'Bob', age: 25 }
];
```

## Loop Types in JavaScript

### 1. For Loop
```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

### 2. While Loop
```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

### 3. Do-While Loop
```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

### 4. For-In Loop
- To loop through the properties of an object.

```javascript
let car = { make: 'Toyota', model: 'Corolla' };
for (let key in car) {
  console.log(key + ': ' + car[key]);
}
```

### 5. For-Of Loop
- To loop through iterable objects (arrays, strings).

```javascript
let fruits = ['apple', 'banana', 'orange'];
for (let fruit of fruits) {
  console.log(fruit);
}
```

### 6. forEach Method
```javascript
let numbers = [1, 2, 3];
numbers.forEach(function(number) {
  console.log(number);
});
```

### 7. Map Method
- Creates a new array populated with the results of calling a provided function on every element.

```javascript
let numbers = [1, 2, 3];
let doubled = numbers.map(number => number * 2);
```

### 8. Filter Method
- Creates a new array with all elements that pass the test implemented by the provided function.

```javascript
let numbers = [1, 2, 3, 4];
let evens = numbers.filter(number => number % 2 === 0);
```

### 9. Find Method
- Returns the value of the first element that satisfies the provided testing function.

```javascript
let numbers = [1, 2, 3, 4];
let found = numbers.find(number => number > 2);
```

### 10. Reduce Method
- Executes a reducer function on each element of the array, resulting in a single output value.

```javascript
let numbers = [1, 2, 3, 4];
let sum = numbers.reduce((accumulator, current) => accumulator + current);
```

## Practice Tasks
1. Create an array of 10 random numbers and find their sum using the reduce method.
2. Create an object to represent a book and loop through its properties using a for-in loop.
3. Use the filter method to create a new array from an existing array of numbers that contains only even numbers.
