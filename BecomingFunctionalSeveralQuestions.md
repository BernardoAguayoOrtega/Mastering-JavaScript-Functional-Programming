###### tags: `Mastering JavaScript Functional Programming` `javascript`
# Becoming Functional - Several Questions

Functional programming (or FP) has been around since the earliest days of computing, and is going through a sort of revival because of its increased use with several frameworks and libraries, most particularly in JavaScript (JS).

## What is functional programming?

If you go back in computer history, you'll find that the second oldest programming language still in use, Lisp, is based on FP. Since then, there have been many more functional languages, and FP has been applied more widely. But even so, if you ask people what FP is, you'll probably get two widely dissimilar answers.

For trivia or history buffs, the oldest language still in use is Fortran, which appeared in 1957, a year before Lisp. Quite shortly after Lisp came another long-lived language, COBOL, for business-oriented programming.

## A different way of thinking
FP is a different way of writing programs, and can sometimes be difficult to learn. In most languages, programming is done in an imperative fashion: a program is a sequence of statements, executed in a prescribed fashion, and the desired result is achieved by creating objects and manipulating them, which usually means modifying the objects themselves. FP is based on producing the desired result by evaluating expressions built out of functions that are composed together. In FP, it's common to pass functions around (such as passing parameters to other functions or returning functions as the result of a calculation), to not use loops (opting for recursion instead), and to skip side effects (such as modifying objects or global variables).

In other words, FP focuses on what should be done, rather than on how. Instead of worrying about loops or arrays, you work at a higher level, considering what you need to be done. After becoming accustomed to this style, you'll find that your code becomes simpler, shorter, and more elegant, and can be easily tested and debugged. However, don't fall into the trap of considering FP as the goal! Think of FP only as a means to an end, as with all software tools. Functional code isn't good just for being functional, and writing bad code is just as possible with FP as with any other technique!

## What FP is not
Since we have been saying some things about what FP is, let's also clear up some common misconceptions, and look at what FP is not:

- FP isn't just an academic ivory tower thing: It is true that the lambda calculus upon which it is based was developed by Alonzo Church in 1936 as a tool to prove an important result in theoretical computer science (which preceded modern computer languages by more than 20 years!); however, FP languages are being used today for all kinds of systems.
- FP isn't the opposite of object-oriented programming (OOP): It isn't a case of choosing declarative or imperative ways of programming. You can mix and match as best suits you, and we'll be doing this throughout this book, bringing together the best of all worlds. 
- FP isn't overly complex to learn: Some of the FP languages are rather different from JavaScript, but the differences are mostly syntactic. Once you learn the basic concepts, you'll see that you can get the same results in JavaScript as with FP languages.

## Why use FP?
Throughout the years, there have been many programming styles and fads. However, FP has proven quite resilient and is of great interest today. Why would you want to use FP? The question should rather first be, what do you want to get? and only then, does FP get you that? Let's answer these important questions in the following sections.

## Not all is gold
However, let's strive for a bit of balance. Using FP isn't a silver bullet that will automagically make your code better. Some FP solutions are actually tricky, and there are developers who greatly enjoy writing code and then asking, what does this do? If you aren't careful, your code may become write-only and practically impossible to maintain; there goes understandable, extensible, and reusable out the door!

Another disadvantage is that you may find it harder to find FP-savvy developers. (Quick question: how many functional programmers sought job ads have you ever seen?) The vast majority of today's web code is written in imperative, non-functional ways, and most coders are used to that way of working. For some, having to switch gears and start writing programs in a different way may prove an unpassable barrier. 

Finally, if you try to go fully functional, you may find yourself at odds with JavaScript, and simple tasks may become hard to do. As we said at the beginning, we'll opt for sorta FP, so we won't be drastically rejecting any language features that aren't 100% functional. After all, we want to use FP to simplify our coding, not to make it more complex!

Is JavaScript functional?

