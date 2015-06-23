![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Assessment for JavaScript Fundamentals

You have 20 minutes

## Instructions

Fork, clone, and npm install.

Follow the prompts below and complete each question.  You may use any resource, other than someone else in the classroom, to help you complete this assessment.

You should save your answers in this README.md file.

# Question 1

```js
var a = 2;
var b = 3;
a = b;
```

After this code executes, what are the values of a and b? Please explain your answer.

a = 3, b = 3. 'a' gets a new value of '3' as a result of assigning operation; 'b' never gets changed

## Question 2

```js
var c = 5;
var d = 2;
c = c + d;
```

After this code executes, what is the value of c?  Please explain what the last line of this program `c = c + d;` means.

c = 7. In the last line 1) the right side of the assignment operation gets evaluated to 7; 2) 'c' gets a new value assigned to it.

## Question 3

```js
var x = 4;
var y = 3;
x = y;
y = 10;
```

After this code executes, what are the values of x and y?  Please explain your answer.

x = 3; y = 10; We assigned new values to each variable in the last two lines.

## Question 4

```js
var weather;
weather = "sunny";
weather === "sunny";
```

What are the values of these expressions?  Explain your answers.

var weather;
undefined  - variable declaration

weather = "sunny";
'sunny' - we assign a new value to weather variable

weather === "sunny";
true - we check if weather variable contains "sunny" in it; and it does!

## Question 5

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi >= 3) {
  console.log("sushi is delicious");
}

if (x > 0) {
  console.log("sushi is tasty");
}
```

Imagine that you take the code from this question, save it to a file called `food.js`, and run `node food.js` in your Terminal.

What would be the output? Explain your answer.

ReferenceError: x is not defined
what happens is the JS interpreter first declares a variable howMuchILikeSushi and assigns a value to it. Then it checks if the (howMuchILikeSushi >= 3) is true (it's not so it proceeds), then it checks if (x > 0) is true. X has never been declared so it spits out an error.

## Question 6

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi > 0) {
  console.log("sushi is tasty");
} else if (x >= 3) {
  console.log("sushi is delicious");
} else {
  console.log("I don't like sushi");
}
```

Imagine that you take the code from this question, save it to a file called `sushi.js`, and run `node sushi.js` in your Terminal.

What would be the output? Explain your answer.

sushi is tasty
what happens is the JS interpreter first declares a variable howMuchILikeSushi and assigns a value to it. Then it checks the first condition (howMuchILikeSushi > 0) which is true. It does what the block says to do (console.log("sushi is tasty");) and stops the "if" execution;

## Question 7

```js
//We'll learn about require later in the course
var ask = require('./ask.js');

var answer = 'not empty';

while (answer !== '' && answer !== 'SeCrEt') {
  answer = ask("Guess my secret? ");
}
```

Imagine that you take the code from this question, save it to a file called `name.js`, and run `node name.js` in your Terminal.

What would you have to type to exit the while loop?  Explain your answer.

SeCrEt
The code (specifically the 'while' loop) will continue requesting an input until 'SeCrEt' or empty string is entered. Then it stops.

---

Commit and push your changes.

Submit a pull request.
