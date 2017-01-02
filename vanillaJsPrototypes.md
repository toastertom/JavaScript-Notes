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
