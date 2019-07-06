> paste [this markdown of exercises](https://raw.githubusercontent.com/janke-learning/truthiness/master/README.md) into this file and complete the exercises!   

# Truthiness

Truthiness is relatively simple to understand.  Does a value convert to _true_ or _false_ when cast to boolean?

This repo covers several key language features who's behavior is dependant on the __truthiness__ of their arguments.

### Index
* [determining truthiness](#determining-truthiness)
* [falsey values](#falsey-values)
* [operators of truhiness](./operators-of-truthiness.md)
* [statements of truhiness](./statements-of-truthiness.md)
* [resources](#resources)

---
---

## Determining Truthiness


Paste this in the console to learn about truthiness, or study it [on python tutor](http://www.pythontutor.com/live.html#code=const%20x%20%3D%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20coerced_to_bool%20%3D%20Boolean%28x%29%3B%0A%0Aconsole.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0Aconsole.log%28%22coerced_to_bool%3A%20%22%20%2B%20typeof%20coerced_to_bool%20%2B%20%22,%20%22%20%2B%20coerced_to_bool%29%3B%0Aconsole.log%28coerced_to_bool%20%2B%20%22y%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B&cumulative=false&curInstr=9&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false):
```js
{
  const x = ; // experiment with different values 
  
  const coerced_to_bool = Boolean(x);
 
  console.log("x: " + typeof x + ", " + x);
  console.log("coerced_to_bool: " + typeof coerced_to_bool + ", " + coerced_to_bool);
  console.log(coerced_to_bool + "y: " + typeof x + ", " + x);
};
```  
values to try:
```js
a: true       --> ?
a: false      --> ?
a: 0          --> ?
a: 1          --> ?
a: null       --> ?
a: undefined  --> ?
a: ''         --> ?
a: ' '        --> ?
a: 'tiil'     --> ?
a: 2          --> ?
a: 345        --> ?
a: NaN        --> ?
a: Infinity   --> ?
a: -Infinity  --> ?
a: -3         --> ?
a: -0.0       --> ?
```

---

## Falsey Values

JavaScript has only 6 falsey primitive values.  All other values are truthy.

[on pytut](https://goo.gl/urDfWG)

```js
{
  const x = ;
  
  const coerced_to_bool = Boolean(x);
  
  console.log("x: " + typeof x + ", " + x);
  console.log("coerced_to_bool: " + typeof coerced_to_bool + ", " + coerced_to_bool);
  console.log(coerced_to_bool + "y: " + typeof x + ", " + x);
};
```
the values:
```js
1: false      --> ?

2: null       --> ?

3: undefined  --> ?

4: ''         --> ?
4: ""         --> ?
4: ``         --> ?

5: NaN        --> ?

6: 0          --> ?
6: 0.0        --> ?
6: +0         --> ?
6: -0         --> ?
```


[TOP](#truthiness)

---


## Resources

__study tools__:
* [PythonTutor for JavaScript](http://www.pythontutor.com/live.html#code=&cumulative=false&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false)
* [the Parsonizer](https://janke-learning.github.io/parsonizer/)

__helpful links__:
* pytut snippets:
    * [truthy & falsey values](https://goo.gl/jBTLFD) 
    * [&& vs. ||](https://goo.gl/BBXea6)  
* javascript.info
    * [data types](https://javascript.info/types)
    * [type conversions](https://javascript.info/type-conversions)
    * [conditionals](https://javascript.info/ifelse)
    * [logical operators](http://javascript.info/logical-operators)  
    * [loops](https://javascript.info/while-for)
* mdn: [logicals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_Operators), [ternary](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)
* [truthiness & comparisons](https://dorey.github.io/JavaScript-Equality-Table/) - click on the "if()" tab for truthiness
* from __boolean by example__: 
    * [truthiness for the console](https://github.com/janke-learning/boolean-by-example/blob/master/README.md#truthiness) 
    * [&&, || for the console](https://github.com/janke-learning/boolean-by-example#and-or-operators)
    * [! for the console](https://github.com/janke-learning/boolean-by-example#not)
    * [live in devtools](https://janke-learning.github.io/boolean-by-example/)
* mdn: 
    * [boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean)  
    * [truthy](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)  
    * [falsey](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)  
* [a codepen](https://codepen.io/philipwalton/pen/nufrk) 

[TOP](#truthiness)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
