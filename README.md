### Jump to any Topic:

| Topic    | Topic links                   |
| -------- | ----------------------------- |
| Variable | [Basic Variables](#variables) |

---

# Variables

> Variable is a contener that stores data and save it to memoey location.

#### Example: `var`, `let`, `const`

### Syntex:

```javascript
const variable_name;
let x = 100
var y = 200
```

 | Keyword | Description |
 |---------|------------|
 | `var` | Try to avoid using it because of the **block scoping** issue. |
 | `let` | Introduced in ES6 (2015). Variables declared with `let` have **block scope** and must be **declared before use**. |
 | `const` | Once declared, `const` variables **cannot be reassigned or modified**. |

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
accountPass = "123910"
accountState = "West Bangal"

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
4030
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
<<<<<<< HEAD
>**Use *`let`* insted of *`const`* if you know the value might change in futute**
=======
>**Use *`let`* insted of *`const`* if you know the value might change in futute**
>>>>>>> f991bf3983c40bf97ebdd138e24533b7dd99d340
