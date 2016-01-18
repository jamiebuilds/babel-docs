# Do Expressions

Compile do expressions to ES5

## Example

**Input**

```js
var x = do { if (test) x; else y }
var x = do { while (x--) y; }
```

**Output**

```js
var x = test ? x : y;
var x = function() {
  var _ret;
  while (x--) _ret = y;
  return _ret;
}();
```

> Note that the output may not be exactly what is above. Babel's implementation
> may have changed since this document was last updated, or the output may have
> been cleaned up for clarity.

## Setup

### Installation

```sh
$ npm install --save-dev babel-plugin-transform-do-expressions
```

### Usage

#### Via `.babelrc` (recommended)

**`.babelrc`**

```json
{
  "plugins": ["transform-do-expressions"]
}
```

#### Via CLI

```sh
babel script.js --plugin transform-do-expressions
```

#### Via Node API

```js
require("babel-core").transform("code", {
  plugins: ["transform-do-expressions"]
});
```
