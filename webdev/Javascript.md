# Javascript:


- ## Hello world test:
open the developer tools in the browser by pressing `F12`, `Shift+Ctrl+i` or even
just right click on the page and select inspect.


once you have the window up, you will see multiple tabs, they're all the developer tools.
we will be focusing on the console.

this Javascript console allows us to execute code on the page and it can be very handy to debug or just run some code.

Lets use the console to write some javascript code,

type in the console
```js
alert("Hello world")
```
alert is a function, and to execute this function we add the paranthesis at the end, inside the paranthesis is the data that we want to give it (in this example is "Hello world").


Okey, but ofcourse we can do alot more
which of course you don't need to understand yet
I just want to show you some stuff that we can do,
you will understand them later on when we progress

**add an experiment using variable, if statement and alert and then explain it**


**show that we can use the console as a calculator**



- ### Linking Javascript:
Now we will be looking at how are we gonna use javascript with with our website

- Open a directory using vscode
- install an extension called `live share` (optional but useful)
- make `index.html` and type `!` then enter to generate the html page
- make a script tag, inside we will be running some js code.

Now, lets talk
we use the script tag, to tell the browser that we want to run or link to a js file.

writing javascript code on the html file is kind of tedious

let's first write the code from last time, in here, and see



so lets learn how to link a js file

in the script tag you add src atribute, and give it the location of the js file
```html
<script src="/your-awsome-spagettie-code.js">
</script>
```

it can use the relative location
`./file.js`
or absolute from the url
`/file.js`
or from another domain entirely
`https://cdn.whatever.com/file.js`



- note: debugging tools
we will be using `console.log` function instead of `alert`  because it's more convenient (if it get triggered multiple times it will be a mess)

ex: `console.log("Hello World")`

- ### values and variables

basic value types can either be number, string, array, object or even a function

the sweet thing about js is that we don't need special syntax for each one.

- the variable always start with either
`let`
or 
`const`

the basic difference between them is that let can be changed later
and const is short for  the word constant which cannot be changed once assigned




```js

let isJsFun = true; // boolean
let whyIsItFun = "cuz i can do anything"; // text

let myGlodenRatio = 1.641; // number

// arrays
let alphabets = [
	"a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r",
	"s","t","u","v","w","x","y","z"
] // array of strings

let numbersTo10 =[
	1,2,3,4,5,6,7,8,9
] // array of numbers


// mixed array
let whatever = [true,"asdf",69420,[]]


// object
let jeff = {};
jeff.age = 22; // pretty old :(
jeff.height = "5'1" // pretty short :<
```

```js
const pi = 4.213;

// trying to change a constant
pi = 4.321; // will not work


const ourGalaxyName = "milkyway";

// trying to change a constant
ourGalaxyName = "urmom's name"; // unfortunetly will not work


// but for objects and arrays it's slightly different
const myarr = [1,2,3];

myarr = [1,2,3,4] // will not work,



```
you basically can't use the `=` directly on a constant, but you can use it on a child of his

```js
const myarr = [1,2,3];

myarr.push(4) // [1,2,3,4]


const jeff = {}; 

jeff.age = 69;
jeff.height = "420cm";

console.log(jeff) // { age:69, height:"420cm" }
```

- we can do math calculations in javascript, surperise!

```js
let wello = 10 * 20; 
console.log(wello) // logs 30

```


## Expand your thoughts:

```js
// you can also 
// make an empty array
const imEmptyInside = [];

// and add stuff to it
imEmptyInside.noLonger = "asdf"

// you can also give it another object as a property
imEmptyInside.notSoMuch = {
  heyImHereNow: true
}

// and you can do the same thing with its sub objects
imEmptyInside.notSoMuch.heyImHereNow2 = false;

// but watch out for trying to set a property on a object that doesn't exist
imEmptyInside.tooMuch.wellIShouldNotExist = true; // Error


```

```js
// you can do the same thing with arrays, the same thing with objects

// arrays are just custom objects that their keys (notSoMuch,...etc) are numbers
// at lest in the logical side of it
// the object needs to know that its an array to use the push pop..etc functions


const arr=[
 "i'm the first item",
 {
   notSoMuch:{
     heyImHereNow: true
   }
 }
]


// just to show you
const arrGeneric = {
 1:"i'm the first item",
 2:{
    notSoMuch:{
	    heyImHereNow: true
    }
 }
}

// if you don't like nesting things (like i do), you can define them as their own variable and pass them in

const notSoMuch ={
	heyImHereNow: true
}

const E2={
	notSoMuch // it's the same as saying notSoMuch: notSoMuch (a shortcut)
}

const arr2 = [
	"i'm the first item",
	E2 // not that you can do E2: E2, because property E2 doesn't exist in arr2, and the type of bracket (array backets) prevent you from specifing the index(key)
]


```

### to note:
- Objects are the most generic thing in javascript
- Arrays are just objects on steroids
- 