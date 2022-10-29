# Hoisting
>> Javascript runs from top to buttom in order. If you notice function can be called even if they are declared anywhere at the buttom.

Here is an example:  <br>
 - _We define **calFunc()** prior to calling it_
```javascript
function calFunc() {
    console.log("I'am a function");
  }

calFunc()
// I'am a function

```
_We call **calFunc()**  prior to defining it_
```javascript
calFunc()

function calFunc() {
  console.log("I'am a function");
}

// I'am a function
```

<hr>

>> Calling the variable at the  buttom cannot be consider as hoisting

### Testing using const keyword
Example 1: _define **str** prior to calling it_
```javascript
const str = "This is a test";
console.log(str);
// This is a test
``` 
Example 2: _call **str**  prior to defining it_
```javascript
console.log(str);
const str = "This is a test";

// Uncaught TypeError: str is not defined
```
### Testing using function
Example1: _define **calFunc** prior to calling it_
```javascript
var calFunc = function() {
  console.log("I'am a function");
}

calFunc()
// I'am a function
```

Example2: _call **calFunc** prior to defining it_
```javascript
calFunc();

var calFunc = function() {
  console.log("I'am a function");
}

// Uncaught TypeError: calFunc is not a function
```




 
