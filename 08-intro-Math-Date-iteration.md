# Day 8 - Math/Date JS objects, more iteration

As we continue to embark on our javascript journey, we discover some useful global objects and explore more ways to iterate over data.

Today we covered:

- review datatypes
  - string methods
  - array methods
- global `Date` object
- global `Math` object
- NaN
- while loops
- case statement

## Some String methods

Below are some of the basic string methods we covered in class today, but there are many methods that are useful in working with strings, such as `.toUpperCase()` and `.toLowerCase()`.

- [Check out the MDN to see them all.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)

### `"string".split("")`

<blockquote>
The split() method splits a String object into an array of strings by separating the string into substrings.
</blockquote>

- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)

```js

"javascript".split("");

// ["j", "a", "v", "a", "s", "c", "r", "i", "p", "t"]

```

### `"string".length`

<blockquote>
The length property represents the length of a string.
</blockquote>

- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/length)

```js
"dog".length

// 3

```

### `"string".charAt(index)`

<blockquote>
The charAt() method returns the specified character from a string.
</blockquote>

- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charAt)

```js

"dog".charAt(1);

// "o"

"dog".charAt(2);

// "g"

```

### `"string".concat("another string")`

The `concat()` string method, combines 2 strings into a new string.

```js

"dog ".concat("cat");

// "dog cat"

```

## Date object

The `Date` object is a built-in object that gives you many standard mathematical methods and constants.



## Math object

Below are a few of the methods we covered in class, please consult the [MDN Documentation on the Math Object for more information](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)

### `Math.floor()`

<blockquote>
Returns the largest integer less than or equal to a number "x". Where "x" is the number (parameter)
</blockquote>

- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/floor)

```js

var pi = Math.PI; // 3.141592653589793

Math.floor(pi);

// 3

```

### `Math.ceil()`

<blockquote>
The Math.ceil(x) function returns the smallest integer greater than or equal to a number "x".
</blockquote>

- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/ceil)


```js

var pi = Math.PI; // 3.141592653589793

Math.ceil(pi);

// 4

```
### `Math.random()`

<blockquote>
The Math.random() function returns a floating-point, pseudo-random number in the range [0, 1) that is, from 0 (inclusive) up to but not including 1 (exclusive), which you can then scale to your desired range.  The implementation selects the initial seed to the random number generation algorithm; it cannot be chosen or reset by the user.
</blockquote>

```js

Math.random();

// 0.765003552660346

Math.random();

// 0.8426717962138355

```



## `while() {}` loops

  <blockquote>
  The while statement creates a loop that executes a specified statement as long as the test condition evaluates to true. The condition is evaluated before executing the statement.
  </blockquote> - MDN

  As long as the condition in the while loop evaluates to `true` or is [truthy](http://www.sitepoint.com/javascript-truthy-falsy/), it will execute everything within the body of that statement.

```js
var i = 0;

while(i < 10) {
  console.log("I'm loopy!")
  i++;
}

```
#### NOTE:

Be careful to think about how your condition will terminate.  Infinite loops are much easier to make with a `while` statement.  


## Case statements

<blockquote>
The switch statement evaluates an expression, matching the expression's value to a case clause, and executes statements associated with that case.
</blockquote> - MDN

```js

var calvinLikes = "pizza";

switch(calvinLikes) {
  case "apples":
  case "bananas":
    console.log("calvin doesn't like apples or bananas");
    break;
  case "durian fruit":
    console.log("if he can get past the smell, durian tastes delicious!")
    break;
  case "pizza":
    console.log("YES!  Pizza is soo good!");
    break;
  default:
    console.log("calvin probably likes it");
    break;
}

// "YES!  Pizza is soo good!"

```

## Resources

[Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

[Math](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)
