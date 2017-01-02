# Vanilla JavaScript Prototypes

## A condensed list of JS Prototypes with brief description, syntax and simple example.

---
### Filter Arrays

***.forEach()***
Executes a provided function once for each array element.
####Syntax
```
array.forEach(callback, thisArg)
```
####example
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
