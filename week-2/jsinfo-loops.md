> start (and try to finish) the [loop tasks](https://javascript.info/while-for) from javascript.info and paste each of your solutions into this file.  
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

## 1. Last loop value
```js
alert(i) -> 3,2,1
1 is the last alerted value. At 1's iteration, 1 is decreased by 1 after being alerted. Which results in 0. In while loop, 0 means false so iteration exits the loop.
```

## 2. Which values does the while loop show? 
```js
1. Prefix
let i = 0;
while (++i < 5) alert( i );
  1 < 5 alert(1)
  2 < 5 alert(2)
  ...
  4 < 5 alert(4)

2.Postfix 
let i = 0;
while (i++ < 5) alert( i );
  0 < 5 alert(1)
  1 < 5 alert(2)
  ...
  4 < 5 alert(5)
  
DIFFERENT
```

## 3. Which values get shown by the "for" loop?
```js
1. Postfix
for (let i = 0; i < 5; i++) alert( i );
  0 < 5 alert(0)
  1 < 5 alert(1)
  ...
  4 < 5 alert(4)

2. Prefix
for (let i = 0; i < 5; ++i) alert( i );
 0 < 5 alert(0)
  1 < 5 alert(1)
  ...
  4 < 5 alert(4)

SAME
```

## 4. Output even numbers in the loop
```js
for (var i = 2; i <= 10 ; i+=2){
  console.log(i);
}
```
## 5. Replace for with while
```js
for (let i = 0; i < 3; i++) {
  alert( `number ${i}!` );
}

let i = 0;
while(i<3){
  alert (`number ${i}` );
  i++;
}
```
## 6. Repeat until the input is correct
```js
var input;
do{
  input = prompt("Please enter a number greater than 100");
} while(input <= 100 && input);

```
## 7. Output prime numbers
```js
var n = prompt("Enter a number");
var primes = [];

pr: for (var i = 2; i < n; i++){
    for(var j=2; j< i; j++){ 
        if(i%j==0 && i!=j)
        continue pr;      
    }
    primes.push(i)
}

console.log(primes);
```

