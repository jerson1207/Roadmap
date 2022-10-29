# Object
JavaScript object is a data structure that allows us to have key-value pairs; so we can have distinct keys and each key is mapped to a value that can be of any JavaScript data type.

Example: 
```javascript
let user = {     // an object
  name: "John",  // by key "name" store value "John"
  age: 30        // by key "age" store value 30
};

console.log(user)
// { name: 'John', age: 30 }

console.log(user.name)
// John

console.log(user.age)
// 30 
```

## Object prototypes
> Makes your code more flexible.

Example 1:
```javascript
function Person( name ,age, color){
  this.name = name;
  this.age = age;
  this.favColor = color;
  this.getName = function() {
    return " (test) Name: " + this.name;
  }
}

let father = new Person("john", 28, "green");
let mother = new Person("Ana", 28, "blue");

console.log(father.getName());
// (test) Name john
console.log(mother.getName());
// (test) Name Ana
```
Example 2:
```javascript
function Person( name ,age, color){
  this.name = name;
  this.age = age;
  this.favColor = color;
}

Person.prototype.getName = function () {
  return "Name "+ this.name;
}

let father = new Person("john", 28, "green");
let mother = new Person("Ana", 28, "blue");

console.log(father.getName());
// Name john
console.log(mother.getName());
// Name Ana
```
> - Notice the example 1 and 2 are the same in output.









