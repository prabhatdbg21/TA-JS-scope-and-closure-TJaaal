Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside {} and we can't access the variable defined inside {} from outside.

The above code will throw an error `Reference Error username is not defined`.


3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside if loop and we can't access the variable defined inside if loop from outside.

The above code will throw an error `Reference Error username is not defined`.


4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope with
value Arya

The above code will throw value `Arya`.


5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope but it not initialized. 

The above code will throw an error `Identifier 'username' has already been declared`.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope with value john. 

The above code will throw value `John`.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope with value john. 

The above code will throw value `John`.


8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); /*
                            0 'First'
                            1 'First'
                            2 'First'
                            3 'First'
                            4 'First'
                            5 'First'
                            6 'First'
                            7 'First'
                            8 'First'
                            9 'First'
                            */
}
console.log(i, 'Second'); // 10 'Second'
```

In above code we are looking for the variable named `i`. Here `i` is initalized .


9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); /*
                            0 'First'
                            1 'First'
                            2 'First'
                            3 'First'
                            4 'First'
                            5 'First'
                            6 'First'
                            7 'First'
                            8 'First'
                            9 'First'
                            */
}
console.log(i, 'Second'); //  i is not defined
```
In above code we are looking for the variable named `i`. Here `i` is not initalized .