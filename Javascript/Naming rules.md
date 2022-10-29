# Naming rules or Naming convention
>> Why namin convetion is important?
>> - It improves readability.
>> - It speeds up development. You don'e need to think what is that for...
>> - Other can understan your code easily.

### Rules of Naming
  1. Variable names must begin with a letter, an underscore (_) or a dollar sign ($).
  2. Variable names cannot contain spaces.
  3. Variable names are case-sensitive.
  4. Variable names cannot use reserved words.
  5. There's no limit to the length of the variable name.

### JAVASCRIPT NAMING CONVENTIONS: 

#### CONSTANT
> Written in capital letters (UPPERCASE):

```javascript
const SECONDS = 60;
const MINUTES = 60;
const HOURS = 24;
const DAY = SECONDS * MINUTES * HOURS;
const DAYS_UNTIL_TOMORROW = 1;
```


### Naming Convention for variable
>> A string, boolean or number, but also an object, array or function -- is declared with a camelCase variable name.
>> Should be self-descriptive. It shouldn't be necessary to add a comment for additional documentation to the variable.

```javascript
// bad
var firstname = 'Robin';

// bad
var first_name = 'Robin';

// bad
var FIRSTNAME = 'Robin';

// bad
var FIRST_NAME = 'Robin';

// good
var firstName = 'Robin';
```


### Naming Convention for boolean
>> A prefix like is, are, or has helps every JavaScript developer to distinguish a boolean from another variable by just looking at it:

```javascript
// bad
var visible = true;

// good
var isVisible = true;

// bad
var equal = false;

// good
var areEqual = false;

// bad
var encryption = true;

// good
var hasEncryption = true;
```
>> In contrast to strings and integers, you can see it as another soft rule for a JavaScript boolean naming convention besides being written in camel case.

### Naming convention for FUNCTION
  >> 1. written in camel case too. 
  >> 2. Best practice: **user verb as prefix.** This verb as prefix can be anything (e.g. get, fetch, push, apply, calculate, compute, post)
```javascript
// bad
function name(firstName, lastName) {
  return `${firstName} ${lastName}`;
}

// good
function getName(firstName, lastName) {
  return `${firstName} ${lastName}`;
}
```

### JAVASCRIPT NAMING CONVENTIONS: CLASS
>> A JavaScript class is declared with a PascalCase in contrast to other JavaScript data structures: <br>
>> Every time a JavaScript constructor is called to instantiate a new instance of a class, the name of the class should appear in Pascal Case, because the class has been declared with Pascal Case in the first place.

```javascript
class SoftwareDeveloper {
  constructor(firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
  }
}

var me = new SoftwareDeveloper('Robin', 'Wieruch');
```














