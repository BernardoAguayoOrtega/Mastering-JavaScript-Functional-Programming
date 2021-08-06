###### tags: `Mastering JavaScript Functional Programming` `javascript`

# Is JavaScript functional?

At about this time, there is another important question that you should be asking: Is JavaScript a functional language? Usually, when thinking about FP, the list of languages that are mentioned does not include JavaScript, but does include less common options, such as Clojure, Erlang, Haskell, and Scala; however, there is no precise definition for FP languages or a precise set of features that such languages should include. The main point is that you can consider a language to be functional if it supports the common programming style associated with FP. Let's start by learning about why we would want to use JavaScript at all and how the language has evolved to its current version, and then see some of the key features that we'll be using to work in a functional way.

# JavaScript as a tool
What is JavaScript? If you consider popularity indices, such as the ones at www.tiobe.com/tiobe-index/ or http://pypl.github.io/PYPL.html, you'll find that JavaScript is consistently in the top ten most popular languages. From a more academic point of view, the language is sort of a mixture, borrowing features from several different languages. Several libraries helped the growth of the language by providing features that weren't so easily available, such as classes and inheritance (today's version of the language does support classes, but that was not the case not too long ago), that otherwise had to be achieved by doing some prototype tricks.

avaScript has grown to be incredibly powerful. But, as with all power tools, it gives you a way to not only produce great solutions, but also to do great harm. FP could be considered as a way to reduce or leave aside some of the worst parts of the language and focus on working in a safer, better way; however, due to the immense amount of existing JavaScript code, you cannot expect it to facilitate large reworkings of the language that would cause most sites to fail. You must learn to live with the good and the bad, and simply avoid the latter parts.

If we ask whether JavaScript is actually functional, the answer will be, once again, sorta. It can be seen as functional because of several features, such as first-class functions, anonymous functions, recursion, and closures—we'll get back to this later. On the other hand, it also has plenty of non-FP aspects, such as side effects (impurity), mutable objects, and practical limits to recursion. So, when programming in a functional way, we'll be taking advantage of all the relevant, appropriate language features, and we'll try to minimize the problems caused by the more conventional parts of the language. In this sense, JavaScript will or won't be functional, depending on your programming style!

If you want to use FP, you should decide which language to use; however, opting for fully functional languages may not be so wise. Today, developing code isn't as simple as just using a language; you will surely require frameworks, libraries, and other sundry tools. If we can take advantage of all the provided tools but at the same time introduce FP ways of working in our code, we'll be getting the best of both worlds, never mind whether JavaScript is functional!

# Going functional with JavaScript

JavaScript has evolved through the years, and the version we'll be using is (informally) called JS10, and (formally) ECMAScript 2019, usually shortened to ES2019 or ES10; this version was finalized in June 2019. The previous versions were as follows:

* ECMAScript 1, June 1997
* ECMAScript 2, June 1998, which was basically the same as the previous version
* ECMAScript 3, December 1999, with several new functionalities
* ECMAScript 5, December 2009 (and no, there never was an ECMAScript 4, because it was abandoned)
* ECMAScript 5.1, June 2011
* ECMAScript 6 (or ES6; later renamed ES2015), June 2015
* ECMAScript 7 (also ES7, or ES2016), June 2016
* ECMAScript 8 (ES8 or ES2017), June 2017
* ECMAScript 9 (ES9 or ES2018), June 2018

# Key features of JavaScript

JavaScript isn't a purely functional language, but it has all the features that we need for it to work as if it were. The main features of the language that we will be using are as follows: 

* Functions as first-class objects
* Recursion
* Arrow functions
* Closures
* Spread

## Functions as first-class objects
Saying that functions are first-class objects (also called first-class citizens) means that you can do everything with functions that you can do with other objects. For example, you can store a function in a variable, you can pass it to a function, you can print it out, and so on. This is really the key to doing FP; we will often be passing functions as parameters (to other functions) or returning a function as the result of a function call. 

## Recursion
Recursion is the most potent tool for developing algorithms and a great aid for solving large classes of problems. The idea is that a function can at a certain point call itself, and when that call is done, continue working with whatever result it has received. This is usually quite helpful for certain classes of problems or definitions. The most often quoted example is the factorial function (the factorial of n is written as n!) as defined for nonnegative integer values:

## Closures
Closures are a way to implement data hiding (with private variables), which leads to modules and other nice features. The key concept of closures is that when you define a function, it can refer to not only its own local variables but also to everything outside of the context of the function. We can write a counting function that will keep its own count by means of a closure:

## Arrow functions

Arrow functions are just a shorter, more succinct way of creating an (unnamed) function. Arrow functions can be used almost everywhere a classical function can be used, except that they cannot be used as constructors. The syntax is either (parameter, anotherparameter, ...etc) => { statements } or (parameter, anotherparameter, ...etc) => expression. The first allows you to write as much code as you want, and the second is short for { return expression }. We could rewrite our earlier Ajax example as follows:

## Spread
The spread operator (see https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Operators/Spread_operator) lets you expand an expression in places where you would otherwise require multiple arguments, elements, or variables. For example, you can replace arguments in a function call

