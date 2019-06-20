> begin [the debugging exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/debugging) and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD)  (wrong exercises, correct markdown styling)

## 1. Use the JavaScript Console to Check the Value of a Variable
```js
let a = 5;
let b = 1;
a++;
// Add your code below this line

console.log(a); // 6
let sumAB = a + b;
console.log(sumAB); // 7
```

## 2. Understanding the Differences between the freeCodeCamp and Browser Console
```js
// Open your browser console
let outputTwo = "This will print to the browser console 2 times";
// Use console.log() to print the outputTwo variable

console.log(outputTwo); ** did not print two times !!!

let outputOne = "Try to get this to log only once to the browser console";
// Use console.clear() in the next line to print the outputOne only once
console.clear();
// Use console.log() to print the outputOne variable
console.log(outputOne);
```

## 3. Use typeof to Check the Type of a Variable
```js
let seven = 7;
let three = "3";
console.log(seven + three);         //73
// Add your code below this line
console.log(typeof seven);          //number
console.log(typeof three);          //string
console.log(typeof (seven+three));  //string
```
