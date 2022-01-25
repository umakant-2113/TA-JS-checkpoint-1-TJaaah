1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}
sum(10,5);
this function will return 15.

// second
function sum(a, b) {
  console.log(a + b);
}
sum(10,5);
this function return undefined .
```

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

function sum(a, b) {
return a + b;
}
let first = sum(10,5);
value of first is 15.

function sum(a, b) {
console.log(a + b);
}
let second = sum(10,5);
the value of second is undefined .

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   function sum(a,b,c) {
   return a + b;
   }
   sum(12,24);
   //output 36 we have pass three parameter and give two agruments . we do not give third arguments   
4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
   function sum(a, b) {
   return a + b;
   }
   let add = sum(10,5);

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
   function sayHello(name){
   return `hello ${name}`
   }
   sayHello("umakant");

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();output` hello john `  username variable takes his value outside of the function.
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1
  he is doing alert this massage  `john`

showMessage(); // Output 2
`hello john `


alert(userName); // Output 3
`john`
```

8. What is a Anonymous Function give example of three functions.
   an anonymous function is a function without a name .
   1 const addNumbers = function (numA,numB){
   return numA+numB
   }
   addNumbers(10,12);
   2 const sequar = function(num){
   return num\*num
   }
   sequar(4);
   3 const substract = (numA,numB) => {
   return numA-numB
   }
   substract(10,6);

9. Can function declaration be a Anonymous Function? Explain

function declaration is always start function keyword . anonymous function is not start function keyword .anonymous function can make help of the function expression.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

function get(a,b){
return a+b
}
get(10,5);
2 function calc(temp in fahrenheit){
return (5 \*temp-160)/9
}
calc(50);
function creat(a,b,opretion){
if(opretion === "sum"){
return a+b
}else if(opretion=== "product"){
  return a*b
}

}
creat(5,4,"product");

function check(a,b){
  if(a>b){
    return true
  }else {
    return false
  }
}
check(5,4);