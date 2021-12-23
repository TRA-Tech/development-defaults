
## React
Default **ESLint**, **Stylelint** settings and packages in React applications.

#### [ESLint](https://github.com/eslint/eslint "ESLint")
ESLint is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code.
[Getting Started with ESLint](https://eslint.org/docs/user-guide/getting-started "Getting Started with ESLint")

Firstly you need to download the eslint package.
```
npm install eslint --save-dev
```
Than you need to init eslint.
```
npx eslint --init
```
After that you have to choose these options
```
------------------------------------------------------------------
1- How would you like to use ESLint?
To check syntax, find problems, and enforce code style
------------------------------------------------------------------
2- What type of modules does your project use?
JavaScript modules (import/export)
------------------------------------------------------------------
3- Which framework does your project use?
React
------------------------------------------------------------------
4- Does your project use TypeScript?
**Depends to your project.
------------------------------------------------------------------
5- Where does your code run?
Browser
------------------------------------------------------------------
6- How would you like to define a style for your project?
Use a popular style guide
------------------------------------------------------------------
7- Which style guide do you want to follow? 
Airbnb
------------------------------------------------------------------
8- What format do you want your config file to be in?
JSON
------------------------------------------------------------------
```

**Settings File**
```
.eslintignore
.eslintrc.json
```

#### [Stylelint](https://github.com/stylelint/stylelint "Stylelint")

A mighty, modern linter that helps you avoid errors and enforce conventions in your styles.

**Used Packages**
```
npm install stylelint
npm install stylelint-config-standard
```

**Settings File**
```
.stylelintignore
.stylelintrc.json
```

#### Scripts
```json
"scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "set CI=true&&react-scripts test --coverage",
    "eject": "react-scripts eject",
    "lint:css": "stylelint ./src/**/*.css",
    "lint:js": "eslint ./src/**/*.js"
  }
```
