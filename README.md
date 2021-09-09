# TypeTerpret
A JavaScript API for a TypeScript interpreter based on @niutech's TypeScript compiler.

Again, thanks to @niutech for the original compiler & interpreter.

# Usage
```javascript
var code=`
var stringTest:string = "Hello World!";
console.log(stringTest);
`;
      TypeTerpret.eval(code, function(a){
        alert(a);
      });
```
