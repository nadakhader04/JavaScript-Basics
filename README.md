
## 📘 JavaScript Basics: window, document, console



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



"color: red" is applied to "Hi"

"color: blue" is applied to "Github



