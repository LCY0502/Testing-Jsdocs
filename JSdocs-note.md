# JS Docs Notes
[JSdoc Github](https://github.com/jsdoc/jsdoc)

## setup
Install Globaly with **-g** : `npm install -g jsdoc` or locally :  `npm install jsdoc --save-dev`

If you installed JSDoc globally, run the jsdoc command: 
`jsdoc yourJavaScriptFile.js`

else installed locally:
`./node_modules/.bin/jsdoc yourJavaScriptFile.js`

For genrating docs for multiple files:
```shell
npx jsdoc file1.js file2.js file3.js
``` 
A directory:
```shell
npx jsdoc src/
```
or add **--exclude** to exclude some file
```shell
npx jsdoc src/ --exclude test, node_modules
```

## Run Result
HTML inside the folder `.\out`.

## Quick Guide
[JsDocs Vscode Quick Guide](https://code.visualstudio.com/docs/languages/javascript)

TL;DR: Create comments using `/**` and enter for functions, and use tags to define variable charateristic like `@constant`, `@enum`, `@global` followed by a curly bracket `{type}` and the type of the variable.

Use `@param` and `@example` in function comment.

### Example:
```javascript
/**
 * @const {string} foo <description of the variable>
 */
const foo = 'Hello World';
/**
/**
 * 
 * <Descripton of the function>
 * @param {string} msg  <descripton of the parameter>
 * @example dumy("Hellow World")
 */
function dumy(msg) {...}
```

## Advance and Extension
More reference: [**JSdoc offical webiste** ](https://jsdoc.app/)

Vscode extension: [**DocThis**](https://marketplace.visualstudio.com/items?itemName=oouo-diogo-perdigao.docthis)

To automate checking: [Eslint plugin for jsdocs](https://www.npmjs.com/package/eslint-plugin-jsdoc)