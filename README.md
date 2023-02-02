<p align="center">
 <img src="images/eslint__logo.jpg" alt="ESLint" title="ESLint" width="100%" height="100%" />
</p>
 
 
## `ESLint Documentation`

    ESLint is a tool for identifying and reporting on patterns found in ECMAScript/
    JavaScript code, with the goal of making code more consistent and avoiding bugs.

    ESLint is completely pluggable. Every single rule is a plugin and you can add
    more at runtime. You can also add community plugins, configurations, and parsers
    to extend the functionality of ESLint.

## `Welcome`

Hello Everyone, I'm **`Sajib Bhattacharjee, A passionate Full-Stack Web-Developer`**, I want to welcome you to `ESLint Documentation ` - basics guideline for all.

## `Topics included/covered`

1. [What is ESLint?](#1-what-is-eslint)
2. [Example of Popular Linters](#2-example-of-popular-linters)
3. [Prerequisites of setting up ESLint](#3-prerequisities-for-setting-up-eslint)
4. [Installing & using ESLint](#4-installing--using-eslint)
5. [Some Example & Command](#5-some-example--command)

## 1. `What is ESLint?`

- A linter - tool for identifying and reporting programmatic, stylistic errors.
- ESLint does static error checking before running the program

## 2. `Example of Popular Linters`

- [JSLint](https://www.jslint.com/)
- [ESLint](https://eslint.org/)
- [JSHint](https://jshint.com/)

## 3. `Prerequisities for setting up ESLint`

    - install Node.js
    - install VSCode (as we will use VSCode)

## 4. `Installing & using ESLint`

1. Create package.json: `npm init`
2. Install eslint as dev dependency: `npm install eslint --save-dev `
3. Initialize eslint: `eslint --init` and follow steps:

   - How would you like to use ESLint? To check syntax and find problems
   - How would you like to use ESLint? None of these
   - How would you like to use ESLint? None of these
   - Does your project use TypeScript? › No
   - Where does your code run? Browser

   Go to `.eslintrc.json` file and make add your necessary adjustments
   Example

   ```json
   
   //following codes will activate the recommended rules which can be changed inside the rules object.
     {
      "extends": "eslint:recommended"
     }

    //first value is error level, it can have 3 values: off/0, warn/1, error/2  
    Example of ESLint rules
    "rules": {
        "quotes": ["error", "double"]
    }

    //More Examples of ESLint rules
   "rules": {
       "no-var": "error",
       "eqeqeq": "error",
       "no-unused-vars": "error",
       "default-case": "error",
       "no-console": "error",
       "camelcase": "error",
       "consistent-return": "error",
       "func-style": "error",
       "max-depth": ["error", 2],
       "max-lines": ["error", 25],
       "prefer-arrow-callback": "error",
       "prefer-const": "error",
       "no-useless-return": "error",
       "no-plusplus": "error",
       "quotes": ["error", "single"]
     }

   ```

## 5. `Some Example & Command`

    add some codes in a js file for testing the eslint. I have created
    a file called app.js and added the following codes for testing purpose.

```javascript
var username = "Sajib Bhattacharjee";
var password = "12345";
var occupation = "full stack web developer";
const user_presentaddress = "Bangladesh";

var a = 6;
a++;

console.log(occupation);

const validateUser = (pwd) => {
  if (password == pwd) {
    return true;
  }
};

console.log(validateUser(12345));

switch (foo) {
  case 1:
    console.log(foo);
    break;

  case 2:
    console.log(foo);
    break;
}

const foo = true;
if (foo) {
  if (foo) {
    if (foo) {
      console.log("hi");
    }
    console.log("hi");
  }
  console.log("hi");
}

setTimeout(function () {}, 1000);
```

 ####  - Make some changes in `setting.json`

 ####  - Format on save and validate js codes: add the following codes in `settings.json`

```
 "editor.codeActionsOnSave": {
 "source.fixAll.eslint": true
 },
 "eslint.validate": ["javascript"]
```

> ### Run the eslint: `eslint fileName.js` and check the erros
>
> ### Fix automatically fixable errors: `eslint fileName.js --fix`

</br>

<div 
align="center">

##### `All rights reserved by Sajib Bhattacharjee @2023`

### `Created By-->`

**`-Sajib Bhattacharjee`**

**`Dedicated for 💕"Zahan" 💕`**

> > > > ### Thanks A Lot For Visiting...!!!

</div>
