# Prototypal Inheritance


### using __proto__ in JavaScript

```javascript
// object surgeon
let surgeon = {
  operate: true,
  OpeateAll() {
      return "Can operate anything";
  },
};
// Object heartSurgeon
let  heartSurgeon = {
    heartSpecialist: false,
    CanOperateHeart() {
      return "Can operate heart disease";
    },
    
  //  Inheriting the properties and methods of surgeon
    __proto__: surgeon, 
};

// Property of sergeon
console.log("Sergeon can operate: " + heartSurgeon.operate); 

// Method of sergeon
console.log("Can operate all:" + heartSurgeon.OpeateAll()); 

// Property of heartSurgeon
console.log("Heart Specialist:" + heartSurgeon.heartSpecialist); 

// Method of heartSurgeon
console.log("Can operate heart: " + heartSurgeon.CanOperateHeart()); 


// Sergeon can operate: true
// Can operate all:Can operate anything        
// Heart Specialist:false
// Can operate heart: Can operate heart disease
```
