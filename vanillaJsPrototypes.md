# Vanilla JavaScript Prototypes

## A condensed list of JS Prototypes with brief description, syntax and simple example.
---
### Filter Array Prototypes
---

**.forEach()**  executes a provided function once for each array element.
####Syntax
```
array.forEach(callback, thisArg)
```
####Example
```
var a = ["a", "b", "c"];

a.forEach(function(element) {
  console.log(element)
});
// Result
// a
// b
// c
```
---
**.Filter()** creates a new array with all elements that pass the test implemented by the provided function.
####syntax
```
var newArray = array.filter(callback, thisArg)
```
####Example
```
var array1 = [12, 5, 8, 130, 44];

function isBigEnough(value) {
  return value >= 10;
}

var filtered = array1.filter(isBigEnough);
//filtered = [12, 130, 44]
```
---
**.map()** creates a new array with the results of calling a provided function on every element in this array.
####Syntax
```
var newArray = array.map(callback, thisArg)
```
####Example
```
var numbers = [1, 5, 10, 15];
var roots = numbers.map(function(x){
  return x * 2;
    });
    //roots is now [2, 10, 20, 30]
    //numbers stays the same

var numbers = [1, 4, 9];
var roots = numbers.map(Math.sqrt);
//roots is now [1, 2, 3]
//numbers stays the same
```
---
