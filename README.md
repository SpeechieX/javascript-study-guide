```
 _________  ________   __   __   ________   ______   ______   ______     ________  ______   _________  
/________/\/_______/\ /_/\ /_/\ /_______/\ /_____/\ /_____/\ /_____/\   /_______/\/_____/\ /________/\ 
\__.::.__\/\::: _  \ \\:\ \\ \ \\::: _  \ \\::::_\/_\:::__\/ \:::_ \ \  \__.::._\/\:::_ \ \\__.::.__\/ 
  /_\::\ \  \::(_)  \ \\:\ \\ \ \\::(_)  \ \\:\/___/\\:\ \  __\:(_) ) )_   \::\ \  \:(_) \ \  \::\ \   
  \:.\::\ \  \:: __  \ \\:\_/.:\ \\:: __  \ \\_::._\:\\:\ \/_/\\: __ `\ \  _\::\ \__\: ___\/   \::\ \  
   \: \  \ \  \:.\ \  \ \\ ..::/ / \:.\ \  \ \ /____\:\\:\_\ \ \\ \ `\ \ \/__\::\__/\\ \ \      \::\ \ 
    \_____\/   \__\/\__\/ \___/_(   \__\/\__\/ \_____\/ \_____\/ \_\/ \_\/\________\/ \_\/       \__\/ 
                                                                                                       
```

# JavaScript Study Guide

This is a list of JavaScript concepts. This list can be used by beginners as a checklist of concepts to study.

## Primitives and Conditionals

Be able to manipulate the following primitives: 

* Numbers 
    - `%`, `+`, `-`, `/`, `*`
    - `Math.floor` 
    - `Math.min`
    - `Math.max`
* Booleans 
    - `&&` 
    - `||`
    - `!`
    - `<`, `>`, `<=`, `>=`, `==`, `===`, `!=`, `!==`
    - What is the difference between `==` and `===`?
    - Values in JS have implicit `true` and `false` values known as *truthy* and *falsey*. What values are truthy and what values are falsey?
    - `!!` type coercion
* Strings 
    - `slice`
    - `splice` 
    - template literals: `` `this is ${someVariable}` ``
    - strings are indexed: `"cat"[1]` //=> "a")
* `while` loops 
* `if/else if/else` conditionals 
* ternary operators: `bool ? value : value`
* other JS operators: 
    - `+=`, `-=`, `*=`, `/=`, `%=`, `++`, `--`
    - What is the difference between pre-increment(`++a`) and post-increment(`a++`)?
* know the difference between `const`, `var` and `let` variable declaration keywords
* destructuring assignment 
* `parseInt`
* `null` and `undefined`
* Know about the useful things you can do with truthy and falsey values with logical operators: 

```js
a = "cat" || 0; //=> a is equal to "cat"
b = "cat" && 0; //=> b is equal to 0
c = 5 || 7; //=> c is equal to 5 
d = 5 && 7; //=> d is equal to 7
```

## Functions 

* **defining** and **invoking** functions, for example: 

```js 
// I am defining a function here: 
function fn(parameter) {
    return parameter
}

// I am invoking a function here:
fn("argument")
```
* closures and the module pattern
* callback functions: functions passed to other functions
* lexical scope in JS: know if a variable is in scope 
    - new scope is defined when a new function is defined
* `return` keyword terminates the execution of a function and causes a function to be evaluated to whatever expression is to the right of the `return`
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
* function declarations vs. function expressions 
* "hoisting" functions in JS
* What are closures?

## Objects, ES6 Classes and Prototypes

* create objects, update properties, delete properties, add new properties 
* the `this` keyword
* `for..in` to iterate through objects 
* Bracket(`[]`) vs. dot (`.`) look-up on objects
* Objects are stored by reference **NOT** value
* ES6 Classes: 
    - `constructor` functions 
    - `this` keyword
    - creating a class with the `class` keyword 
    - sub classing with the `extends` keyword 
    - super class with the `super` keyword
    - instantiate a class with the `new` keyword
    - gives objects behavior with class methods
    - class properties
* Objects are linked to other objects via `prototypes`
    - prototype delegation 
    - `getPrototypeOf`
    - `isPrototypeOf`
    - `Object.create`

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
    - `length`
    - `concat`
    - `some`
    - `find`
    - `findIndex`

* Do the above array methods mutate the array they operate on or do they create and modify a new array?
* arrays are 0-indexed
* spread operator
* Arrays in JS can hold many different types (e.g., `[1, "two", { three:"four"}]`)

## Conclusion 

If you think I should modify this document in any way please create an Issue. Enjoy!
