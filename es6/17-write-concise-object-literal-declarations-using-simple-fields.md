# ES6: Write Concise Object Literal Declarations Using Simple Fields

ES6 adds some nice support for easily definining object literals.

Consider the following code:
```javascript
    const getMousePosition = (x, y) => ({
      x: x,
      y: y
    });
```
getMousePosition is a simple function that returns an object containing two fields.

ES6 provides the syntactic sugar to eliminate the redundancy of having to write x: x. You can simply write x once, and it will be converted tox: x (or something equivalent) under the hood.

Here is the same function from above rewritten to use this new syntax:
```javascript
    const getMousePosition = (x, y) => ({ x, y });
```
Use simple fields with object literals to create and return a Person object.

# Solution:

```javascript

// change code below this line
const createPerson = (name, age, gender) => {
  return {name,age,gender};
};
// change code above this line
console.log(createPerson("Zodiac Hasbro", 56, "male")); // returns a proper object


```

