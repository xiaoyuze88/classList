# classList.js #

This is a tiny plugins with less than 100 lines codes to help you easier to deal with DOM's className when your project don't need library like jQuery. 
For modern browser, we use the HTML5 classList api to deal with className, otherwise, for browsers like IE9-, we use our function to deal with them.

## Quick Start ##

```javascript
//We set classList object to window, so you can use it directly like:

var dom = document.querySelector('#yourDom');
var className = "yourClassName";

classList.addClass(dom,className);
classList.removeClass(dom,className);
classList.toggleClass(dom,className);
classList.hasClass(dom,className);
```

## Parameters ##

```javascript
dom : the dom element that you need to set class name
className : the className that you want to use, 
			you can also set multiple class like : "newClass newClass2 newClass3"
```

## Method ##

classList.addClass    : Add one or more class to the DOM you input.

classList.removeClass : Remove one or more class to the DOM you input.

classList.toggleClass : If the DOM you input has the className, remove it, otherwise, add the className.

classList.hasClass    : If the DOM has the className you input, return true, otherwise ,return false.(For this method, you can only input one className at one time.)

## More ##

1. You can set multiple classes at one time like :

```javascript
//add 3 classes at one time
classList.addClass(dom,"newClass newClass2 newClass3");
```
2. We support chain method,so you can do something like this:

```javascript

classList.addClass(dom,'newClass').removeClass(dom,'oldClass').toggle(dom,'newClass oldClass');

```
If you find any issues, please contact me! 
Hope this will help you.
Thanks!
