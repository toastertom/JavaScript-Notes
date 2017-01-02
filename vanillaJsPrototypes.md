# Vanilla JavaScript Prototypes

## A condensed list of JS Prototypes with brief description, syntax and simple example.
---
### Filter Array Prototypes
---
**.filter()** creates a new array with all elements that pass the test implemented by the provided function.
####syntax
```
var newArray = array.filter(callback [, thisArg])
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
var newArray = array.map(callback [, thisArg])
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
**.sort()** sorts the elements of an array in place and returns the array. The sort is not necessarily stable. the default sort order is according to string Unicode code points.
####Syntax
```
array.sort()
array.sort(compareFunction)
```
####Example
```
var fruit = ['cherries', 'apples', 'bananas'];
fruit.sort();

//Results = ['apples', 'bananas', 'cherries']

var things = ['word', 'Word', '1 Word', '2 Words'];
things.sort();

//Results = ['1 Word', '2 Words', 'Word', 'word']
//In Unicode, numbers come before uppercase letters, which come before lower case letters.
```
---
**.reduce()** applies a function against an accumulator and each value of the array (from left-to-right) to reduce it to a single value.
####Syntax
```
array.reduce(callback, [initialValue])
```
####Example
```
var sum = [0, 1, 2, 3];
sum.reduce(function(a, b){
  return a + b;
}, 0);

//sum is 6
```
---
**.forEach()**  
####Syntax
```

```
####Example
```

```
---
Test Elements In Array
---

**.forEach()**  executes a provided function once for each array element.
####Syntax
```
array.forEach(callback [, thisArg])
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

**.every()**  tests whether ***all elements*** in the array pass the test implemented by the provided function.
####Syntax
```
array.every(callback  [, thisArg])
```
####Example
```
var array1 = [12, 5, 8 ,130, 44];
var array2 = [12, 54, 18, 130, 44];

function isBigEnough(element, index, array) {
  return element >= 10;
}

array1.every(isBigEnough); // false
array2.every(isBigEnough); // true
```
---

**.some()** tests whether ***some elements*** in the array passes the test implemented by the provided function.
####Syntax
```
array.some(callback  [, thisArg])
```
####Example
```
var array1 = [2, 5 , 8, 1, 4];
var array2 = [12, 5, 8, 1, 4];

function isBiggerThan10(element, index, array) {
  return element >= 10;
}

array1.some(isBiggerThan10); // false
array2.some(isBiggerThan10); // true
```
---
**.find()** returns a ***value*** of the ***first element*** in the  array that satisfies the provided testing function. Otherwise undefined is returned.
####Syntax
```
array.find(callback [, thisArg])
```
####Example
```
var array1 = [12, 5, 130, 1, 4];

function isBigEnough(element) {
  return element >= 15;
}

array1.find(isBigEnough); //Value is 130
```
---
