# Setup

## CodeKit

**.scss files**

- set output style to "Compressed"
- check "Create a source map"
- check "Run Autoprefixer on the CSS file"
- set output to "Compile it" and change path if necessary

**.js files**

- set "Check Syntax with" to "Nothing"
- set "Transpile with" to "Babel"
- set "ES6 Bundle Format" to "IIFE"
- check "Minifty the output"
- set output to "Compile it" and change path if necessary

## SCSS – Prettier

Install Prettier and stylelint extensions for VSCode

## JavaScript - ESLint, Prettier & Airbnb Setup

1. Install ESLint and Prettier extensions for VSCode

2. Install Packages

```bash
npm i --save-dev eslint prettier eslint-plugin-prettier eslint-config-prettier
```

```bash
npx install-peerdeps --dev eslint-config-airbnb
```

**Reference**

- ESLint Rules - https://eslint.org/docs/rules/
- Prettier Options - https://prettier.io/docs/en/options.html
- Airbnb Style Guide - https://github.com/airbnb/javascript
