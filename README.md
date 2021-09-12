# TypeTerpret
A JavaScript API for a TypeScript interpreter based on @niutech's TypeScript compiler.

Again, thanks to @niutech for the original compiler & interpreter.

To use it for NodeJS, run ```npm install typeterpret```. Note that the NPM module reads from your node_modules folder to get the interpreter, so you will need read access to node_modules.

Note: the NPM module uses JSDOM to implement the needed browser features to work.

# Usage
## Browser
```javascript
var code=`
var stringTest:string = "Hello World!";
console.log(stringTest);
`;
      TypeTerpret.eval(code, function(a){
        alert(a);
      });
```

## NodeJS
```javascript
var code=`
var stringTest:string = "Hello World!";
console.log(stringTest);
`;

var TypeTerpret=require('typeterpret');

TypeTerpret.eval(code, function(a){
        console.log(a);
});
```
