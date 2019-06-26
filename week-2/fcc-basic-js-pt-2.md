> complete the rest of [basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) on FCC and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 



## 80. Build JavaScript Objects
```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

var myDog = {
  name: "AA", 
  legs: 3,
  tails: 1,
  friends: ["a","b","c"]
};
```

## 81. Accessing Object Properties with Dot Notation
```js
// Setup
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

// Only change code below this line

var hatValue = testObj.hat;      // Change this line
var shirtValue = testObj.shirt;    // Change this line
```

## 82.  Accessing Object Properties with Bracket Notation
```js
// Setup
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

// Only change code below this line

var entreeValue = testObj["an entree"];   // Change this line
var drinkValue = testObj["the drink"];    // Change this line
```

## 83. Accessing Object Properties with Variables
```js
// Setup
var testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};

// Only change code below this line;

var playerNumber = 16;       // Change this Line
var player = testObj[playerNumber];   // Change this Line
```

## 84. Updating Object Properties
```js
// Setup
var myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line.

myDog.name = "Happy Coder";
//or
myDog["name"]="Happy Coder";
```

## 85. Add New Properties to a JavaScript Object
```js
myDog.bark = "woof";
//or
myDog["bark"] = "woof";
```

## 86. Delete Properties from a JavaScript Object
```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line.

delete myDog.tails;
//or
delete myDog["tails"];
```

## 87. Using Objects for Lookups
```js
// Setup
function phoneticLookup(val) {
  

  // Only change code below this line
  var lookup = {
    "alpha":  "Adams",
    "bravo": "Boston",
    "charlie": "Chicago",
    "delta": "Denver",
    "echo":  "Easy",
    "foxtrot": "Frank",
  }
  // Only change code above this line
  var result = lookup[val];
  return result;
}

// Change this value to test
console.log(phoneticLookup("charlie")); /// Chicago
```

## 88. Testing Objects for Properties
```js
// Setup
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {
  // Your Code Here
  if(myObj.hasOwnProperty(checkProp))
    return myObj[checkProp];
  else
    return "Not Found";
}

// Test your code by modifying these values
console.log(checkObj("gift"));
console.log(checkObj("pet"));
console.log(checkObj("aa"));
```

## 89. Manipulating Complex Objects
```js
var myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [ 
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  },
  // Add record here
  {
    "artist": "Rihanna",
    "title": "New",
    "release_year": 2016,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold" : false
  }
];

```

## 90. Accessing Nested Objects
```js
// Setup
var myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};

var gloveBoxContents = myStorage.car.inside["glove box"]; // Change this line
```

## 91. Accessing Nested Arrays
```js
// Setup
var myPlants = [
  { 
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }  
];

// Only change code below this line

var secondTree = myPlants[1].list[1]; // Change this line

```

## 92. Record Collection
```js
// Setup
var collection = {
    "2548": {
      "album": "Slippery When Wet",
      "artist": "Bon Jovi",
      "tracks": [ 
        "Let It Rock", 
        "You Give Love a Bad Name" 
      ]
    },
    "2468": {
      "album": "1999",
      "artist": "Prince",
      "tracks": [ 
        "1999", 
        "Little Red Corvette" 
      ]
    },
    "1245": {
      "artist": "Robert Palmer",
      "tracks": [ ]
    },
    "5439": {
      "album": "ABBA Gold"
    }
};
// Keep a copy of the collection for tests
var collectionCopy = JSON.parse(JSON.stringify(collection));

// Only change code below this line
function updateRecords(id, prop, value) {
  id = id.toString() ;
  if(prop != "tracks" && value != "")
  {
   
   collection[id][prop] = value;
   
  }else if (prop == "tracks" && collection[id].hasOwnProperty("tracks")== false)
  {
   
    collection[id][prop] = [];
    collection[id][prop].push(value);
  } else if (prop == "tracks" && value != "")
  {
    
    collection[id][prop].push(value);
  } else if (value == "")
  {
    
    delete  collection[id][prop];
  }
  
  return collection;
}

// Alter values below to test your code
updateRecords(5439, "artist", "ABBA");

*** Need id = id.toString nad use [id] for spec not .id
```
## 93. Iterate with JavaScript While Loops
```js
// Setup
var myArray = [];

// Only change code below this line.

var i = 0;
while (i < 5)
{
  myArray.push(i);
  i++;
}
```
## 94. Iterate with JavaScript For Loops
```js
// Setup
var myArray = [ ];

// Only change code below this line.
for(var i =1; i<6 ;i++){
  myArray.push(i);
}
```
## 95. Iterate Odd Numbers With a For Loop
```js
var myArray = [];

// Only change code below this line.
for (var i = 1; i < 10; i += 2) {
  myArray.push(i);
}
```
## 96. Count Backwards With a For Loop
```js
// Setup
var myArray = [];

// Only change code below this line.

for (var i = 9; i > 0; i -= 2) {
  myArray.push(i);
}
```
## 97. Iterate Through an Array with a For Loop
```js
// Setup
var myArr = [ 2, 3, 4, 5, 6];
var total = 0;

// Only change code below this line

for (var i = 0; i < myArr.length; i++) {
  total += myArr[i];
}
```
## 98. Nesting For Loops
```js
function multiplyAll(arr) {
  var product = 1;
  for (var i=0; i<arr.length; i++){
    for(var j=0; j<arr[i].length;j++)
      product *= arr[i][j]; 
  }
  return product;
}

// Modify values below to test your code
console.log(multiplyAll([[1],[2],[3]]));

```
## 99. Iterate with JavaScript Do...While Loops
```js
// Setup
var myArray = [];
var i = 10;

// Only change code below this line.

do {
  myArray.push(i);
  i++;
} while (i < 5) 

// Essentially, a do...while loop ensures that the code inside the loop will run at least once.
```
## 100. Profile Lookup
```js
//Setup
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    }
];


function lookUpProfile(name, prop){
// Only change code below this line
var xname = false;
var xprop = false;
for(var i=0; i<contacts.length; i++)
{
  if(contacts[i].firstName == name){ 
    xname=true;
    if (contacts[i].hasOwnProperty(prop)){
      xprop = true;
      return contacts[i][prop];
    } 
  }
}
if (!xname)
    return "No such contact";
if (!xprop)
     return "No such property";
  

// Only change code above this line
}

// Change these values to test your function
lookUpProfile("Kristian", "lastName");

*** HAD PROBLEM WITH .prop and [prop] ***
```
## 101. Generate Random Fractions with JavaScript
```js
function randomFraction() {

  // Only change code below this line.

  return Math.random();

  // Only change code above this line.
}
```
## 102. Generate Random Whole Numbers with JavaScript
```js
function randomWholeNum() {
  return Math.floor(Math.random() * 10);
}
```
## 103. Generate Random Whole Numbers within a Range
```js
function randomRange(myMin, myMax) {

  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin;
}
```
## 104. Use the parseInt Function
```js
function convertToInteger(str) {
  return parseInt(str);
}

convertToInteger("56");
```
## 105. Use the parseInt Function with a Radix
```js
function convertToInteger(str) {
  return parseInt(str, 2);
}

console.log(convertToInteger("10011")); // 19
```
## 106. Use the Conditional (Ternary) Operator
```js
function checkEqual(a, b) {
  return a==b ? true : false;
}

checkEqual(1, 2);
```
## 107. Use Multiple Conditional (Ternary) Operators
```js
function checkSign(num) {
  return num == 0 ? "zero" : num > 0 ? "positive" : "negative";
}

checkSign(10);
```
