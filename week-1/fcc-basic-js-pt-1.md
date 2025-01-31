> complete [the basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) through _Counting Cards_ & paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 

## 1. Comment Your Code
```js
// for one line comments //
/* for multiple
line comments */ 
```

## 2. Declare Variables
```js
var myName; 
>> value of myName is undefined
```
## 3. Storing Values with the Assignment Operator

```js
a = 7;
b = a;
```
## 4. Initializing Variables with the Assignment Operator
```js
var a=9;
```
## 5. Understanding Uninitialized Variables
```js
a =5;
b=10;
c="I am a";
Result:
a=6 b=15 c=I am a String!
```
## 6. Understanding Case Sensitivity in Variables
```js
// Declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Assignments
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;

if the dec and asg do not match, then both will be regarded as two different vars. 
```

## 7. Add Two Numbers with JavaScript
```js
var sum = 10 + 10;
```

## 8. Subtract One Number from Another with JavaScript
```js
var difference = 45 - 33;
```
## 9. Multiply Two Numbers with JavaScript
```js
var product = 8 * 10;
```

## 10. Divide One Number by Another with JavaScript
```js
var quotient = 66 / 33;
if the division is not a whole, also gives out results with decimals
```

## 11. Increment a Number with JavaScript
```js
myVar++;
```

## 12. Decrement a Number with JavaScript
```js
myVar --;
```

## 13. Create Decimal Numbers with JavaScript
```js
var myDecimal = 2.5;
```

## 14. Multiply Two Decimals with JavaScript
```js
var product = 2.0 * 2.5;
```
## 15. Divide One Decimal by Another with JavaScript
```js
var quotient = 4.4 / 2.0;
```
## 16. Finding a Remainder in JavaScript
```js
var remainder;
remainder = 11 % 3;
remainder is assigned 2
```

