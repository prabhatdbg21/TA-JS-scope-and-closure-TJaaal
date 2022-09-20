1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = (marks, total) => {
  return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
let percentage = (marks, total) => {
  return (marks * 100) / total;
}
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// answer
function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// answer
function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// answer
function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// answer
function percentage(marks, total) {
  return (marks * 100) / total;
}
```

3. What is a function definition an expression in JavaScript? Give one example of function expression.
Ans:- Function Expression allows us to create an anonymous function which doesn't have any function name which is the main difference between Function Expression and Function Definition. 


4. What is a function call an expression in JavaScript?
Ans:-  A function call is used to execute the series of steps . Function Expression allows us to create an anonymous function which doesn't have any function name.
```js
// function expression
let percentage = (marks, total) => {
  return (marks * 100) / total;
}

// function call
percentage (40 , 80)   // 50 (output)
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

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid   adding new property (user) in object (hello)

```

9. What is higher order function explain with an example.
Ans:- A function that accept a function defination as an argument is known as higher order function.
```js
function multiplyBy (num){
  return function (num2){
    return num * num2 ;
  }
}
let multiplyBy10 = multiplyBy(10)
console.log (multiplyBy10(20)); // 200
```


10. Explain what is callback function. Why you can pass a function inside a function?
Ans:- callback function return true the value is passed inside will be stored into a new array and if it return false it will not stored into a new array.
```js
let numbers = [1,2, 3, 4 , 5, 6 ,7]
function isEven (num) {
  return num % 2 === 0 ;
}
let evenNumbers = numbers.filter(isEven) ;
console.log (evenNumbers)   //  (3) [2, 4, 6]
```

