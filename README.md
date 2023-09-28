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









