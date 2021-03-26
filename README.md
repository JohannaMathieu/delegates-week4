# delegates-week4

### delegates this week: Gege and Hanna

---
Loops & nested loops

NESTED

for(let i = 0; i < .length; i++){ for(let j = 0; j < [i].length; j++){ console.log( [i][j]) } }

MAP

Map requires a new variable, it will create a new array using a previous one - call the 1st variable then add ".map" - from there you can call an arrow function ( => );

ForEach

Is used to work on every element in the array, it will not generate a new array as of "map".

To make it work use ".forEach (() => () );"

Filter

Fill create a new array if the condition passes

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



# ARRAYS
## .map

### Map requires a new variable, it will create a new array using a previous one - call the 1st variable then add ".map" - from there you can call an arrow function ( => );

## .ForEach

### Is used to work on every element in the array, it will not generate a new array as of "map".

To make it work use ".forEach (() => () );"
to recreate it : 


## function foreach (array,callback) {

  for (let i = 0; i < array.length; i++) {
     callback(array[i])
  }
  }

  foreach( ___ , console.log)


## .Every 
to check if all items pass a given test - if even one is false, the return will be false

## .Filter

Fill create a new array if the condition passes

## .reduce
Can be used to find the total of a sumn.

## .shift
Will remove the first element of an array

## .join
Will export the array into a string + ou can add the separator in () for example (+) will show "element1 + element2 ".


# Filtering arrays

### To find the scripts in the data set that are still in use, the following function might be helpful. It filters out the elements in an array that don’t pass a test.
--------------

---

## arrays advanced

+ `unshift("elementA")` adds an elementA at the beginning of an array
+ `shift()` removes the **first element** of an array
+ `join()` will transform the array to a string. You can specify a character to seperate the array-elements -> `join(",")`

### finding elements in an array

+ `lastIndexOf(item)` will return the **last index** where a specific **item** was seen 
+ `IndexOf(item)` will return the **first index** where a specific **item** was seen

### map
`map` is a method that you can use on arrays to create a new array and execute a block of code on every element in the returning array.

```javascript
const numbers = [1, 2, 5, 7];

const doubles = numbers.map(function(num){

  return num * 2;

});


console.log(doubles);

// [2, 4, 10, 14]
```
### forEach

`map` will generate a new array. `forEach` is just doing an action for every array element.

### every
The `every` method checks if all the arrays element matches with a condition. The result of every is a boolean.

```javascript
const myArray = [11, 34, 54, 32, 54];
console.log(myArray.every(element => element > 10));
// true 
```

### filter
The `filter` method will create a new array with only the element that passes the condition of the given function.

```javascript
const myArray = [3, 2, 40, 15, 20];
const greaterThanFive = myArray.filter(number => number > 5);
console.log(greaterThanFive);
// [40, 15, 20]
```

### reduce
The `reduce` method will reduce the array to a single value.

```javascript
const myArray = [13, 200, 404, 430, 10];
console.log(myArray.reduce((acc, currentValue) => acc + currentValue));
// 1057
```

### Array destructuring

Array destructuring automatically creates variables that correspond to one or multiples items of an array.

```javascript
const animals = ["Hubert", "Rosemary", "Paul"];
const [hamster, kiwi, guineaFowl] = animals;

console.log(hamster);
// "Hubert"
console.log(kiwi);
// "Rosemary"
console.log(guineaFowl);
// "Paul"
```

### to sum up
![alt text](https://storage.googleapis.com/quest_editor_uploads/Jfb7pFRSdBBCkms0sZuykoKffThSpu0a.png)



## Dojo: Palindrome algorythm
(https://codesandbox.io/s/palindrome-algorithm-begin-forked-y7yep?file=/src/palindrome.js)
