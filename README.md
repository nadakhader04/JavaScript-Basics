## 📘 JavaScript Basics  
### **`window`  `document` `console`**




## Window

The window object represents the browser window or tab. You can also access global functions or variables without explicitly typing window.

```bash
window.username = 'nada';
window.alert(username);

```


## Document
It gives you access to the HTML content of the page and allows you to select, modify, create, or remove elements from the DOM (Document Object Model).


```bash
document.getElementById("title").textContent = "Updated Title";
```


## Console
The console object is used mainly for debugging. It allows to print values, test logic, and track issues while the page runs.

####   You can view the console by right-clicking the page → Inspect → Console tab.

### Console Styling with %c 

```bash
console.log("%cHi %cGithub", "color: red", "color: blue");
```

#### %c is a special placeholder in console.log() that tells the browser: The next string argument is a CSS style to apply to the text following me.



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



"color: red" is applied to "Hi"

"color: blue" is applied to "Github



