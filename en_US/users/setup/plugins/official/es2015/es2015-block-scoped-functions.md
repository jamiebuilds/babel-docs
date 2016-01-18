# ES2015 Block Scoped Functions

Babel plugin to ensure function declarations at the block level are block
scoped.

## Example

**Input**

```js
function foo() {}
if (true) {
  function bar() {}
}
```

**Output**

```js
function foo() {}
if (true) {
  let bar = function() {}
}
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-es2015-block-scoped-functions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-es2015-block-scoped-functions"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-es2015-block-scoped-functions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-es2015-block-scoped-functions"]
});
```
