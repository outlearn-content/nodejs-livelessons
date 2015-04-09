## Introduction by Marc Wandschneider

<!-- @asset, "name":"intro_screenshot" -->

Here you can see the live version of the [Introductory video](https://www.safaribooksonline.com/library/view/learning-nodejs-livelessons/9780133378023/part00.html).

1. In index.html, add the following line just before the `<script>` element:
```html
<button>Change user</button>
```
2. In `main.js`, add the following code at the bottom of the file, exactly as written — this grabs references to the new button we added and the heading, and stores them in variables:
```javascript
var myButton = document.querySelector('button');
var myHeading = document.querySelector('h1');
```
3. Now add the following function to set the personalized greeting — this won't do anything yet, but we'll use it later on:
```javascript
function setUserName() {
  var myName = prompt('Please enter your name.');
  localStorage.setItem('name', myName);
  myHeading.innerHTML = 'Mozilla is cool, ' + myName;
}
```
