# TypeTerpret
A JavaScript API for a TypeScript interpreter based on @niutech's TypeScript compiler.

Again, thanks to @niutech for the original compiler & interpreter.

NPM package is coming soon! Meanwhile, use typeterpret-node.js in /dist-node.

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
