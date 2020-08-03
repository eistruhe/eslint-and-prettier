# Setup

## CodeKit

### .scss files
  * set output style to "Compressed"
  * check "Create a source map"
  * check "Run Autoprefixer on the CSS file"
  * set output to "Compile it" and change path if necessary

### .js files
  * set "Check Syntax with" to "Nothing"
  * set "Transpile with" to "Babel"
  * set "ES6 Bundle Format" to "IIFE"
  * check "Minifty the output"
  * set output to "Compile it" and change path if necessary

## VSCode - ESLint, Prettier & Airbnb Setup

### 1. Install ESLint extension for VSCode

Set format on save to true in VSCode

### 2. Install Packages
```bash
npm i --save-dev eslint prettier eslint-plugin-prettier eslint-config-prettier
```

```bash
npx install-peerdeps --dev eslint-config-airbnb
```

### 3. Create .prettierrc for any prettier rules (semicolons, quotes, etc)

### 4. Create .eslintrc.json file (You can generate with eslint --init if you install eslint globally)

```json
{
  "extends": ["airbnb", "prettier"],
  "plugins": ["prettier"],
  "rules": {
    "prettier/prettier": "error",
    "no-unused-vars": "warn",
    "no-console": "off",
    "func-names": "off",
    "no-process-exit": "off",
    "object-shorthand": "off",
    "class-methods-use-this": "off",
    "indent": ["error", 2]
  }
}
```

### Reference
* ESLint Rules - https://eslint.org/docs/rules/
* Prettier Options - https://prettier.io/docs/en/options.html
* Airbnb Style Guide - https://github.com/airbnb/javascript
