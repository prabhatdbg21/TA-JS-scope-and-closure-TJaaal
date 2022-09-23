1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
}

let percentage = function (marks, total) {
  return (marks * 100) / total;
}

let percentage = (marks, total) => {
  return (marks * 100) / total;
}

let percentage = (marks, total) => (marks * 100) / total;
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
```js
// expression is someting which result into value
// number, boolean, string, null, undefined and object

function add(){

}
let obj = {};

let add = function () {} ;

```


4. What is a function call an expression in JavaScript?
```js
function add(a,b){
  return a + b ;
}
function addAgain(a,b){

}

add(12 , 23); // 35    

addAgain(); // undefined

// function call always return some value when return is present and if return is not present it will give undefined which is also a value
```

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // VALID
five = add; // VALID
five = five(10, 11); // VALID
five = function () {
  return 'Hello';
}; // VALID
```

6. What is the difference between function definition and function call? Explain with an example.
Ans:- Function Definition allows us to create an anonymous function with any function name .
A function call is used to execute the series of steps .
```js
// function definition
function percentage(marks, total) {
  return (marks * 100) / total;
}

// function call
percentage (40 , 80)   // 50 (output)
```

7. What is the similarities between function definition and function call?
```js
// Function Defination is an expression (function is an object)
// Function Call is an expression (function call always returns a value)
```

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid   adding new property (user) in object (hello)

```

9. What is higher order function explain with an example.
Ans:- A function that accept a function defination as an argument or that return a function defination is known as higher order function.
```js
function multiplyBy (num){
  return function (num2){
    return num * num2 ;
  }
}
let multiplyBy10 = multiplyBy(10)
console.log (multiplyBy10(20)); // 200

// OR

function add(cb){ // HOF    (accept a function defination)
  cb()
}

function add(){ // HOF      (return a function defination)
  function main(){}
  return main
}
```


10. Explain what is callback function. Why you can pass a function inside a function?
```js
// Callback function is a function that get accepted inside a higher order function (HOF) , Because as an argument we can only pass expression and  function is an expression in JS so we can pass a function inside another function.
```




Ans:- callback function return true the value is passed inside will be stored into a new array and if it return false it will not stored into a new array.
```js
let numbers = [1,2, 3, 4 , 5, 6 ,7]
function isEven (num) {
  return num % 2 === 0 ;
}
let evenNumbers = numbers.filter(isEven) ;
console.log (evenNumbers)   //  (3) [2, 4, 6]
```

