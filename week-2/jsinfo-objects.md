> start (and try to finish) the [object tasks](https://javascript.info/object) from javascript.info and paste each of your solutions into this file.    
> Don't be afraid of peeking at the solutions!  Just be sure you study them well


## 1. 
```js
var user = {};
user.name = "John";
user.surname= "Smith";
user.name = "Pete";
remove user.name;
```

## 2.
```js
function isEmpty(obj){
  for( var value in obj)
    return false;
  return true;
}
```

## 3.
```js
My answer: No, it cannot be changed. 
Correct answer: Yes, as long as the decleared variable is not changed, consts can be altered. 
```

## 4. 
```js
function sumSalaries(obj){
  var sum = 0;
  for (var person in obj)
    sum += obj[person];
    
   return sum;
}

let salaries = {
  John: 100,
  Ann: 160,
  Pete: 130
}

console.log(sumSalaries(salaries));
```

## 5.
```js
function multiplyNumeric(obj){
  for (var val in obj){
    if(typeof obj[val] == "number"){
      obj[val] *=2;
    }
  }
}
```
