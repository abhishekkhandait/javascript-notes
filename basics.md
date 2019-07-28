# *Basics*

## Declaration

There are three kinds of declarations in JavaScript.

[`var`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var "The var statement declares a variable, optionally initializing it to a value.") : Declares a variable, optionally initializing it to a value.

[`let`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let "The let statement declares a block scope local variable, optionally initializing it to a value.") : Declares a block-scoped, local variable, optionally initializing it to a value.

[`const`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const "Constants are block-scoped, much like variables defined using the let statement. The value of a constant can't be changed through reassignment, and it can't be redeclared.") : Declares a block-scoped, read-only named constant.

## Variables

Variables are containers that you can store values in. You start by declaring a variable with the `var` or the `let` keyword, followed by any name you want to call it:

```javascript
let myVariable;
```

> - JavaScript is case sensitive — `myVariable` is a different variable to `myvariable`
> 
> - You can name a variable nearly anything, but there are some name restrictions. A JavaScript identifier must start with a letter, underscore (_), or dollar sign ($); subsequent characters can also be digits (0-9). 
> 
> - Some examples of legal names are `Number_hits`, `temp99`, `$credit`, and `_name`.



## Datatypes

JS has seven datatypes:

- Boolean: `true` and `false`

- null: A special keyword denoting a null value.

- undefined: A variable/property whose value is not defined

- Number: An integer or floating point number

- String: A sequence of characters that represent a text value. For example: "JavaScript"

- Object:

- Function
  
   some extras:
  
  Symbol, BigInt

### Datatype conversion

JavaScript is a dynamically typed language. That means you don't have to specify the data type of a variable when you declare it, and data types are converted automatically as needed during script execution. So, for example, you could define a variable as follows:

```javascript
var answer = 25;
```

and later ou could assign the same variable a string value, for example:

```javascript
answer = 'my answer'
```

In expressions involving numeric and string values with the + operator, JavaScript converts numeric values to strings. For example, consider the following statements:

```javascript
x = 'The answer is ' + 42 // "The answer is 42"
y = 42 + ' is the answer' // "42 is the answer"
```

In statements involving other operators, JavaScript does not convert numeric values to strings. For example:

```javascript
'37' - 7 // 30
'37' + 7 // "377"
```

#### Type conversion

There are methods for conversion from strings to numbers

- [`parseInt()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt "The parseInt() function parses a string argument and returns an integer of the specified radix (the base in mathematical numeral systems).")
- [`parseFloat()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseFloat "The parseFloat() function parses an argument and returns a floating point number.")


