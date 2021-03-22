# delegates-week4

### delegates this week: Gege and Hanna

---

## advanced functions

+ It's possible to assign a default value to a parameter in case no argument is passed

```javascript
function sayHello(parameter = "default argument"){
   console.log(`Hello, ${parameter}!`);
}

sayHello();
// Hello, default argument!

sayHello("Bob");
// Hello, Bob!
```

+ Arrow function is a shorter way to write functions

```javascript
function sum(a, b) {
  return a + b
}

let sum = (a, b) => { return a + b };

let sum = (a, b) => a + b;
```

+ an **anonymous function** is a function that doesn't have any label
+ A **higher-order function** is a function that accepts other function as an arguments
+ A **callback function** is a function passed as an argument of a higher-order function.

```javascript
function sayHello(userName){
	console.log(`Hello, ${userName}`);
}

function sayWelcome(userName){
	console.log(`Welcome, ${userName}`);
}

function askUserName(callback){
	const name = prompt("Hey, what's your name?");
	callback(name);
}

askUserName(sayWelcome);
askUserName(sayHello);
```
