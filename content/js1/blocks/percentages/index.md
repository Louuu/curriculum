+++
title = '🧩 Percentages'
headless = true
time = 20
facilitation = false
emoji= '🗄️'
[objectives]
    1='Define a parameter'
    2='Construct simple expressions to represent a calculation'
+++

Let's begin with this problem.

> Given a _decimal number_ I want to convert it into a _percentage format_.

For example, given the decimal number `0.5` we return the string `"50%"`. Given the decimal number `0.231` we return the string `"23.1%"`.

### Restating the problem

Our function must convert _any_ decimal to a percentage. We have used functions already. Here are some functions we've used:

```js {linenos=table,linenostart=1}
console.log("hello world"); // logs "hello world" to the console
Math.round(3.141); // evaluates to 3
```

All these expressions are _function calls_: we’re passing input (`"hello world"` or `3.141`) to the functions (`console.log` or `Math.round`) to use their functionality. `Math.round` and `console.log` are functions that the JavaScript language designers have written and stored inside the language, because everyone needs them all the time.

No such pre-built function converts any number to a percentage, so we must write our own. We're going to create a function called `convertToPercentage` with these requirements:

- takes any number input
- converts it to a string in percentage form
- returns that string.

```js {linenos=table,linenostart=1}
convertToPercentage(0.5); // should return "50%"
```

```js {linenos=table,linenostart=1}
convertToPercentage(0.231); // should return "23.1%"
```

### Useful expressions

It is often helpful to solve a problem in one specific instance before doing it for all cases.

In programming, we always try the simplest thing first. Let’s consider how to convert just one number to a percentage. Look at this variable declaration:

```js {linenos=table,linenostart=1}
const decimalNumber = 0.5;
```

We want to create an expression for the percentage using the value of `decimalNumber`. To convert to a percentage, we will multiply the number by 100 and then add a `"%"` sign on the end.

```js {linenos=table,linenostart=1}
const decimalNumber = 0.5;
const percentage = `${decimalNumber * 100}%`;
```

Recalling template literals, the expression in the curly braces will be evaluated first and then inserted into the string, giving us the percentage string.

{{<tabs name="Calculation with variables">}}

{{<tab name="Calculate area">}}

### Generally calculate area and perimeter

These variables describe the dimensions of a rectangle:

```js
const height = 10; // 10 is just an example of a value here - your code should still work if you change this to another value.
const width = 30; // Also just an example - your code should still work if this changes.
```

Create variables [`area`](https://www.bbc.co.uk/bitesize/topics/zjbg87h/articles/zwqt6fr) and [`perimeter`](https://www.bbc.co.uk/bitesize/topics/zvmxsbk/articles/zmrpxbk) for the area and perimeter of the rectangle, by creating expressions from the `height` and `width` variables.

```js
const area = FILL_ME_IN;
const perimeter = FILL_ME_IN;
```

Now give different numbers to `height` and `width`. Are the `area` and `perimeter` values still correct?

{{</tab>}}

{{<tab name="Convert pence">}}

### Generally convert pence to pounds

This variable stores a [price in pence](http://teach.files.bbci.co.uk/skillswise/ma26mone-e3-f-money-pounds-and-pence.pdf):

```js
const price = 130; // Just an example value. Try changing this value to 0, 10, or 1521, and make sure you still get the right answer from your code.
```

Write an expression for the price in pounds. The price in pounds should be shown with 2 decimal places and start with "£".
{{</tab>}}
{{</tabs>}}
