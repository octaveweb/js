### Jump to any Topic:

| Topic     | Topic links                      |
| --------- | -------------------------------- |
| Variable  | [Basic Variables](#variables)    |
| Data Type | [Basic of Data Tyle](#data-type) |
| Memory    | [Stack & Heap](Memory.md)        |
| Data Conversion    | [Basic data conversion](#data-conversion)        |

---

# Variables

> Variable is a contener that stores data and save it to memoey location.

#### There are 3 types of variable's in JavaScript `var`, `let`, `const`

### Syntex:

```javascript
const variable_name;
let x = 100
var y = 200
```

| Keyword | Description                                                                                                       |
| ------- | ----------------------------------------------------------------------------------------------------------------- |
| `var`   | Try to avoid using it because of the **block scoping** issue.                                                     |
| `let`   | Introduced in ES6 (2015). Variables declared with `let` have **block scope** and must be **declared before use**. |
| `const` | Once declared, `const` variables **cannot be reassigned or modified**.                                            |

<!-- [Back to Topic List](#jump-to-any-topic) -->

## Let's see a Example:

```javascript
const accountId = 4303;
let accountEmail = "demo@gmail.com";
var accountPass = "123456";
accountCity = "Kolkata"; // not a good practice
let accountState;

// console.log() is use to print in console;

console.log(accountId);
console.log(accountEmail);
console.log(accountPass);
console.log(accountCity);
console.log(accountState);
```

### Output:

```javascript
4303
demo@gmail.com
123456
Kolkata
undefined
```

### Change data of variable:

```javascript
accountEmail = "octaveweb@gmail.com";
accountPass = "123910";
accountState = "West Bangal";

console.log(accountEmail);
console.log(accountPass);
console.log(accountState);
```

### Output:

```javascript
octaveweb@gmail.com
123910
West Bangal
```

### See some Error's

```javascript
const accountId = 4303;
console.log(accountId);
```

### Output:

```javascript
4030;
```

### But if we that to assign

```javascript
const accountId = 4303;
console.log(accountId);
accountId = 20; // ❌ Error: Assignment to constant variable.
```

### Output:

```javascript
Error: Assignment to constant variable.
```

> **Use _`let`_ insted of _`const`_ if you know the value might change in futute**

<br>

# Data Type

> "use strict"; Defines that JavaScript code should be executed in "strict mode". more [mode details](https://www.w3schools.com/js/js_strict.asp)

### There are Two type of data

1. `Primitive` data type
2. `Reference` or `Non-primitive` data type

## Primitive Data Type

> Primitive data types are basic data types that are built into a programming language. They are the fundamental building blocks of coding.

### There are 7 primitive date types

| Shortcut |   Meaning   |
| :------: | :---------: |
| 🟢 **N** |  `Number`   |
| ⚪ **N** |   `Null`    |
| 🔵 **B** |  `Boolean`  |
| 🟡 **B** |  `BigInt`   |
| 🔴 **S** |  `String`   |
| 🟣 **S** |  `Symbol`   |
| ⚫ **U** | `Undefined` |

### For some Example:

```javascript
const score = 100; // Number
const scoreValue = 100.3; // Decimal Number

const outsideTemp = null; // Null
const forEmptyValue = null; // Null

const isUserLog = true; // Boolean
const isPMisaCook = false; // Boolean

const longInt = 12345678910111213; // BigInt
const numberAfterN = 12345678910111213n; // BigInt


const yourName = "Karan Swarnakar";// String
const youeEmail = "demo@gmail.com";// String

const sym1 = Symbol(); // Symbol - Empty
const sym2 = Symbol("foo"); // Symbol
const sym3 = Symbol("foo"); // Symbol

const userAge; // Undefined
const userPurches; // Undefined
```

## Non-Primitive/Rererence Data Type

> Non-primitive data types, also known as reference types, include objects, arrays, and functions. These types hold references to memory locations rather than the actual data values.

### There are Two type of data

> `Array`, `object`, `function` are the non-primitive data type [mode details](https://262.ecma-international.org/5.1/#sec-11.4.3)

## For some Example:

```javascript
// Array
const heros = ["Batman", "Supperman", "Flash"];
// Object
let myObj = {
  name: "Karan Swarnakar",
  age: 20,
};
// Function
const myFunction = function () {
  console.log("Hello I am a Function");
};
```

# Data Conversion

> Data conversion is a part of progaming let think data come from data base and it is in object format so we have to change it to our spacific version of data.

### For Example:

```javascript
const score1 = 33;
const score2 = "33sf";
const score3 = null;
const score4 = undefined;

console.log(typeof score1);
console.log(typeof score2);
console.log(typeof score3);
console.log(typeof score4);
```

### Output:

```javascript
Number
String
Object
undefined
```
| Keyword   | Description |
|-----------|-------------|
| `Number()` | Converts a value to a number. |
| `String()`   | A primitive data type representing text. Strings are immutable and String() use for converting data into string.  |
| `Boolean()`  | Represents a logical value (`true` or `false`) and `1` means True, `0` means False.    |

### For Example Number(): 
```javascript
const string_num = "7856321456";
const string_num_cher = "33sf";

const demo1= Number(string_num);
const demo2 = Number(string_num_cher);

console.log(demo1)
console.log(demo2)
```
### Output: 
```javasctipt
7856321456
NaN
```

### Summary: 
```javascript
"43" => 43 
"43abc" => NaN
true => 1 ; false =>0;
```

