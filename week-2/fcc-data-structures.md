> begin [the basic data structure exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-data-structures) and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  


## 1. Use an Array to Store a Collection of Data
```js
let yourArray = [ "Saliha", 22, true, "Student", 50 ];

```
## 2. Access an Array's Contents Using Bracket Notation
```js
let myArray = ["a", "b", "c", "d"];

myArray[1] = "anything";
```

## 3. Add Items to an Array with push() and unshift()
```js
push() method adds elements to the end of an array, and unshift() adds elements to the beginning

function mixedNumbers(arr) {
  // change code below this line
    arr.unshift('I', 2, 'three');
    arr.push(7, 'VIII', 9);
  // change code above this line
  return arr;
}

// do not change code below this line
console.log(mixedNumbers(['IV', 5, 'six']));
```

## 4. Remove Items from an Array with pop() and shift()
```js
pop() removes an element from the end of an array, while shift() removes an element from the beginning

function popShift(arr) {
  let popped = arr.pop(); 
  let shifted = arr.shift(); 
  return [shifted, popped];
}

// do not change code below this line
console.log(popShift(['challenge', 'is', 'not', 'complete']));  // challenge,complete
```

## 5. Remove Items Using splice()
```js
function sumOfTen(arr) {
  // change code below this line
  arr.splice(2,2);
  // change code above this line
  return arr.reduce((a, b) => a + b);
}

// do not change code below this line
console.log(sumOfTen([2, 5, 1, 5, 2, 1]));
```

## 6. Add Items Using splice()
```js
function htmlColorNames(arr) {
  // change code below this line
  arr.splice(0,2,'DarkSalmon','BlanchedAlmond');
  // change code above this line
  return arr;
} 
 
// do not change code below this line
console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurqoise', 'FireBrick']));
```
## 7. Copy Array Items Using slice()
```js
function forecast(arr) {
  // change code below this line
  
  return arr.slice(2,4);
}

// do not change code below this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms'])) // warm,sunny
```

## 8. Copy an Array with the Spread Operator
```js
function copyMachine(arr, num) {
  let newArr = [];
  while (num >= 1) {
    newArr.push([...arr]);
    num--;
  }
  return newArr;
}

// change code here to test different cases:
console.log(copyMachine([true, false, true], 2));
```

## 9. Combine Arrays with the Spread Operator
```js
function spreadOut() {
  let fragment = ['to', 'code'];
  case 1: let sentence = ['learning',...fragment,'is','fun'];
  case 2: let sentence = ['learning',fragment,'is','fun'];
  fragment[0] = 'as';
  return sentence;
}

// do not change code below this line
console.log(spreadOut());


... creates vars and copies fragment elements
not using ... references to fragnemtn elements. So any changes to fragment will change the result.
```

## 10. Check For The Presence of an Element With indexOf()
```js
function quickCheck(arr, elem) {
  // change code below this line
  if (arr.indexOf(elem) == -1)
  return false;
  else
  return true;
  // change code above this line
}

// change code here to test different cases:
console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));
```
## 11.  Iterate Through All an Array's Items Using For Loops *** HARD ***
```js
function filteredArray(arr, elem) {
  let newArr = [];
  // change code below this line
var a = 0;
for(let i=0; i<arr.length ; i++)
{ newArr[a] = [];
  newArr[a].push(...arr[i]);
  for(let j=0; j<arr[i].length; j++)
  {
    if(arr[i][j] == elem)
     { newArr.pop();
      a--
     }
  }
  a++;
}
  // change code above this line
  return newArr;
}

// change code here to test different cases:
console.log(filteredArray([[10, 8, 3], [14, 6, 23], [3, 18, 6]], 18));

*** USING INDEXOF ***

function filteredArray(arr, elem) {
  let newArr = [];
  // change code below this line
  
 for (let i = 0; i < arr.length; i++) { 
    if (arr[i].indexOf(elem)==-1){ //Checks every parameter for the element and if is NOT there continues the code
          newArr.push(arr[i]); //Inserts the element of the array in the new filtered array
            };
          };

  // change code above this line
  return newArr;
};
```

## 12. Create complex multi-dimensional arrays
```js
let myNestedArray = [
  // change code below this line
  ['unshift', false, 1, 2, 3, 'complex', 'nested'],
  ['loop', 'shift', 6, 7, 1000, 'method'],
  ['concat', false, true, 'spread', 'array'],
  ['mutate', 1327.98, 'splice', 'slice', 'push'],
  ['iterate', 1.3849, 7, '8.4876', 'arbitrary', 'depth'],
  [[[['deepest']]]],
  [[['deeper']]],
  [['deep']]
  // change code above this line
];
```

## 13. Add Key-Value Pairs to JavaScript Objects
```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28
};

// change code below this line
foods.bananas= 13;
foods.grapes=35;
foods.strawberries = 27;
// change code above this line

console.log(foods);
```

## 14.  Modify an Object Nested Within an Object
```js
let userActivity = {
  id: 23894201352,
  date: 'January 1, 2017',
  data: {
    totalUsers: 51,
    online: 42
  }
};

// change code below this line
userActivity.data.online = 45;
// change code above this line

console.log(userActivity);
```
## 15. Access Property Names with Bracket Notation
```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};
// do not change code above this line

function checkInventory(scannedItem) {
  // change code below this line
  if(foods.hasOwnProperty(scannedItem))
    return foods[scannedItem];
  else
  return undefined;
}

// change code below this line to test different cases:
console.log(checkInventory("apples"));
```

## 16. Use the delete Keyword to Remove Object Properties
```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};

// change code below this line
delete foods.oranges;
delete foods.plums;
delete foods.strawberries;
// change code above this line

console.log(foods);
```

## 17. Check if an Object has a Property
```js
let users = {
  Alan: {
    age: 27,
    online: true
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: true
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function isEveryoneHere(obj) {
  if(users.hasOwnProperty('Alan','Jeff','Sarah','Ryan')) {
    return true;
  }
  return false;
 
}

console.log(isEveryoneHere(users));
```

## 18. Iterate Through the Keys of an Object with a for...in Statement

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function countOnline(obj) {
  // change code below this line
  var a=0;
  for (let usr in users)
  {
    if(users[usr].online)
    a++;
  }
  return a;
}

console.log(countOnline(users));

```
## 19. Generate an Array of All Object Keys with Object.keys()

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function getArrayOfUsers(obj) {
  // change code below this line
  return Object.keys(obj);
  // change code above this line
}

console.log(getArrayOfUsers(users));  // Alan,Jeff, Sarah, Ryan
```
## 20. Modify an Array Stored in an Object
```js
let user = {
  name: 'Kenneth',
  age: 28,
  data: {
    username: 'kennethCodesAllDay',
    joinDate: 'March 26, 2016',
    organization: 'freeCodeCamp',
    friends: [
      'Sam',
      'Kira',
      'Tomo'
    ],
    location: {
      city: 'San Francisco',
      state: 'CA',
      country: 'USA'
    }
  }
};

function addFriend(userObj, friend) {
  // change code below this line  
  userObj.data.friends.push(friend);
  return userObj.data.friends;
  // change code above this line
}

console.log(addFriend(user, 'Pete'));
```

