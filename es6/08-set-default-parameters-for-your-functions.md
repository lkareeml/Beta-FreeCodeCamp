# ES6: Set Default Parameters for Your Functions

In order to help us create more flexible functions, ES6 introduces default parameters for functions.

Check out this code:
```javascript
    function greeting(name = "Anonymous") {
      return "Hello " + name;
    }
    console.log(greeting("John")); // Hello John
    console.log(greeting()); // Hello Anonymous
```
The default parameter kicks in when the argument is not specified (it is undefined). As you can see in the example above, the parameter name will receive its default value "Anonymous" when you do not provide a value for the parameter. You can add default values for as many parameters as you want.

Modify the function increment by adding default parameters so it will always return a valid number and it will add 1 to number if value is not specified.

Note
Don't forget to use strict mode.

# Solution:

```javascript

function increment(number, value = 1) {
    return number + value;
}
console.log(increment(5, 2)); // returns 7
console.log(increment(5)); // returns NaN

```
