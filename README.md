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
Loops & nested loops

NESTED

for(let i = 0; i < .length; i++){
for(let j = 0; j < [i].length; j++){
console.log( [i][j])
}
}

MAP

Map requires a new variable, it will create a new array using a previous one - call the 1st variable then add ".map" - from there you can call an arrow function ( => );

ForEach

Is used to work on every element in the array, it will not generate a new array as of "map".

To make it work use ".forEach (() => () );"

Filter

Fill create a new array if the condition passes
