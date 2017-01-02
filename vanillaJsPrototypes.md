# Vanilla JavaScript Prototypes

## A condensed list of JS Prototypes with brief description, syntax and simple example.
---
### Filter Array Prototypes
---

* **.forEach()**  executes a provided function once for each array element.
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
