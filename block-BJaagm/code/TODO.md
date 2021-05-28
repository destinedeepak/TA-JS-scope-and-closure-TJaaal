1. What does thread of execution means in JavaScript?
- Thread of execution defines how a block of code gets executed line by line and how memory gets allocated in global and function execution context.

2. Where the JavaScript code gets executed?
- In Javascript Engine

3. What does context means in Global Execution Context?
- context can an environemnt in where codes gets executed.

4. When do you create a global execution context.
- Global Execution Context gets created when the js engine starts the running code.

5. Execution context consists of what all things?
- Execution context consits of two context i.e. global and function.The Global execution context consits of two area one for memory and second one is for function execution context which created every time on function call and after completion gets deleted. The Function excution context also consists of two area one is for memory and second one for executing the function.

6. What are the different types of execution context?
 Global and Function

7. When global and function execution context gets created?
-  Global execution context gets created when js engine starts running code. But, Function execution context gets created on each function call.

8. Function execution gets created during function execution or while declaring a function.
-  During execution of function.


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/img1.jpg)



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

![](./img/img2.jpg)



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