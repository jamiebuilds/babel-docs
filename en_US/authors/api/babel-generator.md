## [`babel-generator`](https://github.com/babel/babel/tree/master/packages/babel-generator)

Babel Generator is the code generator for Babel. It takes an AST and turns it
into code with sourcemaps.

Run the following to install it:

```sh
$ npm install --save babel-generator
```

Then use it

```js
import * as babylon from "babylon";
import generate from "babel-generator";

const code = `function square(n) {
  return n * n;
}`;

const ast = babylon.parse(code);

generate(ast, null, code);
// {
//   code: "...",
//   map: "..."
// }
```

You can also pass options to `generate()`.

```js
generate(ast, {
  retainLines: false,
  compact: "auto",
  concise: false,
  quotes: "double",
  // ...
}, code);
```
