
## table of contents
| No                  | Link                            |
|--------------------------|---------------------------------|
| 1.             | [Window](#Window) |
| 2.     | [Document](#document) |
| 3.         | [Console](#console) |
| 4.         | [Data Type of JavaScript](#data-type-of-javascript) |
| 5.         | [JavaScript Variables](#javascript-variables) |
| 6. | [Unary Plus and Minus Operator](#unary-plus-and-minus-operator) |
| 7. | [JavaScript if, else, and else if](#javascript-if-else-and-else-if) |



## 📘 JavaScript Basics  
### **`window`  `document` `console`**




## Window

The window object represents the browser window or tab. You can also access global functions or variables without explicitly typing window.

```javascript
window.username = 'nada';
window.alert(username);

```


## Document
It gives you access to the HTML content of the page and allows you to select, modify, create, or remove elements from the DOM (Document Object Model).


```javascript
document.getElementById("title").textContent = "Updated Title";
```


## Console
The console object is used mainly for debugging. It allows to print values, test logic, and track issues while the page runs.

####   You can view the console by right-clicking the page → Inspect → Console tab.

### Console Styling with %c 

```javascript
console.log("%cHi %cGithub", "color: red", "color: blue");
```

#### %c is a special placeholder in console.log() that tells the browser: The next string argument is a CSS style to apply to the text following me.

"color: red" is applied to "Hi"

"color: blue" is applied to "Github



## Data Type of JavaScript 

- String


```javascript
let color = "Yellow";
let country = 'Tulkarm';
```

- Number
```javascript
let length = 16;
let weight = 7.5;
```

- Boolean
```javascript
let x = true;
let y = false;
```

- Object
The object data type can contain both **built-in objects**, and **user-defined objects**:

Built-in object types can be:

**objects, arrays, dates, maps, sets, intarrays, floatarrays, promises**, and more.
```javascript
const person = {firstName:"Nada", lastName:"Khader"};
```

- Array -> Object
```javascript
const cars = ["Saab", "Volvo", "BMW"];
let nums = [1, 45, 7];
```

- null
```javascript
console.log(typeof null); //object
```

- Undefined

```javascript
console.log(typeof undefined); //undefined
```
### ⚠️ Important Notes:
null is not the same as undefined.

"undefined" means: "the variable was declared but never assigned.

"null" means: "the variable was deliberately set to have no value
```javascript
let x;
console.log(x); // undefined

let y = null;
console.log(y); // null

```

## JavaScript Variables
JavaScript Variables can be declared in 4 ways:

- **Automatically**
```javascript
x = 5;
y = 6;
z = x + y;
```
- `var`
```javascript
var x = 5;
var y = 6;
var z = x + y;
```
### ⚠️ Important Note:
**When an element in HTML has an id, it can be accessed directly in JavaScript as a global variable.**



 The element with id="card" in the HTML becomes a variable in JavaScript (declared automatically with var)
The value of this variable is the content inside the <div> element
To update the content, we use the innerHTML property
```javascript
<body>
  <h1>Products</h1>
  <div id="card">this is div</div>
</body>

<script>
  console.log(card); // Prints the <div> element with id "card"
  card.innerHTML = "updated div"; // Updates the content inside the <div>
</script>

```
**❗❗this is not recommended for larger projects.**



- `let`
```javascript
let x = 5;
let y = 6;
let z = x + y;
```
- `const`
```javascript
const x = 5;
const y = 6;
const z = x + y;
```

## Differences


| `Example`               | `var`                              | `let`                                | `const`                             |
|-------------------------|-------------------------------------|--------------------------------------|-------------------------------------|
| **Redeclare**           | ✅ `var x = 2; var x = 3;`           | ❌ `let y = 2; let y = 6;` → *Error*  | ❌ `const z = 2; const z = 6;` → *Error* |
| **Access Before Declare** | 🟡 `console.log(a); var a = 9;` → *undefined* | ❌ `console.log(a); let a = 9;` → *Error* | ❌ `console.log(a); const a = 9;` → *Error* |
| **Added to window object** | ✅ Yes                           | ❌ No                                 | ❌ No                                 |
| **Block Scope**         | ❌ No (function scoped)              | ✅ Yes                                | ✅ Yes                                |




## Unary Plus and Minus Operator
- **Plus**
The unary plus (+) converts an operand into a number, 

```javascript
console.log(+4); //4
console.log(+"4"); //4
console.log(+"-4"); //-4
console.log(+"nada"); //NaN
console.log(+"0xff"); //255
console.log(+null); //0
console.log(+false); //0
console.log(+true); //1
```
- **Minus**
The Unary Negation (-) operator is used to convert its operand to a negative number


```javascript
console.log(-4); //-4
console.log(-"4"); //-4
console.log(-"-4"); //-4
console.log(-"nada"); //NaN
console.log(-"0xff"); //-255
console.log(-null); //-0
console.log(-false); //-0
console.log(-true); //-1
```


## JavaScript if, else, and else if

#### Syntax
```syntax
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
```

**💡Example**

If time is less than 10:00, create a "Good morning" greeting, if not, but time is less than 20:00, create a "Good day" greeting, otherwise a "Good evening":
```javascript
if (time < 10) 
  greeting = "Good morning";

else if (time < 20) 
  greeting = "Good day";

else 
  greeting = "Good evening";

```
The result of greeting will be:
```run
Good morning
```

## Ternary Operator
#### Syntax

```syntax
variable = Expression1 ? ExpressionTrue : ExpressionFalse;
```
**💡Example**

Use ternary operator to find the maximum
```javascript
    let a = 5;
    let b = 9;
    console.log((a > b) ? a : b); // Output: max: 9
```


