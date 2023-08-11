# JavaScript
1. build the interactivity into web pages - interact with websites
2. VBScript
3. TypeScript

- Node.js and npm
## Important 
1. Direct interaction(dynamically on the client)
2. Backwards compatible (built past still works for today)
3. Central pillar

## Benefits
1. ease-of-use
2. built-in tools
3. use widely
4. Accessible
5. Community
6. In demand

- Plain JavaScript (Vinilla JS)
- JavaScript Framework(React)
- Node.js (on the server)

# Programming in JavaScript
1. Power Websites - server
2. Communicate with databases - database
3. Native feel to web apps - web

## JS is everywhere
1. React Native
2. Internet of Things

## Browser vendors
1. jQuery : JavaScript Library - write code using its features

## React - 2011
Knockout, Backbone, Angular, Ember, Vue, Alpine
1. Legancy code


# Variable
JavaScript Structure
```javascript
"Luxin"
'Luxin'
"Hello Luxin"
'Hello Luxin'
var person;
undefined
var person = "Luxin"
undefined
person;
'Luxin'

console.log("Hello", person)
Hello Luxin
undefined
```

# Data Type
1. Packing, unpacking(boxes)

- String, Number, Boolean, Null, Undefined, Blgint, Symbol 

2. Null: the absence of a calue
3. Undefined: not assigned a value yet
4. BigInt
5. Symbol: unique identifier

# Operator
1. comparision operators:  >, <, ==, ≠ 
2. logical operators: &&, ||, ! 

# Number
1. 10**2 = 100
2. 9 % 8

# String
1. single quotes or double quotes

# Boolean
100 == “100” //true, regardless of the type
strict equality: 100 === "100"  //false, also check type

1 !== "1" // true

# JavaScript Selectors
1. DOM(Document Object Model) - the framework a browser uses to read and store  webpage

```javascript
document
document.querySelector('p');
document.querySelectorAll('p');
document.getElementById('heading');
document.getElementsByClassName('txt');
```

# Scoping with var, let and const
```javascript
var num1 = 10;

function score(){
    var num2 = 20;
    console.log(nums2);
}
```
1. ES5 JavaScript - Functions build local scope
2. ES6 JavaScript - Block scope

```javascript
//Block scope
let color = 'red';
if(color == 'red'){
    let color == 'blue'
}
console.log(color); //red

//ES5
let user = "Marinda"
```
1. var, let, const

## var, const 
1. can't be used before it is declared
2. variable can't be redeclared
3. it's scoped to the bloc

### Use let if the alue might change in the future, use const if the value will never change

# Functions
DRY: Don't repeat yourself
```javascript
function myFunc(){
    console.log("hi");
}
myFunc();
```
# JavaScript DOM manipulation
1. DOM: a browser builds a DOM, or model, for every webpage it downloads as a JavaScript object
2. Elements Tab
    - Used to interact with the DOM
    - Access through the devtools in the browser window
    - Provides interactivity via the GUI
3. JavaScript
    - Used to interact with the DOM
    - Access JavaScript via the Console tab
    - Access the console panel using the escape key

```javascript 
document.body.innerText = "Hello"

const h2 = document.createElement('h2');
h2.innerText = "This is an h2 heading";
h2.setAttribute('id', 'sub-heading');
h2.setAttribute('class', 'secondary');
document.body.appendChild(h2);
```
The DOM is an in-memory representation of the active HTML document. Any changes made are local and do not affect the document stored on the webserver.

# Event Handling
1. User-triggered events
2. Listen for the events

```javascript
const target = document.querySelector('body');
function handleClick(){
    console.log('click the body');
    
}

target.addEventListener('click', handleClick);
function handleClick2(){
    console.log('clicking the heading');
}
```

```html
<h1 onclick="handleClick2()"> Hi </h1>
```

```javascript
let answer = prompt('What is your name?');
if (typeof(answer) === 'string') {
    var h1 = document.createElement('h1')
    h1.innerText = answer;
    document.body.innerText = '';
    document.body.appendChild(h1);
}


var h1 = document.createElement('h1')
h1.innerText = "Type into the input to make this text change"
var input = document.createElement('input')
input.setAttribute('type', 'text')
document.body.innerText = '';
document.body.appendChild(h1);
document.body.appendChild(input);


var h1 = document.createElement('h1')
h1.innerText = "Type into the input to make this text change"
var input = document.createElement('input')
input.setAttribute('type', 'text')
document.body.innerText = '';
document.body.appendChild(h1);
document.body.appendChild(input);
input.addEventListener('change', function() {
    console.log(input.value)
})


var h1 = document.createElement('h1')
h1.innerText = "Type into the input to make this text change"
var input = document.createElement('input')
input.setAttribute('type', 'text')
document.body.innerText = '';
document.body.appendChild(h1);
document.body.appendChild(input);
input.addEventListener('change', function() {
    h1.innerText = input.value
})
```
# Frameworks and Libraries
1. Libraries: re-usable code, purposely built with specific functionality
2. Frameworks: structures
    - Express, Django, ASP.NET, Rails, Spring
3. HTTP requests


1. Framework
    - Adv: Time Saving, Structure, Best Practice
    - DisAdv: Structure Constraints, Compatibility
2. Libraries
    - Adv: Replace Libraries
    - Dis: Selecting Library Set, Compatibility