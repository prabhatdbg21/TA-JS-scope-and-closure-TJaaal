1. What does thread of execution means in JavaScript?
```js
// JavaScript engine takes the code and execute line by line this is known as thread of execution .
```

2. Where the JavaScript code gets executed?
```js
// JavaScript code gets executed in JavaScript engine.
```
3. What does context means in Global Execution Context?
```js
// Global Execution Context is the envirement in which we are executing the code and it will created once for each program
```

4. When do you create a global execution context.
```js
// As soon as we execute a code snippet , the JavaScript engine creates a global execution context.
```

5. Execution context consists of what all things?
```js
/*
Execution context consists of two part 
    1) one where we store all the data , variable , function etc .
    2) one where execution happens things like operation manipulation .
*/
```

6. What are the different types of execution context?
```js
/*
Different types of execution context are
      1)  Global Execution Context 
      2)  Function execution context .
*/
```

7. When global and function execution context gets created?
```js
// Global execution context gets created only once by JavaScript engine but can be a multiple Function execution context inside one Global execution context .
```

8. Function execution gets created during function execution or while declaring a function.
```js
// Function execution gets created during function execution .
```


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)