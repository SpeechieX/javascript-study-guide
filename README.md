```
    __   ______   __   __ ______   ______   ______   ______   __   ______  ______  
   /\ \ /\  __ \ /\ \ / //\  __ \ /\  ___\ /\  ___\ /\  == \ /\ \ /\  == \/\__  _\ 
  _\_\ \\ \  __ \\ \ \'/ \ \  __ \\ \___  \\ \ \____\ \  __< \ \ \\ \  _-/\/_/\ \/ 
 /\_____\\ \_\ \_\\ \__|  \ \_\ \_\\/\_____\\ \_____\\ \_\ \_\\ \_\\ \_\     \ \_\ 
 \/_____/ \/_/\/_/ \/_/    \/_/\/_/ \/_____/ \/_____/ \/_/ /_/ \/_/ \/_/      \/_/ 
	
```

# What's In This Document 

This is a list of JavaScript concepts meant to be used by beginners learning JavaScript. This is essentially a checklist for topics to study.

## Primitives and Conditionals

Be able to manipulate the following primitives: 

* Numbers 
    - `%` 
    - `+`
    - `-`
    - `/`
    - `*`
    - `Math.floor` 
    - `Math.min`
    - `Math.max`
* Booleans 
    - `&&` 
    - `||`
    - `!`
    - Values in JS have implcit `true` and `false` values known as *truthy* and *falsy*
    - `!!` type coercion
* Strings 
    - `slice`
    - `splice` 
    - template literals: `this is a ${someVariable}`
    - strings are indexed (e.g., "cat"[1] //=> "a")
* `while` loops 
* `if` conditional 
* ternary operators (`bool ? value : value`)

## Functions 

* **defining** and **invoking** functions for example: 


```js 
// I am defining a function here: 
function fn(parameter) {
    return parameter
}

// I am invoking a function here:
fn("argument")
```
* closures
* callback functions: functions passed to other functions
* lexical scope in JS: know if a variable is in scope 
    - new scope is defined within functions
* `return` keyword terminates the function and causes the function to be evaluated to whatever expression is to the right of the `return`
* arrow functions
    - preserve lexical scope 
    - implicit `return` 

```js
// This is an arrow function 
const fn = () => "Hello World!" // There is an "implicit return before the "Hello World" 

const add = (a,b) => {
    return a + b; // No implicit return 
}
```

* Immediately Invoked Function Expressions (IIFE's)

## Objects and ES6 Classes

* create objects, update properties, delete properties, add new properties 
* the `this` keyword
* `for..in` to iterate through objects 
* Bracket(`[]`) vs. dot (`.`) look-up on objects
* Objects are stored by reference **NOT** value
* ES6 Classes: 
    - `constructor` functions 
    - `class` keyword 
    - `extends` keyword 
    - `super`


## Arrays 

* Know how to define arrays 
* Arrays are stored by reference **NOT** value
* Iterate through arrays with a `for-loop`
* Know the following methods on the Array prototype: 
    - `map`
    - `reduce` 
    - `filter` 
    - `some` 
    - `includes` 
    - `forEach`
    - `pop`
    - `push`
    - `shift`
    - `unshift` 
    - `indexOf` 
    - `sort`

* Arrays are 0-indexed
* Spread operator


