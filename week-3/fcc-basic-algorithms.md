> [FCC basic algorithm scripting](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-algorithm-scripting) - complete a few and paste your solutions into this MD file.  
> recommended challenges (alphabetically): celcius to farenheit, chunkey monkey, factorialize, falsey bouncer, largest of 4, repeat, reverse a string, title case.  And the rest are also great
> examples to study: [samanthaming](https://github.com/samanthaming/freecodecamp-my-solutions/tree/master/basic-algorithm), [jadonOrr](https://github.com/jadonOrr/freeCodeCampAlgorithms/tree/master/basic-algorithms), [TheNewStyles](https://github.com/TheNewStyles/freecodecamp-algorithm-solutions/tree/master/BasicAlgorithmScripting)


## 1. Convert Celsius to Fahrenheit
```js
function convertToF(celsius) {
  let fahrenheit = celsius*9/5+32;
  return fahrenheit;
}

console.log(convertToF(30)); // 86
```

## 2. Reverse a String
```js
function reverseString(str) {
  var newstr = "";
  for(let i=str.length; i>0; i--)
    newstr+=str[i-1];
  return newstr;
}

console.log(reverseString("hello"));

/// solution 2

function reverseString2(str) {
  var newarr = str.split("");
  newarr.reverse();
  return newarr.join("");  
}

console.log(reverseString2("hello"));
```
## 3. Factorialize a Number
```js
function factorialize(num) {
  let ret = 1;
  for(let i=1; i<num+1; i++)
    ret*=i;
  return ret;
}

console.log(factorialize(5));
```
## 4. Find the Longest Word in a String
```js
function findLongestWordLength(str) {
  let len = 0;
  let arr = str.split(" ");
  for(let i=0; i<arr.length; i++)
  {    if(arr[i].length > len)
          len = arr[i].length;
  }
  return len;
}

console.log(findLongestWordLength("The quick brown fox jumped over the lazy dog"));  // 6

```
## 5. Return Largest Numbers in Arrays
```js
function largestOfFour(arr) {
 let newarr = [];
 let largest;
  for(let i =0; i<arr.length; i++){
    largest = arr[i][0];
    for(let j=0; j< arr[i].length; j++){
      if(arr[i][j] > largest){
        largest = arr[i][j];
      }
    }
    newarr.push(largest);
  }
  return newarr;
}

console.log(largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]));
```
## 6. Confirm the Ending
```js
function confirmEnding(str, target) {
  return str.slice(-target.length) == target;
}

console.log(confirmEnding("Bastian", "n"));
```
## 7. Repeat a String Repeat a String
```js
function repeatStringNumTimes(str, num) {
  let newstr = "";
  let i=0;
  while(i<num){
    newstr+=str;
    i++;
  }
  return newstr;
}

console.log(repeatStringNumTimes("abc", 3));
```
## 8. Truncate a String
```js
function truncateString(str, num) {
  if(num < str.length)
    return str.slice(0,num)+"...";
  else
    return str;
}

console.log(truncateString("A-tisket a-tasket A green and yellow basket", "A-tisket a-tasket A green and yellow basket".length));
```
## 9. Finders Keepers **IMP**
```js
function findElement(arr, func) {
  for(let i =0; i< arr.length; i++){
    if(func(arr[i]))
      return arr[i];
  }
  return undefined;
}

findElement([1, 2, 3, 4], num => num % 2 === 0);

```
## 10. Boo who
```js
function booWho(bool) {
  if(bool === true || bool === false)
       return true;
  return false;
}

console.log(booWho(null));
```
## 11. Title Case a Sentence
```js
function titleCase(str) {
 
  let newarr = str.toLowerCase().split(" ");
  
  for(let i in newarr){
    newarr[i] = newarr[i][0].toUpperCase() + newarr[i].slice(1);
  }
return newarr.join(" ");
}

console.log(titleCase("I'm a little tea pot"));
```
## 12. Slice and Splice **QUESTION *** 
```js
/*
function frankenSplice(arr1, arr2, n) {
  let newarr2 = arr2.slice();
  newarr2.splice(n,0,arr1);
  return newarr2;
}

console.log(frankenSplice(["claw", "tentacle"], ["head", "shoulders", "knees", "toes"], 2));

*/

function frankenSplice(arr1, arr2, n) {
  let newarr2 = arr2.slice();
  for (let i = 0; i < arr1.length; i++) {
    newarr2.splice(n, 0, arr1[i]);
    n++;
  }  
  return newarr2;
}

console.log(frankenSplice(["claw", "tentacle"], ["head", "shoulders", "knees", "toes"], 2));

```
## 13. Falsy Bouncer
```js
function bouncer(arr) {
  let newarr = [];
  for (var i in arr)
  {
    if(Boolean(arr[i]))
      newarr.push(arr[i]);
  }
  return newarr;
}

console.log(bouncer([7, "ate", "", NaN, 9]));

function bouncer2(arr) {
  
  return arr.filter(Boolean);
}

console.log(bouncer2([7, "ate", "", NaN, 9]));
```
## 14. Where do I Belong . *** QUESTION ***
```js
function getIndexToIns(arr, num) {
  let newarr = arr.sort(function(a, b) {
    return a - b;});
  for(let i=0; i< newarr.length; i++) .  //** GAVE ERROR WHEN for(let i in newarr)
  {
    if(num <= newarr[i])
      return i;
  }
return arr.length;
}

console.log(getIndexToIns([10, 20, 30, 40, 50], 35));

```
## 15. Mutations
```js
function mutation(arr) {
  var first = arr[0].toLowerCase();
  var second = arr[1].toLowerCase();

  for(let i=0; i<second.length; i++){
    if(first.indexOf(second[i]) < 0){
      return false;
    }
  }

  return true;
}

mutation(["hello", "hey"]);
```
## 16. Chunky Monkey
```js
function chunkArrayInGroups(arr, size) {
  var innerarr;
  var outerarr = [];
  for(let i=0; i< arr.length; i++){
    innerarr = [];
    for(let j=0; j< size; j++){
      innerarr.push(arr[i]);
      i++;
      if(i == arr.length)
      break;
    }
    i--;
    outerarr.push(innerarr);
  }
  return outerarr;
}

console.log(chunkArrayInGroups([0, 1, 2, 3, 4, 5], 4));

/// 

function chunkArrayInGroups(arr, size) {
      var newArr = [];
      while (arr.length) {
        newArr.push(arr.splice(0,size));
      }
      return newArr;
    }
    
```
