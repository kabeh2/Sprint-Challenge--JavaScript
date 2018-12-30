# Sprint Challenge: JavaScript Fundamentals

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a survey of problems. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied variables, functions, object literals, arrays, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a survey of JavaScript problems.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in JavaScript fundamentals.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

You will notice there are several JavaScript files being brought into the index.html file. Each of those files contain JavaScript problems you need to solve. If you get stuck on something, skip over it and come back to it later.

In meeting the minimum viable product (MVP) specifications listed below, you should have a console full of correct responses to the problems given.

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1.  Describe the biggest difference between `.forEach` & `.map`.

        The biggest difference between them is that for .forEach does not return a new array of values
        where map does. .map can be better for functional style programming as it does not mutate the
        original array.

2.  What is the difference between a function and a method?

        The difference between a function and a method is that a function is defined outside of an object
        where a method is a property of an object that is a function.

3.  What is closure?

        Closure is a feature in javascript where an inner function has access to the outer (enclosing)
        function's variables -- a scope chain.

        The closure has 3 scope chains:

            1. It's own scope - variables defined between it's own curly brackets
            2. Access to the outer function's variables
            3. Access to the global variables

        Lexical Scope: is based on where variables and blocks of scope exist at author time, and thus are
        locked down at the end of the lexing phase. Scope is not defined at runtime, rather it can be
        accessed at runtime.


                ```js
                function foo() {  // 'scope of foo' aka lexical scope for bar
                var memory = 'hello closure';
                    return function bar() {
                        console.log(memory);
                        }
                }

                // returns the bar function and assigns it to the identifier 'closure’;
                const closure = foo();
                closure(); // hello closure
                ```

        <code>function scope of outer function === lexical scope of inner function.<code>

4.  Describe the four rules of the 'this' keyword.

        1. In the Global scope, "this" refers to the Global Object.
        2. Implicitly, "this" refers to the object left of the dot.
        3. When using the "new" keyword, "this" is bound to the new object being created.
        4. Explicitly, "this" can be bound using .call(), .apply(), or .bind()

5.  Why do we need super() in an extended class?

        We need super() in an extended class to provide inheritance from parent class, much
        like we would do in ES5 with Object.prototype = Object.create(Super.prototype);

        It can also be used as an object which refers to an instance of Super and call methods of the
        parent class explicitly.

### Git Set up

- [ ] Fork the project into your GitHub user account
- [ ] Clone the forked project into a directory on your machine
- [ ] Create a pull request before you start working on the project requirements. You will continuously push your updates throughout the project.
- [ ] You are now ready to build this project with your preferred IDE

## Minimum Viable Product

Your finished project must include all of the following requirements:

**Pro tip for this challenge: If something seems like it isn't working locally, copy and paste your code up to codepen and take another look at the console.**

## Task 1: Objects and Arrays

Test your knowledge of objects and arrays.

- [ ] Use the [objects-arrays.js](challenges/objects-arrays.js) link to get started. Read the instructions carefully!

## Task 2: Functions

This challenge takes a look at callbacks and closures as well as scope.

- [ ] Use the [functions.js](challenges/functions.js) link to get started. Read the instructions carefully!

## Task 3: Prototypes

Create constructors, bind methods, and create cuboids in this prototypes challenge.

- [ ] Use the [prototypes.js](challenges/prototypes.js) link to get started. Read the instructions carefully!

## Task 4: Classes

Once you have completed the prototypes challenge, it's time to convert all your hard work into classes.

- [ ] Use the [classes.js](challenges/classes.js) link to get started. Read the instructions carefully!

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

There are a few stretch problems found throughout the files, don't work on them until you are finished with MVP requirements!
