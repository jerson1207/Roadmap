# Keyed Collections
Keyed collections are data collections that are **ordered by key not index**. They are associative in nature. Map and set objects are keyed collections and are iterable in the order of insertion.
> When you want to work on with key valude pairs better use map

https://www.youtube.com/watch?v=rMmnFYvqKtw

## Map object
Creating a collection of key/value pairs

To Create a map you use a map constractor, you need to use new keyword
```javascript
let coll = new Map();
```
> In creating Object and to set up the property you use the dot syntax, and many others<br>
> In map you use set method

```javascript
let coll = new Map();
coll.set('key', 100)
```
> To access the key value pair we ned the **get method**
```javascript
let coll = new Map();
coll.set('key', 100);
console.log(coll.get('key'))
// 100
```
> You can access all the values
```javascript
let coll = new Map();
coll.set('key', 100);
coll.set(300, 200);
console.log(coll.values());
// [Map Iterator] { 100, 200 }
```

The use of **for of loop**
