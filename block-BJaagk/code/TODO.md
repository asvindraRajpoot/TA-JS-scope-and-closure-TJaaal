1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage=function(marks,total){
   return (marks * 100) / total;
}
let percentage=(marks,total)=>{
   return (marks * 100) / total;
}
let percentage=(marks,total)=> (marks * 100) / total;
   






```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer

let percentage=(marks,total)=>{
   return (marks * 100) / total;
}



```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

Function defination is expression in javaScript because function is an object which can be stored in variable .
exp:
```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

```


4. Why is a function call an expression in JavaScript?

function call is an expression in JavaScript because when we are calling a function we are executing the function defination and function defination can be refered as function expression


5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // VALID
five = add; // VALID
five = five(10, 11); // INVALID
five = function () {
  return 'Hello';
}; // VALID
```

6. What is the difference between function definition and function call? Explain with an example.

Function defination defines the steps which can be performed and function call is to execute those steps defined by functions defination.

exp:

```js

function sub(a,b){

  return a+b;
} /// function defination


sub(2,4);// Function call

```

7. What is the similarities between function definition and function call?

In both cases it tells what are steps are there.


8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // Valid
```
here hello() is function and a function is an object so we can define the property.



9. What is higher order function explain with an example.
Higer order function is which itself consist multiple fucntion defination  inside it.that is higher order function.
exp:

```js
function hello(function(a,b)=>{
  return a+b;
}) {
  console.log('Hello World!');
}
//here hello is consisting one function that is why hello is higher order function


```



10. Explain what is callback function. Why you can pass a function inside a function?

callback function is a function which is called inside a function which returns some value
and it is always inside the higher order function.


```js
function mul((a,b)=>a*b);

//here mul is higher order function and inside that one expression is there that is call back function which  is performing multiplication so that is called callback function.
