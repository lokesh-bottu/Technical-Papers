# Introduction
- JavaScript is a versatile and widely-used programming language primarily known for its role in web development. 
- It empowers developers with various tools and concepts to manipulate data and create interactive web applications. 

## Loops


### for Loop

```html 
for (let i = 0; i < 5; i++) {
    console.log(i);
}

```

### forEach

```html 

const array = [1, 2, 3];
array.forEach(item => {
    console.log(item);
});
```

### for..in

```html
const person = { name: "John", age: 30 };
for (const key in person) {
    console.log(key, person[key]);
}
```




### for..of


```html
const iterable = [1, 2, 3];
for (const value of iterable) {
    console.log(value);
}
```


### while Loop

```html
let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}
```



## Mutable and Immutable Methods

In JavaScript, strings and arrays have both mutable and immutable methods.

### Mutable Methods
```html

let mutableArray = [1, 2, 3];
mutableArray.push(4);  // Modifies the array in-place

let mutableString = "Hello";
mutableString += " World";  // Modifies the string in-place
```


### Immutable Methods

```html
const immutableArray = [1, 2, 3];
const newArray = immutableArray.concat(4);  // Creates a new array

const immutableString = "Hello";
const newString = immutableString.concat(" World");  // Creates a new string
```


## Pass by Reference and Pass by Value
JavaScript uses both pass by reference and pass by value, depending on the data type.

### Pass by Value

```html
let a = 10;
let b = a;  // a is passed by value, and b is a copy of a

```
### Pass by Reference

```html
const originalArray = [1, 2, 3];
const newArray = originalArray;  // Both point to the same array in memory
```


## Array Methods


### Array.pop

```html
const array = [1, 2, 3];
const poppedValue = array.pop();  // Removes and returns the last element

```
### Array.push

```const array = [1, 2, 3];
array.push(4);  // Appends an element to the end

```




### Array.splice

```const array = [1, 2, 3];
const slicedArray = array.slice(1, 2);  // Returns a new array with selected elements
```


### Array.includes

```const array = [10, 20, 30, 40];
const hasValue = array.includes(30);  // Checks if an element is present
```


```const array = [1, 2, 3];
array.forEach(item => {
    console.log(item);
});
```


## Higher Order Functions

### Array.forEach
```
const array = [1, 2, 3];
array.forEach(item => {
    console.log(item);
});
```

### Array.filter

```const numbers = [10, 20, 30, 40];
const filteredNumbers = numbers.filter(num => num > 25);

```
### Array.map

```const array = [1, 2, 3];
const mappedArray = array.map(item => item * 2);
```

### Array.reduce

```const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((accumulator, current) => accumulator + current, 0);

```


Scopes
JavaScript has function and block scopes.

```
function scopeExample() {
    var x = 10;  // Scoped to the function
}

{
    let y = 20;  // Scoped to the block
}
```