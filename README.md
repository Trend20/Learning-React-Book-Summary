# Learning React Book Summary.

### Functions

There are two major ways of writing functions in javascript.

**Function Expression**: Not Hoisted(You can't invoke the function before it is defined)

`const sayHi = () => {
    console.log('Hello, this is your favourite frontend developer, Enock);
}
sayHi();
`

**Function Declaration**: Hoisted(You can invoke the function before its declaration)


`function sayHi(){
    console.log('Hello, this is your favourite frontend developer, Enock);
}
sayHi();`

### Hoisting
This is when a function can be invoked before it is declared or defined. Functions defined through function 
expressions are not hoisted while the ones defined using function declaration are hoisted be default.

**Example**

`// Invoking the function before it's declared`


`hey()`

`
function hey(){
    console.log('How are your doing bitch?')
}`

`// invoking the function after it's declared`

`
const hey = () =>{
console.log('How are your doing bitch?')
}`

`hey()`

### Arrow Functions

This is another way of declaring functions without using the `function keyword`. For simple functions, the `block` and the `return` keyword is not a **`MUST`**.

**Example**

`const greetNeighbour = () => console.log('Hello')`

`const sum = (a, b) =>{
    const total = a + b;
    console.log(total);
}
`


If the function only have one parameter, the parenthesis is not required. For more than one parameter, parenthesis is required. 

When returning an object in an arrow function, make sure you wrap the object in a parenthesis.

**Example**

`const person = (firstName, lastName) => return {first: firstName, last: lastName});`

The code snippet above logs an error when called because the function return is not inside a parenthesis.

**Valid solution**

`const person = (firstName, lastName) => return ({first: firstName, last: lastName}));`

**Arrow functions and scope**
Regular functions do not block `this`.

### Objects and Arrays

Most of the creative techniques provided by objects and arrays are widely used in **React**.

**Example**

1. [ ] Destructuring
2. [ ] Object Literal enhancement
3. [ ] Spread Operator.


**Destructuring Objects**

Destructuring assignment allows you to locally scope fields within an
object and to declare which values will be used.

**Example**

consider the object:

`const sandwich = {`

    bread: 'dutch crunch',

    meat: 'tuna',

    cheese: 'swiss',

    toppings:["lettuce", "tomato", "mustard"]
`}`

destructure

`const {bread, cheese} = sandwich;`











