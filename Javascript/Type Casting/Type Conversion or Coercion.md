# Type Conversion/Coercion
> It force convert from one data type to another

Example: 
```javascript
const value1 = "5";
const value2 = 9;
let sum = value1 + value2;

console.log(sum);
// 59
```
> It coerce the value2 to be string and the '+' concatenate value1 and value2

```javascript
const value1 = "5";
const value2 = 9;
let sum = Number(value1) + value2;
console.log(sum);
// 14
```
URL: https://developer.mozilla.org/en-US/docs/Glossary/Type_coercion
