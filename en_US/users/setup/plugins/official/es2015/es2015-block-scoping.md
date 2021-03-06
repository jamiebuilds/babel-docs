# ES2015 Block Scoping

Compile ES2015 block scoping (const and let) to ES5

## Example

**Input**

```js
const foo = 1;
if (true) {
  let foo = 2;
}
```

**Output**

```js
var foo = 1;
if (true) {
  var _foo = 2;
}
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-block-scoping
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-block-scoping"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-block-scoping
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-block-scoping"]
});
```
