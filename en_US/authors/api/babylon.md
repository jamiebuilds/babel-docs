## [`babylon`](https://github.com/babel/babel/tree/master/packages/babylon)

Babylon is Babel's parser. Started as a fork of Acorn, it's fast, simple to use,
has plugin-based architecture for non-standard features (as well as future
standards).

First, let's install it.

```sh
$ npm install --save babylon
```

Let's start by simply parsing a string of code:

```js
import * as babylon from "babylon";

const code = `function square(n) {
  return n * n;
}`;

babylon.parse(code);
// Node {
//   type: "File",
//   start: 0,
//   end: 38,
//   loc: SourceLocation {...},
//   program: Node {...},
//   comments: [],
//   tokens: [...]
// }
```

We can also pass options to `parse()` like so:

```js
babylon.parse(code, {
  sourceType: "module", // default: "script"
  plugins: ["jsx"] // default: []
});
```

`sourceType` can either be `"module"` or `"script"` which is the mode that
Babylon should parse in. `"module"` will parse in strict mode and allow module
declarations, `"script"` will not.

> **Note:** `sourceType` defaults to `"script"` and will error when it finds
> `import` or `export`. Pass `sourceType: "module"` to get rid of these errors.

Since Babylon is built with a plugin-based architecture, there is also a
`plugins` option which will enable the internal plugins. Note that Babylon has
not yet opened this API to external plugins, although may do so in the future.

To see a full list of plugins, see the
[Babylon README](https://github.com/babel/babel/blob/master/packages/babylon/README.md#plugins).
