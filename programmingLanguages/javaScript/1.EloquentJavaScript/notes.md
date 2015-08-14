# [Eloquent Java Script][1]
## [1][2]. Values, Types and Operators

* ECMA Script 5 is used in this book.
* Six basic types of values exist in java Script
  * Number
  * Boolean
  * String
  * Objects
  * Functions
  * Undefined

*  Many operations in the language that don’t produce a meaningful value (you’ll see some later) yield undefined simply because they have to yield some value.
* `null` and `undefined` are used to denote the absence of meaningful value.
>The difference in meaning between `undefined` and `null` is an accident of JavaScript’s design, and it doesn’t matter most of the time. In the cases where you actually have to concern yourself with these values, I recommend treating them as interchangeable (more on that in a moment).  

**Numbers**
* fixed 64 bits
* scientific notation - 2.98e8
* fractional number calculations are imprecise
* `Infinity, -Infinity and NaN` are considered numbers but don't behave so
* there is only one value in java script that is not equal to itself
```
 console.log(NaN == NaN);
 // -> false
```
NaN is supposed to denote the result of a non sensical computation and as such is not equal to the result of any other nonsensical computation.


**Strings**
* '' and "" are valid
* concatenation operator is +
* `typeof` operator is like `instanceOf` in java
* string comparison is based on _Unicode_ standard


**Boolean**
* `true` or  `false`

**Logical Operators**
* java script supports three logical operators: `and, or, not`

**Automatic Type Conversion(Type Coercion)**
* Type coercion examples
```
console.log(8 * null) // -> 0
console.log("5" - 1) // -> 4
console.log("5" + 1) // -> 51
console.log("five" * 2) // -> NaN
console.log(false == 0) // -> true
```
* When something that doesn’t map to a number in an obvious way (such as "five" or undefined) is converted to a number, the value NaN is produced. Further arithmetic operations on NaN keep producing NaN.
* When null or undefined occurs on either side of the operator `==`, it produces true only if both sides are one of null or undefined.
```
console.log(null == undefined); // → true
console.log(null == 0); // → false
```
This behavior is often useful. When you want to test whether a value has a real value instead of null or undefined, you can simply compare it to null with the `== (or !=)` operator.
* Automatic type conversion is avoided using the operators `=== or !==`.

## [2][3] Program Structure
## [3][4] Functions



[1]: http://eloquentjavascript.net/
[2]: http://eloquentjavascript.net/01_values.html
[3]: http://eloquentjavascript.net/02_program_structure.html
[4]: http://eloquentjavascript.net/03_functions.html
