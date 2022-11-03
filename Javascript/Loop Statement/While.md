# While Statement
> The while statement creates a loop that executes a specified statement as long as the test condition evaluates to true. The condition is evaluated before executing the statement.

### Syntax
```javascript
while (condition)
  statement
```

#### condition
> An expression evaluated before each pass through the loop. If this condition evaluates to true, statement is executed. When condition evaluates to false, execution continues with the statement after the while loop.
#### statement
> An optional statement that is executed as long as the condition evaluates to true. To execute multiple statements within the loop, use a block statement ({ /* ... */ }) to group those statements.
#### Example # Generate a number 1 to 10 using while statement
```javascript
let counter = 1;

while (counter <= 10) {
	console.log(counter);
	counter ++;
}

// 1
// 2
// 3
// 4
// 5
// 6
// 7
// 8
// 9
// 10
```
