1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

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

function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

function expression

```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

function expression /anonymous function
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};

function expression / arrow functionn
```

```js
let percentage = (marks, total) => (marks * 100) / total;

function expression / arrow functionn  n   
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

In Javascript object can be assigned to a variable and function is an object. So, a function can be assigned to a variable which became a function expression.

4. Why is a function called as an expression in JavaScript?

Because function always return a value like a expression. 

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // valid, add with arguments wil call the function
five = add; // valid the execution step inside add function will be assign to variable five.
five = five(10, 11); // valid 
five = function () {
  return 'Hello';
}; //  valid, it's a function expression
```

6. What is the difference between function definition and function call? Explain with an example.

-Function is block of code which has a name and inside execution steps so that you can call it as many time you wish. Whereas, function call is used to call the same function with the name and arguments.

7. What is the similarities between function definition and function call?

- Both is an expression 

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
} 

hello.user = 'Sam'; // valid
```

9. What is higher order function explain with an example.

When a function accepts a function as an argument or it returns a function, then the function will be called as a higher order function.
```js
function isEven(num){
  return num % 2 === 0;  
}
function filter(arr, fn){
  for(let ele of arr){
    if(fn(ele)){
      console.log(ele)
    }
  }
}

filter([1,2,3,4,5,6],isEven)
```
10. Explain what is callback function. Why you can pass a function inside a function?

-When a function passes into another function as an argument which gets invoked inside that function is known as a callback function.
Because function is an expression in javascript so it can be passed as an argument.