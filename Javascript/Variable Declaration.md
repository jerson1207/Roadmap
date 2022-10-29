# Variable Declarations
> To use variables in JavaScript, we first need to create it i.e. declare a variable. To declare variables, we use one of the **var, let, or const** keywords.


#### About var keyword
 - can be called global, function and block
 - var keyword has pre-defined value of undifined
 
Example: **let declared inside the block and called outside the block**
```javascript
if (true) {
  var varVariable = 'var is inside the block'
}

console.log(varVariable)
// var is inside the block
```

Example: **let declared twice and called**
```javascript
var varVariable = 'First Declared'
var varVariable = 'Second Declared'
console.log(varVariable)
// Second Declared
``


Example: **var keyword declared last**
```javascript
console.log(varVariable)
var varVariable = 'This is true'

// undefined
//Note: var has predefined value of undifined
// its like var varVariable = undefined;
```
<hr>

### let and const keyword
- can be called with the function and block
- let and const are the same in every way except for changing the value

Example: **let declared inside the block and called outside the block**
```javascript
if (true) {
  let letVariable = 'let is inside the block'
}

console.log(letVariable)
// Uncaught ReferenceError: letVariable is not defined ...
```

Example: **let declared twice and called**
```javascript
let letVariable = 'First Declared'
let letVariable = 'Second Declared'
console.log(letVariable)
// Identifier 'letVariable' has already been declare
```

Example: **let keyword declared last**
```javascript
console.log(letVariable)
let letVariable = 'This is true'
// Uncaught ReferenceError: letVariable is not defined ...
```

### let and const difference

Example: Changing the value

```javascript
let letVariable = 1
letVariable = 2
console.log(letVariable)
// 2


const constVariable = 1
constVariable = 2
console.log(constVariable)
// Uncaught TypeError: Assignment to constant variable. ...
```

Example: const in object, changing its value
```javascript
const constVariable = {name: 'Jmaes'} 
constVariable .name = 'Bob'
console.log(constVariable)
// { name: 'Bob' }
```
