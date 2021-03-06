# Front-end Job Interview Questions

This file contains a number of front-end interview questions that can be used when vetting potential candidates. It is by no means recommended to use every single question here on the same candidate (that would take hours). Choosing a few items from this list should help you vet the intended skills you require.

**Note:** Keep in mind that many of these questions are open-ended and could lead to interesting discussions that tell you more about the person's capabilities than a straight answer would.

## Table of Contents

  1. [General Questions](#general-questions)
  1. [HTML Questions](#html-questions)
  1. [CSS Questions](#css-questions)
  1. [JS Questions](#js-questions)
  1. [Testing Questions](#testing-questions)
  1. [Performance Questions](#performance-questions)
  1. [Network Questions](#network-questions)
  1. [Coding Questions](#coding-questions)
  1. [Fun Questions](#fun-questions)

## Getting Involved

  1. [Contributors](#contributors)
  1. [How to Contribute](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/CONTRIBUTING.md)
  1. [License](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/LICENSE.md)

#### General Questions:

* What did you learn yesterday/this week?
* What excites or interests you about coding?
* What is a recent technical challenge you experienced and how did you solve it?
* What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?
Maintain a clean file structure and code to ensure other developers with no experience with the project could hop in and understand what's going on.

* Talk about your preferred development environment.
Sublime Tools running an eslint of some type, depending on the project. Chrome for the awesome developer tools, hyper for the beautiful terminal, then usually react-native-standalone-dev-tools.

* Which version control systems are you familiar with?
Git with services such as GitHub, BitBucket, and Ajira.

* Can you describe your workflow when you create a web page?


* If you have 5 different stylesheets, how would you best integrate them into the site?
Generally, I would compile them into one stylesheet with some webpack configuration.

* Can you describe the difference between progressive enhancement and graceful degradation?

* How would you optimize a website's assets/resources?
Minifying code, hosting appropriate assets on CDN's. Perhaps server side render if the project called for it. With images, I'd convert all static images into a compressed form or possibly even WebP. 

* How many resources will a browser download from a given domain at a time?
  * What are the exceptions?
  
* Name 3 ways to decrease page load (perceived or actual load time).
Code Splitting, decreasing time to first paint, server-side rendering.

* If you jumped on a project and they used tabs and you used spaces, what would you do?
Alter my sublime to use tabs instead of spaces, adjusting to their given width.

* Describe how you would create a simple slideshow page.
* If you could master one technology this year, what would it be?
Progressive Web Apps!

* Explain the importance of standards and standards bodies.
* What is Flash of Unstyled Content? How do you avoid FOUC?

* Explain what ARIA and screenreaders are, and how to make a website accessible.

* Explain some of the pros and cons for CSS animations versus JavaScript animations.

* What does CORS stand for and what issue does it address?
Cross Origin Resource Sharing. CORS allows you to access resources from a server on a different domain.

#### HTML Questions:

* What does a `doctype` do?
Defines the language the page is being written in.

* What's the difference between full standards mode, almost standards mode and quirks mode?

* What's the difference between HTML and XHTML?

* Are there any problems with serving pages as `application/xhtml+xml`?

* How do you serve a page with content in multiple languages?
* What kind of things must you be wary of when design or developing for multilingual sites?
* What are `data-` attributes good for?
* Consider HTML5 as an open web platform. What are the building blocks of HTML5?
* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
* Describe the difference between `<script>`, `<script async>` and `<script defer>`.
* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions? 
CSS: To decrease the possibility of FOUC. JS: To render all client facing UI before you load JS files will decrease time to first paint.

* What is progressive rendering?
* Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.
* Have you used different HTML templating languages before?

#### CSS Questions:

* What is the difference between classes and IDs in CSS?
Specificity. Id's take preference over classes and are generally used once. Classes can be used multiple times.

* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
Reset removes all browser given styles. Normalizing sets a base starting point for your styles. I would use normalizing because I do believe there is value in having semantic tags built in styling such as H1-H6.

* Describe Floats and how they work.
* Describe z-index and how stacking context is formed.
* Describe BFC(Block Formatting Context) and how it works.
* What are the various clearing techniques and which is appropriate for what context?
* Explain CSS sprites, and how you would implement them on a page or site.
* What are your favourite image replacement techniques and which do you use when?


##### My favorite image replacement technique is the App Shell Method, designed by Google. I use it when I have sections of a website that will eventually be populated with data, but when I don't want to show just a blank screen. This increases user experience and retention.


* How would you approach fixing browser-specific styling issues?
I would use vendor-specific css tags. 

* How do you serve your pages for feature-constrained browsers?
* What techniques/processes do you use?
* What are the different ways to visually hide content (and make it available only for screen readers)?
* Have you ever used a grid system, and if so, what do you prefer?
I have used Bootstraps grid system, though I far prefer css grid as that's just one less CDN that I need to bring in, which will decrease load page loading time.

* Have you used or implemented media queries or mobile specific layouts/CSS?
I have. Mobile First is the way to go!

* Are you familiar with styling SVG?
* How do you optimize your webpages for print?
* What are some of the "gotchas" for writing efficient CSS?
Keeping dry! 
* What are the advantages/disadvantages of using CSS preprocessors?
* Describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
* Explain how a browser determines what elements match a CSS selector.
* Describe pseudo-elements and discuss what they are used for.
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.


* What does ```* { box-sizing: border-box; }``` do? What are its advantages?

Border box will include padding and border in the width and height of an element.

* List as many values for the display property that you can remember.
block, inline-block, flex, inline-flex, inline, table, grid, none

* What's the difference between inline and inline-block?
You can add height and width to inline-block;

* What's the difference between a relative, fixed, absolute and statically positioned element?
* The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?


* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
I have used Bootstrap, Tiny, Propeller and MDBootstrap.


* Have you played around with the new CSS Flexbox or Grid specs?
Yes! It's the best.

* How is responsive design different from adaptive design?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?

#### JS Questions:

* Explain event delegation
##### Event delegation allows us to attach a single event listener, to a parent element, that will fire for all descendants matching a selector.


* Explain how `this` works in JavaScript
* Explain how prototypal inheritance works


* What do you think of AMD vs CommonJS?
* Explain why the following doesn't work as an IIFE: `function foo(){ }();`.
  * What needs to be changed to properly make it an IIFE?
* What's the difference between a variable that is: `null`, `undefined` or undeclared?
  * How would you go about checking for any of these states?
* What is a closure, and how/why would you use one?
* Can you describe the main difference between a `forEach` loop and a `.map()` loop and why you would pick one versus the other?
* What's a typical use case for anonymous functions?
* How do you organize your code? (module pattern, classical inheritance?)
* What's the difference between host objects and native objects?
* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
* What's the difference between `.call` and `.apply`?
* Explain `Function.prototype.bind`.
* When would you use `document.write()`?
* What's the difference between feature detection, feature inference, and using the UA string?
* Explain Ajax in as much detail as possible.
* What are the advantages and disadvantages of using Ajax?
* Explain how JSONP works (and how it's not really Ajax).
* Have you ever used JavaScript templating?
  * If so, what libraries have you used?
* Explain "hoisting".
* Describe event bubbling.
* What's the difference between an "attribute" and a "property"?
* Why is extending built-in JavaScript objects not a good idea?
* Difference between document load event and document DOMContentLoaded event?
* What is the difference between `==` and `===`?
* Explain the same-origin policy with regards to JavaScript.
* Make this work:
```javascript
function duplicate(arr){
  return arr.concat(arr);
}

duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```
* Why is it called a Ternary expression, what does the word "Ternary" indicate?
A ternary is syntactic sugar on a conditional statement. Instead of using if and then, you'd use ? and :

if ? then : else

Ternary indicates there are three sections.

* What is `"use strict";`? what are the advantages and disadvantages to using it?
* Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`

```javascript
function fizzBuzz(num) {
	let count = 0;
	while (count <= num) {
		if (!(count % 5) && !(count % 3) && count) {
			console.log('fizzbuzz');
		} else if (!(count % 3)) {
			console.log('fizz');
		} else if (!(count % 5)) {
			console.log('buzz');
		}
		count++;
	}
}
```

* Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
* Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?
* Explain what a single page app is and how to make one SEO-friendly.
* What is the extent of your experience with Promises and/or their polyfills?
I am well versed in Promises, asynchronous programming is a daily tool that I utilize. 

* What are the pros and cons of using Promises instead of callbacks?

* What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?

* What tools and techniques do you use debugging JavaScript code?
I use the chrome console along with React DevTools, Redux DevTools, and breakpoints.

* What language constructions do you use for iterating over object properties and array items?
For in loops, map, reduce, filter, for each, every and I try to avoid standard for loops whenever possible.

* Explain the difference between mutable and immutable objects.
  * What is an example of an immutable object in JavaScript?
  * What are the pros and cons of immutability?
  * How can you achieve immutability in your own code?
* Explain the difference between synchronous and asynchronous functions.
* What is event loop?
  * What is the difference between call stack and task queue?
  
* Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`

* What are the differences between variables created using `let`, `var` or `const`?
`var` is function scope, `let` and `const` are block scope. 
`const` means that the variable can't be reassigned. 
`let` and `var` can be reassigned.

#### Testing Questions:

* What are some advantages/disadvantages to testing your code?
* What tools would you use to test your code's functionality?
* What is the difference between a unit test and a functional/integration test?
* What is the purpose of a code style linting tool?

#### Performance Questions:

* What tools would you use to find a performance bug in your code?
* What are some ways you may improve your website's scrolling performance?
* Explain the difference between layout, painting and compositing.

#### Network Questions:

* Traditionally, why has it been better to serve site assets from multiple domains?
* Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.
* What are the differences between Long-Polling, Websockets and Server-Sent Events?
* Explain the following request and response headers:
  * Diff. between Expires, Date, Age and If-Modified-...
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options
* What are HTTP methods? List all HTTP methods that you know, and explain them.

#### Coding Questions:

*Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```

*Question: What will be the output of the code below?*
```javascript
console.log(0.1 + 0.2 == 0.3);
```
false. this is because of how javascript uses floating point numbers.

*Question: How would you make this work?*
```javascript
add(2, 5); // 7
add(2)(5); // 7
```

*Question: What value is returned from the following statement?*
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```
"hog angasal a m'i"

*Question: What is the value of `window.foo`?*
```javascript
( window.foo || ( window.foo = "bar" ) );
```

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```
Hello World followed by "bar is not defined"

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```
2


*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```
undefined

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

*Question: What is the difference between these four promises?*
```javascript
doSomething().then(function () {
  return doSomethingElse();
});

doSomething().then(function () {
  doSomethingElse();
});

doSomething().then(doSomethingElse());

doSomething().then(doSomethingElse);
```


#### Fun Questions:

* What's a cool project that you've recently worked on?
* What are some things you like about the developer tools you use?
I love sublime because it's so customizable visually. Sounds a bit superficial and silly, but I couldn't use VSCode because I don't believe it's UI is visually appealing. I'll have a hard time spending 8+ hours a day staring at a program that isn't beautiful. 
* Who inspires you in the front-end community?
* Do you have any pet projects? What kind?
* What's your favorite feature of Internet Explorer?
Deprecation per the new TLS standards :-)
* How do you like your coffee?
Black as night.


#### Contributors:

This document started in 2009 as a collaboration of [@paul_irish](https://twitter.com/paul_irish) [@bentruyman](https://twitter.com/bentruyman) [@cowboy](https://twitter.com/cowboy) [@ajpiano](https://twitter.com/ajpiano)  [@SlexAxton](https://twitter.com/slexaxton) [@boazsender](https://twitter.com/boazsender) [@miketaylr](https://twitter.com/miketaylr) [@vladikoff](https://twitter.com/vladikoff) [@gf3](https://twitter.com/gf3) [@jon_neal](https://twitter.com/jon_neal) [@sambreed](https://twitter.com/sambreed) and [@iansym](https://twitter.com/iansym).

It has since received contributions from over [100 developers](https://github.com/h5bp/Front-end-Developer-Interview-Questions/graphs/contributors).