## 17. Compound Assignment With Augmented Addition
```js
a+=12;
b+=9;
c+= 7;

console.log(a,b,c); 15, 26, 19
```
## 18. Compound Assignment With Augmented Subtraction
```js
a -= 6;
b -= 15;
c -= 1;

console.log(a,b,c); 5,-6,2
```
## 19. Compound Assignment With Augmented Multiplication
```js
a *= 5;
b *= 3;
c *= 10;
```
## 20. Compound Assignment With Augmented Division
```js
a /= 12;
b /= 4;
c /= 11;
```
## 21. Declare String Variables
```js
var myFirstName = "saliha"
var myLastName = "yaylaci"
```
## 22. Escaping Literal Quotes in Strings
```js
myStr = "I am a \"double quoted\" string inside \"double quotes\"."
```
## 23.Quoting Strings with Single Quotes
```js
var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```
## 24. Escape Sequences in Strings
```js
var myStr = "FirstLine\n\t\\SecondLine\nThirdLine"
\'	single quote
\"	double quote
\\	backslash
\n	newline
\r	carriage return
\t	tab
\b	backspace
\f	form feed
```
## 25. Concatenating Strings with Plus Operator
```js
myStr = "This is the start. " + "This is the end.";
console.log(myStr); == This is the start. This is the end.
```
## 26. Concatenating Strings with the Plus Equals Operator
```js
var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
console.log(myStr); == This is the first sentence. This is the second sentence.
```
## 27. Constructing Strings with Variables
```js
var myName = "saliha"
var myStr = "I am " + myName + "!"
console.log(myStr); == I am saliha!
```
## 28. Appending Variables to Strings
```js
var someAdjective = "makkelijk"
var myStr = "Learning to code is ";
myStr+=someAdjective;
console.log(myStr); == Learning to code is makkelijk
```
## 29. Find the Length of a String
```js
lastNameLength = lastName.length;
```
## 30. Use Bracket Notation to Find the First Character in a String
```js
Zero-based indexing.
firstLetterOfLastName = lastName[0]; -> gets the first letter
```
## 31. Understand String Immutability
```js
myStr = "Hello World";
```
## 32. Use Bracket Notation to Find the Nth Character in a String
```js
var thirdLetterOfLastName = lastName[2];
```
## 33. Use Bracket Notation to Find the Last Character in a String
```js
var lastLetterOfLastName = lastName[lastName.length - 1];
```
## 34. Use Bracket Notation to Find the Nth-to-Last Character in a String
```js
var secondToLastLetterOfLastName = lastName[lastName.length - 2];
```
## 35. Word Blanks
```js
var result =  myAdjective + " " + myNoun + " " + myVerb + " " + myAdverb;
var str = wordBlanks("dog", "big", "ran", "quickly");
console.log(str) == big dog ran quickly
```
## 36. Store Multiple Values in one Variable using JavaScript Arrays
```js
var myArray = ["aa",2];
var s = myArray[0]; == "aa"

```
## 37. Nest one Array within Another Array
```js
var myArray = [["a",1],["b",2]];
var s = myArray[0][0]; == "a"
```
## 38. Access Array Data with Indexes
```js
var myData = myArray[0];
```
## 39. Modify Array Data With Indexes
```js
myArray[0] = 45;
```
## 40. Access Multi-Dimensional Arrays With Indexes
```js
var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];
var myData = myArray[2][1]; == 8
```
## 41. Manipulate Arrays With push()
```js
adds to end
myArray.push(["dog",3]);
```
## 42. Manipulate Arrays With pop()
```js
removes from end
var removedFromMyArray = myArray.pop();
console.log(removedFromMyArray); == [cat,2]
```
## 43. Manipulate Arrays With shift()
```js
removes from start
var removedFromMyArray = myArray.shift();
console.log(removedFromMyArray); == [John,23]

```
## 44. Manipulate Arrays With unshift()
```js
adds to start
myArray.unshift(["Paul",35]);
console.log(myArray); == Paul,35,dog,3

```
## 45. Shopping List
```js
var myList = [["tomato",2],["choco", 3],["lemon", 3],["berry", 6],["ice",6]];
```
## 46. Write Reusable JavaScript with Functions
```js
function reusableFunction(){
    console.log("Hi World");
}
reusableFunction();
```
## 47. Passing Values to Functions with Arguments
```js
function functionWithArgs (a,b){
  console.log(a+b);
}
functionWithArgs(9,8); == 17
```
## 48. Global Scope and Functions
```js
var myGlobal = 10

function fun1() {
  oopsGlobal = 5 
}                 // myGlobal = 10 fun1()-> oopsGlobal thus no reference error

but

oopsGlobal =5 // ReferenceError: oopsGlobal is not defined
```
## 49. Local Scope and Functions
```js
function myLocalScope() {
  var myVar = 'use strict'; // you shouldn't need to edit this line
  
  console.log(myVar);
}
myLocalScope();
//deleted console.log(myVar); defined outside the function
```
## 50. Global vs. Local Scope in Functions
```js
// Setup
var outerWear = "T-Shirt";

function myOutfit() {
  // Only change code below this line
  
  outerWear = "sweater"
  
  // Only change code above this line
  return outerWear;
}
```
## 51. Return a Value from a Function with Return
```js
function timesFive(num){
  return num*5;
}
console.log(timesFive(4)); == 20
```
## 52. Understanding Undefined Value returned from a Function
```js
function addFive() {
  sum +=5;
}
var returnedValue = addFive();
 // sum=5 returnedValue=undefined
```
## 53. Assignment with a Returned Value
```js
function processArg(num) {
  return (num + 3) / 5;
}
processed = processArg(7);
console.log(processed); == 2
```
## 54. Stand in Line
```js
function nextInLine(arr, item) {
  // Your code here
  arr.push(item);
  return arr.shift();
}

// Test Setup
var testArr = [1,2,3,4,5];

// Display Code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6)); // Modify this line to test
console.log("After: " + JSON.stringify(testArr));
--- 
Before: [1,2,3,4,5]
1
After: [2,3,4,5,6]
```
## 55. Understanding Boolean Values
```js
function welcomeToBooleans() {
return true; 
}
```
## 56. Use Conditional Logic with If Statements
```js
function trueOrFalse(wasThatTrue) {
    if(wasThatTrue) {
        return "Yes, that was true"
    }
    return "No, that was false"

}
console.log(trueOrFalse(true)); == Yes, that was true
console.log(trueOrFalse(false)); == No, that was false
```
## 57. Comparison with the Equality Operator
```js
function testEqual(val) {
  if (val==12) { 
    return "Equal";
  }
  return "Not Equal";
}
console.log(testEqual(10)); == Not Equal
console.log(testEqual(12)); == Equal
```
## 58. Comparison with the Strict Equality Operator
```js
function testStrict(val) {
  if (val === 7) { 
    return "Equal";
  }
  return "Not Equal";
}
console.log(testStrict(7)); == Equal
console.log(testStrict('7')); == Not Equal
```
## 59. Practice comparing different values
```js
function compareEquality(a, b) {
  if (a === b) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}
```
## 60. Comparison with the Inequality Operator
```js
function testNotEqual(val) {
  if (val != 99 ) { // Change this line
    return "Not Equal";
  }
  return "Equal";
}
```
## 61. Comparison with the Strict Inequality Operator
```js
function testStrictNotEqual(val) {
  // Only Change Code Below this Line
  
  if (val !== 17) {

  // Only Change Code Above this Line

    return "Not Equal";
  }
  return "Equal";
}
```
## 62. Comparison with the Greater Than Operator
```js
function testGreaterThan(val) {
  if (val > 100) {  // Change this line
    return "Over 100";
  }
  
  if (val > 10) {  // Change this line
    return "Over 10";
  }

  return "10 or Under";
}
```
## 63. Comparison with the Greater Than Or Equal To Operator
```js
function testGreaterOrEqual(val) {
  if (val >= 20) {  // Change this line
    return "20 or Over";
  }
  
  if (val >= 10) {  // Change this line
    return "10 or Over";
  }

  return "Less than 10";
}
```
## 64. Comparison with the Less Than Operator
```js
function testLessThan(val) {
  if (val < 25) {  // Change this line
    return "Under 25";
  }
  
  if (val < 55) {  // Change this line
    return "Under 55";
  }

  return "55 or Over";
}

```
## 65. Comparison with the Less Than Or Equal To Operator
```js
function testLessOrEqual(val) {
  if (val <= 12 ) {  // Change this line
    return "Smaller Than or Equal to 12";
  }
  
  if (val <= 24) {  // Change this line
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}
```
## 66. Comparisons with the Logical And Operator
```js
 if (val <= 50 && val >= 25) {
      return "Yes";
    }
```
## 67. Comparisons with the Logical Or Operator
```js
if (val < 10 || val > 20) {
    return "Outside";
  }
```
## 68. Introducing Else Statements
```js
 if (val > 5) {
    result = "Bigger than 5";
  }
  else {
    result = "5 or Smaller";
  }
```
## 69.  Introducing Else If Statements
```js
 if (val > 10) {
    return "Greater than 10";
  }
  
  else if (val < 5) {
    return "Smaller than 5";
  }
  
  else {return "Between 5 and 10";}
}
```
## 70. Logical Order in If Else Statements
```js
if (val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
```
## 71. Chaining If Else Statements
```js
if(num < 5)
  return "Tiny";
  else if (num < 10)
  return "Small";
  else if (num < 15)
  return "Medium";
  else if (num < 20)
  return "Large";
  else 
  return "Huge";
```
## 72. Golf Code
```js
var names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];
function golfScore(par, strokes) {
  if(strokes == 1)
  return names[0];
  else if (strokes <= par-2)
  return names[1];
  else if (strokes == par -1)
  return names[2];
  else if (strokes == par)
  return names[3];
  else if (strokes == par +1)
  return names[4];
  else if (strokes == par +2)
  return names[5];
  else if (strokes >= par +3)
  return names[6];
}
```
## 73. Selecting from Many Options with Switch Statements
```js
switch(val){
    case 1:
      answer = "alpha";
      break;
    case 2:
      answer = "beta";
      break;
    case 3:
      answer = "gamma";
      break;
    case 4:
      answer = "delta";
      break;
  
}
```
## 74. Adding a Default Option in Switch Statements
```js
switch(val){
    case "a":
      answer = "apple";
      break;
    case "b":
      answer = "bird";
      break;
    case "c":
      answer = "cat";
      break;
    default:
      answer = "stuff";
      break;
  }
```
## 75. Multiple Identical Options in Switch Statements
```js
 switch (val) {
    case 1:
    case 2:
    case 3:
      answer = "Low";
      break;
    case 4:
    case 5:
    case 6:
      answer = "Mid";
      break;
    case 7:
    case 8:
    case 9:
      answer = "High";
      break;
  }
```

## 76. Replacing If Else Chains with Switch
```js
 switch (val){
    case "bob":
      answer = "Marley";
      break;
    case 42:
     answer = "The Answer";
    break;
    case 1:
    answer = "There is no #1";
    break;
    case 99:
     answer = "Missed me by this much!";
    break;
    case 7:
     answer = "Ate Nine";
    break;
  }
```

## 77. Returning Boolean Values from Functions
```js
function isLess(a, b) {
 return a<b;
}
```

## 78. Return Early Pattern for Functions
```js
if (a < 0 || b < 0)
    return undefined;
```

## 79. Counting Cards
```js
switch(card){
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      count+= 1;
      if (count > 0)
        return count + " Bet";
      else
        return count + " Hold";
    case 7:
    case 8:
    case 9:
      if (count > 0)
        return count + " Bet";
      else
        return count + " Hold";
    case 10:
    case 'J':
    case 'Q':
    case 'K':
    case 'A':
      count-= 1;
      if (count > 0)
        return count + " Bet";
      else
        return count + " Hold";
  }
```

